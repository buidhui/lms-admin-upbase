# Business Rules

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description                  | Version |
| -------------- | --------------- | ----- | ----------------------------------- | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo nội dung quy tắc nghiệp vụ | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Admin CX

**Mục đích:**

1. Mô tả quy tắc hệ thống dùng để tự động xác định ca dạy, đồng bộ dữ liệu và tính công của giảng viên.
2. Mô tả các quy tắc hệ thống áp dụng cho Timeoff Request loại Attendance Adjustment — phân công Approver, cập nhật công sau phê duyệt và check trùng phiếu.
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Hệ thống tích hợp:** Zoom (lớp Online), Dahahi (lớp Offline)
* **Phạm vi:** lớp Offline / Hybrid / Blended / Live Online
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Có dữ liệu log từ Zoom và/hoặc Dahahi.
* Giảng viên đã được mapping với hệ thống.
* Đã có phiếu Timeoff Request loại Attendance Adjustment được tạo trên hệ thống.
{% endhint %}

## II. Quy tắc xác định ca dạy & gộp ca

<details>

<summary>1. Xác định ca dạy và nhóm ca</summary>

**Lấy thông tin ca dạy từ lịch học thực tế:** Hệ thống xác định ca dạy dựa trên **Start Time** và **End Time** thực tế của từng buổi học lấy từ lịch học LMS, không phụ thuộc khung giờ cố định.

**Ngưỡng gộp ca (T):** Hệ thống dùng tham số ngưỡng nghỉ giữa ca **T = 180 phút** (mặc định) để xác định 2 ca có liên tiếp hay không.

**Rule xác định nhóm ca:**

```
Nếu (Start Time[i+1] − End Time[i]) ≤ T
  → Ca i và Ca i+1 là liên tiếp → Gộp vào cùng 1 nhóm

Nếu (Start Time[i+1] − End Time[i]) > T
  → Ca i và i+1 là ca độc lập
```

Mỗi nhóm ca tối đa gồm **2 ca liên tiếp**. Trường hợp trong ngày có 3 buổi học, hệ thống chỉ gộp tối đa 2 ca liên tiếp gần nhau nhất, ca còn lại xử lý độc lập.

</details>

<details>

<summary>2. Khung thời gian tính công theo nhóm</summary>

**Nhóm ca đơn (1 ca):**

```
Start nhóm = Start Time của ca
End nhóm   = End Time của ca
```

**Nhóm ca gộp (2 ca liên tiếp):**

```
Start nhóm = Start Time của ca đầu tiên
End nhóm   = End Time của ca thứ hai
```

Thời gian nghỉ giữa 2 ca trong nhóm gộp **không được tính vào công**. Hệ thống tính công riêng từng ca rồi cộng tổng.

</details>

## III. Quy tắc đồng bộ & xác định check-in / check-out

<details>

<summary>1. Mapping dữ liệu giảng viên</summary>

| Nguồn  | Trường nguồn  | Map sang OPS |
| ------ | ------------- | ------------ |
| Dahahi | Mã giảng viên | Code         |
| Zoom   | Email         | Email        |

</details>

<details>

<summary>2. Rule xác định log hợp lệ</summary>

**Với Zoom:** Áp dụng rule join time / leave time giống học viên.

**Với Dahahi:**

* **Ca đơn:** log hợp lệ nếu nằm trong khoảng **00:00 -> 23:59**
* **Ca gộp:** log hợp lệ nếu nằm trong **±1h30 của start ca sớm** và **±1h30 của end ca muộn**.
* **Ca 1 & Ca 3 (không gộp):** xử lý riêng từng ca theo rule ca đơn.

**Khung thời gian tính công:**

* Chỉ tính trong khoảng thời gian lịch học LMS.
* Nếu check-in sớm hơn Start → tính từ Start.
* Nếu check-out muộn hơn End → tính đến End.

</details>

## IV. Quy tắc tính công

<details>

<summary>1. Công chuẩn &#x26; xác định đi muộn / về sớm</summary>

**Công chuẩn:** Rule **1 giờ = 1 công**. Một ca 3 giờ ⇒ 3 công.

**Đi muộn / về sớm:**

```
Thời gian đi muộn = Check-in sớm nhất (trong khung log hợp lệ) − Start time
  → Nếu > 0  ⇒ Đi muộn

Thời gian về sớm = End time − Check-out muộn nhất (trong khung log hợp lệ)
  → Nếu > 0  ⇒ Về sớm
```

