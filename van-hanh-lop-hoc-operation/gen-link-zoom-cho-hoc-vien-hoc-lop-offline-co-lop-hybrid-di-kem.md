# Gen link zoom cho học viên học lớp Offline có lớp Hybrid đi kèm

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version | Effective Date |
| -------------- | ------------- | ----- | ------------------ | ------- | -------------- |
| Jul 20, 2026   | Lê Xuân Mai   | A     | Tạo mới user guide | 4.9.0   | July 20, 2026  |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** OPS → Class → Class List → Class Detail → Students → Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** OPS - Attendance
* **Chức năng chính:** Gen link Zoom / Cancel link Zoom theo buổi cho lớp Hybrid
* **Module liên quan:** LMS - Student Calendar, Email Service, Zoom Service, Attendance Service
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào **OPS** và có quyền **Gen link Zoom**.
* Lớp có **Construction Mode = Offline hoặc Blended** và **đã có lớp Hybrid liên kết** (field Hybrid Class ≠ rỗng).
* Lớp có **program = ACCA, Cert/Dip, CFA hoặc CMA**.
* Buổi học Hybrid tương ứng đã được gán link Zoom.
* Buổi học chưa kết thúc (đối với gen link) / chưa bắt đầu (đối với cancel link).
{% endhint %}

{% hint style="info" %}
**Bối cảnh:** Với lớp Hybrid, một số học viên đăng ký học Offline nhưng có buổi cần học Online qua Zoom. Chức năng này cho phép CX gen link Zoom **cá nhân hóa (encrypted)** cho từng buổi trực tiếp từ màn Attendance — không thay đổi schedule gốc, không lộ link Zoom gốc. Học viên truy cập Zoom qua LMS.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Gen link Zoom cho học viên (Admin CX)</summary>

{% stepper %}
{% step %}
**Truy cập màn Attendance của học viên**

Vào **OPS → Class → chọn lớp Offline/Blended → Class Detail → Students → Attendance**, tìm học viên và click vào tên học viên (hoặc dữ liệu tại cột Attendance).

<figure><img src="../.gitbook/assets/image (1438).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm buổi cần gen link Zoom**

Tìm buổi học cần gen link Zoom — buổi có **cột Zoom = ✗**.

<figure><img src="../.gitbook/assets/image (1439).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Action → Gen link Zoom**

Tại dòng buổi học, click **⋮ (Action)** → chọn **"Gen link Zoom"**. (Nút này chỉ hiển thị khi buổi chưa có link Zoom và lớp có Hybrid Class liên kết.)

<figure><img src="../.gitbook/assets/image (1440).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống kiểm tra điều kiện**

Hệ thống kiểm tra: Thời điểm hiện tại < End time buổi học (nếu buổi đã kết thúc → báo lỗi _"Buổi học đã kết thúc"_) và tìm được buổi Hybrid tương ứng.
{% endstep %}

{% step %}
**Xác nhận trên popup**

Hệ thống hiển thị popup **"Gen link Zoom"** với nội dung _"Gen link Zoom cho \[Tên HV] - \[Tên buổi học] - \[Ngày học HH:mm–HH:mm]?"_. Chọn **Confirm** để tiếp tục (chọn **Cancel** để hủy thao tác).

<figure><img src="../.gitbook/assets/image (1441).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống xử lý sau Confirm**

Hệ thống gen link Zoom encrypted, cập nhật cột **Zoom → ✓ (màu xanh)** và gửi email **"Thông báo lịch học Online Zoom"** cho học viên (chỉ gửi khi trạng thái lớp là **Public**). Trên LMS của học viên, buổi học hiển thị thêm button **"Tham gia Zoom"** kèm link encrypted.

<figure><img src="../.gitbook/assets/image (1442).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1443).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cancel link Zoom cho học viên (Admin CX)</summary>

{% stepper %}
{% step %}
**Tìm buổi đang có link Zoom**

Tại màn **Attendance**, tìm học viên và tìm buổi đang có **cột Zoom = ✓**.
{% endstep %}

{% step %}
**Chọn Action → Cancel link Zoom**

Tại dòng buổi học, click **⋮ (Action)** → chọn **"Cancel link Zoom"**. (Nút này chỉ hiển thị khi buổi đang có link Zoom = ✓.)

<figure><img src="../.gitbook/assets/image (1444).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống kiểm tra điều kiện**

Hệ thống kiểm tra: Thời điểm hiện tại < Start time buổi học. Nếu buổi đã diễn ra → báo lỗi _"Buổi học đã diễn ra"_ và không cho cancel.

<figure><img src="../.gitbook/assets/image (1445).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận trên popup**

Hệ thống hiển thị popup **"Cancel link Zoom"** với nội dung _"Hủy link Zoom cho \[Tên HV] - \[Tên buổi học] - \[Ngày học HH:mm–HH:mm]? Học viên sẽ không thể tham gia Zoom cho buổi này."_. Chọn **Confirm** để tiếp tục (chọn **Cancel** để hủy).

<figure><img src="../.gitbook/assets/image (1447).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống xử lý sau Confirm**

Hệ thống vô hiệu hóa link Zoom encrypted, cập nhật cột **Zoom → ✗ (màu xám)**, ẩn button **"Tham gia Zoom"** trên LMS của học viên. Buổi này **không được tính** vào bộ đếm 3/10/8 buổi.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Học viên tham gia Zoom trên LMS</summary>

{% stepper %}
{% step %}
**Đăng nhập LMS và mở Calendar**

Học viên đăng nhập LMS, truy cập mục **Calendar (Lịch học)** và chọn đúng buổi học cần tham gia.
{% endstep %}

{% step %}
**Nhấn Tham gia Zoom**

Mở thông tin buổi học và nhấn button **"Zoom"** (link encrypted cá nhân hóa) để tham gia lớp học qua Zoom. Link hiển thị bên dưới thông tin Offline (địa điểm, phòng học).
{% endstep %}

{% step %}
**Hệ thống ghi nhận điểm danh sau buổi học**

Sau khi buổi học kết thúc, qua webhook `meeting.end`, hệ thống lấy Zoom Participant Report để ghi nhận Check-in (thời điểm vào Zoom đầu tiên hợp lệ) và Check-out (thời điểm rời Zoom cuối cùng hợp lệ), tính điểm danh theo quy tắc bộ đếm (xem mục III). Để được ghi nhận chuyên cần, học viên cần tham gia tối thiểu **2/3 thời lượng** buổi học.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chức năng chỉ áp dụng cho lớp **Offline/Blended** có **Hybrid Class liên kết** và **program = ACCA, Cert/Dip, CFA, CMA**; buổi Hybrid tương ứng phải đã được gắn link Zoom.
2. CX chỉ gen/cancel link Zoom cho **từng buổi một** (không hỗ trợ gen hàng loạt), thao tác qua Action menu (⋮) tại từng dòng buổi học.
3. Chỉ gen link khi **thời điểm hiện tại < End time** buổi học; chỉ cancel link khi buổi học **chưa bắt đầu** (thời điểm hiện tại < Start time).
4. Thao tác gen/cancel **không thay đổi schedule** của học viên — học viên vẫn giữ nguyên trong buổi Offline gốc, chỉ gen thêm/vô hiệu hóa link Zoom gắn với buổi Hybrid tương ứng.
5. Toàn bộ dữ liệu điểm danh ghi về **lớp Offline gốc** — không tạo record tại lớp Hybrid.
6. Link Zoom là link encrypted (token gắn user\_id + class\_schedule\_id lớp Hybrid), không expose link gốc; cancel link → token bị vô hiệu hóa.
7. Nếu sau khi gen link học viên bị chuyển sang trạng thái không được học (Reserved, Retook, Moved\_out, Transferred\_To): link Zoom bị vô hiệu hóa tự động, điểm danh không được ghi nhận.
8. Nếu CX cancel link trước khi buổi học diễn ra → buổi đó không tính vào bộ đếm, điểm danh theo logic Offline bình thường.
9. Email **"Thông báo lịch học Online Zoom"** chỉ gửi cho học viên khi trạng thái lớp là **Public**.
{% endhint %}