</details>

<details>

<summary>2. Rule tính đủ công / công thực tế</summary>

* Nếu **(đi muộn + về sớm) ≤ 15 phút** ⇒ Tính **đủ công** (ví dụ ca 3 giờ = 3 công).
* Nếu **> 15 phút** ⇒ Tính theo **thời gian dạy thực tế**:

```
Công thực tế = Thời gian dạy thực tế / Thời gian buổi học của 1 công
(Đơn vị tính theo giây, làm tròn đến 4 chữ số thập phân)
```

* Với trường hợp **ca gộp**, công giảng viên = tổng công của các ca đơn.

</details>

<details>

<summary>3. Ví dụ minh họa</summary>

**Ví dụ 1 — Ca đơn, đi muộn > 15 phút:**

Buổi học diễn ra 8:00 – 11:00. Giảng viên dạy từ 8:20:24 – 11:20:00.\
Thời gian tính công: từ 8:20:24 ⇒ 11:00. Thời gian dạy thực tế = 2 giờ 39 phút 36 giây.

```
Công = 2 + 39/60 + 36/3600 = 2.66 công
```

**Ví dụ 2 — Ca gộp 2 ca:**

Giảng viên dạy 2 ca gộp: 8:30 – 11:30 và 14:30 – 17:30. Giảng viên dạy từ 8:45:20 – 17:20:10.

* **Ca 1:** tính công từ 8:45:20 ⇒ 11:30. Đi muộn = 00:15:20 > 15 phút ⇒ tính theo thực tế. Thời gian dạy = 2 giờ 44 phút 40 giây ⇒ **Công = 2.7444 công**.
* **Ca 2:** tính công từ 14:30:00 ⇒ 17:20:10. Về sớm = 00:09:50 < 15 phút ⇒ tính đủ công. Thời gian dạy = 2 giờ 50 phút 10 giây ⇒ **Công = 3 công**.

```
Công tổng = 2.7444 + 3 = 5.7444 công
```

</details>

## V. Quy tắc phân công Approver & email thông báo

<details>

<summary>1. Phân công Approver</summary>

Approver của phiếu được xác định theo Program của Class:

| Điều kiện         | Approver mặc định | Cách xác định (Job Position)                                                                                           |
| ----------------- | ----------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Program = **CMA** | BU Head           | Check theo Job Position của Staff — Level: **Assistant Manager**                                                       |
| Các Program khác  | CX Supervisor     | Check theo Job Position — Level: **CX Supervisor 1 / CX Supervisor 2**. Nếu tồn tại cả 2 → gửi cho **CX Supervisor 2** |

**Approver Deadline:** mặc định **3 ngày** sau ngày tạo Request.

</details>

<details>

<summary>2. Email gửi Approver</summary>

**Khi tạo mới request:**

* Title: _Thông báo request cần phê duyệt: `[Tên request]`_
* Nội dung: Thân gửi `[Tên người duyệt]`. Bạn có một request Attendance Adjustment từ `[Tên giảng viên được tạo Timeoff]` cần duyệt. Để xem thông tin chi tiết về request, vui lòng truy cập vào website của hệ thống: _\<Link>_.

**Khi chỉnh sửa request:**

* Title: _Thông báo request đã được cập nhật: `[Tên request]`_
* Nội dung: Thân gửi `[Tên người duyệt]`. Request Attendance Adjustment `[Tên request]` từ `[Tên giảng viên được tạo Timeoff]` đã được cập nhật. Để xem thông tin chi tiết về request, vui lòng truy cập vào website của hệ thống: _\<Link>_.

</details>

## VI. Quy tắc cập nhật Attendance Tracking theo trạng thái phiếu

<details>

<summary>1. Cập nhật công sau khi duyệt</summary>

Sau khi Timeoff Request chuyển trạng thái:

* **Approved** → hệ thống **tự động cập nhật lại công** của giảng viên (Attendance Tracking) theo thời gian Check-in, Check-out mới.
* **Rejected** → **giữ nguyên** công hiện tại của giảng viên.

</details>

<details>

<summary>2. Cập nhật công khi chỉnh sửa / hủy phiếu</summary>