### Điều kiện hợp lệ

| Điều kiện          | Chi tiết                                                                                                                                                                |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Lớp hợp lệ         | Construction Mode = **Offline hoặc Blended**, đã có **Hybrid Class** liên kết (≠ rỗng), program = **ACCA, Cert/Dip, CFA, CMA**; buổi Hybrid tương ứng đã gắn link Zoom. |
| Học viên hợp lệ    | Đang ở trạng thái **Normal, Reassigned, Retaking, Moved\_in, Be\_transferred** (Active hoặc Temporarily Absent) trong lớp.                                              |
| Buổi được gen link | Thời điểm hiện tại **< End time** buổi học (chính xác đến giờ, phút).                                                                                                   |
| Buổi được cancel   | Buổi học **chưa bắt đầu** (thời điểm hiện tại < Start time).                                                                                                            |

### Bộ đếm ghi nhận chuyên cần theo program

Bộ đếm chỉ tính các buổi có link Zoom **active tại thời điểm buổi học diễn ra**, sắp xếp theo thời gian gen link tăng dần.

| Program        | Số buổi được ghi nhận chuyên cần | Từ buổi vượt ngưỡng (Không được ghi nhận chuyên cần) |
| -------------- | -------------------------------- | ---------------------------------------------------- |
| ACCA, Cert/Dip | Buổi Zoom thứ **1, 2, 3**        | Buổi Zoom thứ **4 trở đi**                           |
| CFA            | Buổi Zoom thứ **1 → 10**         | Buổi Zoom thứ **11 trở đi**                          |
| CMA            | Buổi Zoom thứ **1 → 8**          | Buổi Zoom thứ **9 trở đi**                           |

* Buổi trong ngưỡng: tính điểm danh theo Zoom Participant Report — đủ **≥ 2/3 thời lượng** → **Present**, không đủ → **Absent**.
* Buổi vượt ngưỡng: vẫn có link Zoom, vẫn vào được lớp, vẫn ghi nhận Check-in/Check-out nếu tham gia, nhưng Status luôn = **Absent** và Reason = **"Đã quá buổi switch cho phép ghi nhận điểm danh"**.

### Nguồn ghi nhận điểm danh & logic Status

| Trường hợp                                    | Check-in / Check-out                         | Status                        | Reason                                           |
| --------------------------------------------- | -------------------------------------------- | ----------------------------- | ------------------------------------------------ |
| Buổi **Zoom ✗** (không có link Zoom)          | Theo logic Offline hiện tại                  | Present / Absent theo Offline | -                                                |
| Buổi **Zoom ✓**, trong ngưỡng, tham gia ≥ 2/3 | Từ Zoom Participant Report                   | **Present**                   | -                                                |
| Buổi **Zoom ✓**, trong ngưỡng, tham gia < 2/3 | Ghi nhận nếu có; để trống nếu không tham gia | **Absent**                    | -                                                |
| Buổi **Zoom ✓**, vượt ngưỡng (4+/11+/9+)      | Ghi nhận nếu có tham gia                     | **Absent**                    | "Đã quá buổi switch cho phép ghi nhận điểm danh" |

Quy tắc tính thời gian tham gia hợp lệ: chỉ tính trong khung \[start\_time, end\_time] của buổi học theo lịch LMS; gộp overlap nhiều thiết bị trước khi cộng tổng.

### Các cột màn Attendance (lớp có Hybrid Class liên kết)

| Cột        | Mô tả                                                                                                                     |
| ---------- | ------------------------------------------------------------------------------------------------------------------------- |
| Lesson     | Tên buổi học.                                                                                                             |
| Date       | Ngày học & thời gian Start–End.                                                                                           |
| **Mode**   | Mode buổi học: **Offline** hoặc **Live-online** (lấy từ construction mode cấp buổi).                                      |
| **Zoom**   | ✓ (xanh) nếu HV đang có link Zoom active; ✗ (xám) nếu không có link active/đã vô hiệu hóa. Lớp không có Hybrid: luôn `-`. |
| Check-in   | Thời điểm check-in (buổi Zoom ✓ lấy từ Zoom Participant Report).                                                          |
| Check-out  | Thời điểm check-out (buổi Zoom ✓ lấy từ Zoom Participant Report).                                                         |
| Status     | Present / Absent (theo BR5 & BR7).                                                                                        |
| Device     | Thiết bị ghi nhận.                                                                                                        |
| Reason     | Lý do; với buổi Zoom vượt ngưỡng: "Đã quá buổi switch cho phép ghi nhận điểm danh".                                       |
| Action (⋮) | Bổ sung **Gen link Zoom / Cancel link Zoom**.                                                                             |

### Điều kiện hiển thị Action menu

| Action               | Điều kiện hiển thị                                                              |
| -------------------- | ------------------------------------------------------------------------------- |
| Attendance History   | Giữ nguyên hiện tại.                                                            |
| Edit Attendance      | Giữ nguyên hiện tại.                                                            |
| **Gen Zoom link**    | Buổi Offline chưa gen link Zoom (cột Zoom = ✗) VÀ lớp có Hybrid Class liên kết. |
| **Cancel Zoom link** | Buổi đang có link Zoom (cột Zoom = ✓).                                          |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                       | Nguyên nhân                                                                    | Cách xử lý                                                       |
| ------------------------------------------------------ | ------------------------------------------------------------------------------ | ---------------------------------------------------------------- |
| "Buổi học đã kết thúc" (khi gen link)                  | Thời điểm hiện tại ≥ End time buổi học                                         | Chỉ gen link cho buổi chưa kết thúc                              |
| "Không tìm thấy buổi Hybrid tương ứng"                 | Không có buổi Hybrid trùng Start/End time với buổi Offline                     | Kiểm tra mapping buổi Hybrid (cùng Start/End time, UTC)          |
| "Buổi học đã diễn ra" (khi cancel link)                | Thời điểm hiện tại ≥ Start time buổi học                                       | Chỉ cancel link khi buổi học chưa bắt đầu                        |
| Không thấy nút Gen link Zoom                           | Buổi đã có link (Zoom = ✓) hoặc lớp không có Hybrid Class liên kết             | Gen chỉ hiển thị với buổi Zoom = ✗ và lớp có Hybrid Class        |
| Không thấy nút Cancel link Zoom                        | Buổi chưa có link Zoom (Zoom = ✗)                                              | Cancel chỉ hiển thị với buổi Zoom = ✓                            |
| Học viên không nhận được email                         | Trạng thái lớp không phải **Public**                                           | Email chỉ gửi khi lớp ở trạng thái Public                        |
| Học viên không tham gia Zoom được                      | Link đã bị cancel/vô hiệu hóa hoặc học viên đổi sang trạng thái không được học | Kiểm tra cột Zoom và trạng thái học viên trong lớp               |
| Buổi Zoom nhưng Status = Absent kèm Reason vượt ngưỡng | Buổi vượt bộ đếm 3/10/8 theo program                                           | Đây là quy tắc hệ thống; buổi vượt ngưỡng không ghi nhận Present |
| Điểm danh không được ghi nhận dù có link Zoom          | Học viên bị chuyển sang trạng thái không được học sau khi gen link             | Link tự vô hiệu hóa; kiểm tra lại trạng thái học viên            |