| Trạng thái phiếu | Edit                                                        | Cancel                                                       |
| ---------------- | ----------------------------------------------------------- | ------------------------------------------------------------ |
| Pending          | Chưa cập nhật Attendance Tracking (phiếu chưa được approve) | Không cập nhật Attendance Tracking, giữ nguyên công hiện tại |
| Approved         | Không cho phép Edit (đã cập nhật công theo mục III.1)       | Không cho phép Cancel                                        |
| Rejected         | Không cho phép Edit, không cập nhật công                    | Không cho phép Cancel                                        |

</details>

## VII. Quy tắc check trùng phiếu Attendance Adjustment

<details>

<summary>1. Định nghĩa phiếu trùng</summary>

Một phiếu được coi là **trùng** khi có cùng tổ hợp:

* `Teacher` (mã giảng viên)
* `Timeoff Date` (ngày/buổi học cần điều chỉnh)
* `Check-in Check-out` (check trùng trong khoảng Check-in, Check-out)

</details>

<details>

<summary>2. Phạm vi trạng thái &#x26; thời điểm đối chiếu</summary>

Chỉ tính trùng với các phiếu **đang còn hiệu lực**:

* `Pending`: đang chờ duyệt, sẽ tác động công nếu được approve.
* `Approved`: đã điều chỉnh công thực tế.

Bỏ qua phiếu `Rejected` và `Cancelled` → cho phép tạo lại phiếu mới cho cùng buổi (vì phiếu cũ đã không còn tác dụng).

**Thời điểm thực thi:** check trùng sau khi click **Save** ở thao tác **Create** và **Edit** Timeoff Request loại Attendance Adjustment.

</details>

<details>

<summary>3. Hành vi khi phát hiện trùng</summary>

| Tình huống phát hiện              | Xử lý                                                                                                                                                                                                                                                                                                                                                                                   |
| --------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Đã tồn tại phiếu `Pending` trùng  | **Chặn cứng** — không cho Save. Hiển thị cảnh báo và link tới màn Edit phiếu Pending để CX kiểm tra/sửa thay vì tạo mới. Noti: _"A pending Attendance Adjustment request already exists for \[Teacher Name] – \[Timeoff Date] - \[Check-in Check-out]. Please review and edit the existing request instead of creating a new one."_ — Hiện 2 nút: **Edit existing request** và **Back** |
| Đã tồn tại phiếu `Approved` trùng | **Cảnh báo + xác nhận** — Noti: _"An approved Attendance Adjustment request already exists for \[Teacher Name] – \[Timeoff Date] - \[Check-in Check-out], and the attendance has been updated accordingly. Do you want to continue?"_ — nút: **Yes / Cancel**. Sau khi ấn **Yes**: thực hiện Save tạo phiếu mới                                                                         |

</details>

## VIII. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Ngưỡng nghỉ giữa ca mặc định **T = 180 phút**; mỗi nhóm tối đa **2 ca liên tiếp**.
2. Ngưỡng cho phép đi muộn + về sớm để vẫn tính đủ công là **15 phút**.
3. Công thực tế tính theo **giây** và làm tròn **4 chữ số thập phân**.
4. Thời gian nghỉ giữa 2 ca trong nhóm gộp **không tính vào công**.
5. Approver Deadline mặc định là **3 ngày** sau ngày tạo Request.
6. Attendance Tracking chỉ được cập nhật khi phiếu **Approved**; Rejected giữ nguyên công.
7. Check trùng chỉ đối chiếu với phiếu **Pending** và **Approved**; bỏ qua Rejected/Cancelled.
8. Trùng phiếu **Pending** → chặn cứng; trùng phiếu **Approved** → cảnh báo và cho phép xác nhận tiếp tục.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Khi số công lệch so với kỳ vọng, đối chiếu check-in/check-out của buổi với các quy tắc ở trên để xác định nguyên nhân (đi muộn/về sớm vượt 15 phút, log ngoài khung ±1h30…).
{% endhint %}

## IX. Tài liệu liên quan

* [Quản lý chấm công giảng viên](/broken/pages/590d496c2faa37030c15c53ce299e0ba225f976b)
* [Tạo Timeoff Request (Attendance Adjustment)](/broken/pages/d6e80ca9f8cbe5ed9affbab15b21ce481ae567b7)
* [Chỉnh sửa & hủy Timeoff Request](/broken/pages/d64345dd1110656c968b798747f9b4a0b6a8ae0b)
