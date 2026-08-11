# Quản lý điểm danh học viên

### 📘 Quản Lý Chuyên Cần Học Viên

***

## Record of changes

\*A - Add M - Modify D - Delete

| **Effective Date** | **Update Person** | **A,M,D** | **Change Description**                         | **Version** |
| ------------------ | ----------------- | --------- | ---------------------------------------------- | ----------- |
| 10 Jun 2025        | Huy Lê Xuân       | A         | Create New (UG Chuyên cần - Dahahi)            | 1.0.0       |
| 30 Jan 2026        | Nguyễn Duy Hiếu   | A         | Create New (UG Chuyên cần - Zoom)              | 1.0         |
| 01 Jun 2026        | …                 | M         | Gộp 2 UG (Dahahi & Zoom) theo template Gitbook | 2.0         |

***

## Definitions and Acronyms

<table data-header-hidden><thead><tr><th width="122"></th><th width="188"></th><th></th></tr></thead><tbody><tr><td><strong>#</strong></td><td><strong>Term</strong></td><td><strong>Definition</strong></td></tr><tr><td>1</td><td>Ops</td><td>Operations</td></tr><tr><td>2</td><td>LMS</td><td>Learning Management System</td></tr><tr><td>3</td><td>Dahahi</td><td>Hệ thống điểm danh bằng thiết bị phần cứng (offline check-in)</td></tr><tr><td>4</td><td>Zoom</td><td>Nền tảng học trực tuyến; dữ liệu vào/ra được đồng bộ về LMS</td></tr><tr><td>5</td><td>Admin CX</td><td>Người dùng quản trị vận hành lớp học</td></tr></tbody></table>

***

#### I. Giới Thiệu Chung

{% tabs %}
{% tab title="First Tab" %}
**1.1 Mục đích**

Tài liệu này hướng dẫn người dùng sử dụng chức năng **quản lý chuyên cần học viên** trên hệ thống **LMS**, bao gồm: tra cứu, lọc thông tin điểm danh, xem lịch sử check-in và hiểu rõ logic đồng bộ/xử lý dữ liệu điểm danh từ hai nguồn:

* **Dahahi** – thiết bị điểm danh phần cứng (áp dụng cho lớp Offline / Hybrid offline)
* **Zoom** – nền tảng học trực tuyến (áp dụng cho lớp Live Online / Hybrid online)

**1.2 Đối tượng áp dụng**

| Admin    | Quản trị hệ thống | Toàn quyền                             |
| -------- | ----------------- | -------------------------------------- |
| Admin CX | Vận hành lớp học  | Xem, điểm danh bù, chỉnh sửa điểm danh |

**1.3 Phạm vi & Module liên quan**

* **Module chính:** Chuyên cần Học viên (Student Attendance)
* **Module liên quan:** Classes, Student Management
* **Hệ thống tích hợp:** Dahahi (điểm danh phần cứng), Zoom (điểm danh online)

**1.4 Điều kiện tiên quyết**

* Đã có tài khoản và được cấp quyền truy cập LMS Operation
* Lớp học đã được tạo và có lịch học cố định trên LMS
{% endtab %}

{% tab title="Second Tab" %}

{% endtab %}
{% endtabs %}

<details>

<summary></summary>



</details>

**Mục đích**

Tài liệu này hướng dẫn người dùng sử dụng chức năng **quản lý chuyên cần học viên** trên hệ thống **LMS**, bao gồm: tra cứu, lọc thông tin điểm danh, xem lịch sử check-in và hiểu rõ logic đồng bộ/xử lý dữ liệu điểm danh từ hai nguồn:

* **Dahahi** – thiết bị điểm danh phần cứng (áp dụng cho lớp Offline / Hybrid offline)
* **Zoom** – nền tảng học trực tuyến (áp dụng cho lớp Live Online / Hybrid online)

**1.2 Đối tượng áp dụng**

| Admin    | Quản trị hệ thống | Toàn quyền                             |
| -------- | ----------------- | -------------------------------------- |
| Admin CX | Vận hành lớp học  | Xem, điểm danh bù, chỉnh sửa điểm danh |

**1.3 Phạm vi & Module liên quan**

* **Module chính:** Chuyên cần Học viên (Student Attendance)
* **Module liên quan:** Classes, Student Management
* **Hệ thống tích hợp:** Dahahi (điểm danh phần cứng), Zoom (điểm danh online)

**1.4 Điều kiện tiên quyết**

* Đã có tài khoản và được cấp quyền truy cập LMS Operation
* Lớp học đã được tạo và có lịch học cố định trên LMS

***

#### II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (935).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (937).png" alt=""><figcaption></figcaption></figure>

Mô tả ngắn các thành phần chính trên màn hình:

* **Cột Attendance:** Hiển thị tỉ lệ điểm danh dạng **\[Số buổi đã điểm danh / Tổng số buổi học]**. Ví dụ: 5/10 – học viên đã điểm danh 5 buổi trên tổng số 10 buổi.
* **Giao diện chi tiết chuyên cần:** Hiển thị khi click vào số liệu chuyên cần, gồm khu vực Filter và bảng danh sách buổi học.

***

#### III. Các Bước Thực Hiện Chi Tiết

**3.1 Access Flow**

🎯 _Mục tiêu: Truy cập vào màn hình quản lý chuyên cần học viên_

**Bước 1:** Truy cập hệ thống LMS Operation

**Bước 2:** Chọn mục **"Classes"**

**Bước 3:** Chọn lớp học mong muốn

**Bước 4:** Chọn tab **"Student"**

***

**3.2 Xem Thông Tin Attendance (Chuyên cần)**

🎯 _Mục tiêu: Tra cứu tỉ lệ điểm danh tổng quan của từng học viên_

**Bước 1:** Tại tab **Student**, cột **Attendance** hiển thị theo dạng:

**\[Số buổi đã điểm danh / Tổng số buổi học]**

Ví dụ: 5/10 – Học viên đã điểm danh 5 buổi trên tổng số 10 buổi học.

<figure><img src="../../.gitbook/assets/image (935).png" alt=""><figcaption></figcaption></figure>

***

**3.3 Hành Động Khi Click Vào Số Liệu Chuyên Cần**

🎯 _Mục tiêu: Xem chi tiết chuyên cần của từng học viên_

**Bước 1:** Click vào số liệu chuyên cần của học viên.

Hệ thống hiển thị giao diện chi tiết chuyên cần của học viên đó với 2 khu vực chính:

* **Filter:** Bộ lọc kết quả tìm kiếm
* **Danh sách:** Thông tin các buổi học của học viên trong lớp tương ứng

<figure><img src="../../.gitbook/assets/image (937).png" alt=""><figcaption></figcaption></figure>

***

**3.4 Giao Diện Chi Tiết Chuyên Cần**

**3.4.1 Thanh Bộ Lọc Tìm Kiếm**

* **Lesson:** Tìm kiếm theo tên buổi học (gõ ký tự gần đúng hoặc chính xác)
* **Status:** Dropdown list gồm:
  * Present – Có mặt
  * Absent – Vắng mặt
  * Người dùng có thể chọn nhiều nhất 1 giá trị.
* **From Date – To Date:** Lọc theo khoảng thời gian diễn ra buổi học. Người dùng lựa chọn theo ngày bắt đầu và ngày kết thúc được hiển thị trên giao diện hệ thống.

**3.4.2 Các Nút Chức Năng**

* **Nút Search:** Người dùng bấm Search để áp dụng bộ lọc và hiển thị kết quả.
* **Nút Reset:** Xóa bộ lọc, hiển thị lại toàn bộ dữ liệu.

***

**3.5 Bảng Danh Sách Chuyên Cần**

Bảng danh sách hiển thị các cột sau (cột hiển thị có thể khác nhau tùy theo nguồn điểm danh):

| **Lesson**    | Tên buổi học                                                     | ✓               | ✓    |
| ------------- | ---------------------------------------------------------------- | --------------- | ---- |
| **Date**      | Ngày diễn ra buổi học (Zoom: có cả thời gian bắt đầu – kết thúc) | ✓               | ✓    |
| **Check-in**  | Thời gian check-in hợp lệ sớm nhất (dd/mm/yyyy hh:mm)            | ✓               | ✓    |
| **Check-out** | Thời gian check-out muộn nhất (dd/mm/yyyy hh:mm)                 | –               | ✓    |
| **Status**    | Present / Absent / –                                             | ✓               | ✓    |
| **Device**    | Thiết bị ghi nhận check-in                                       | Thiết bị Dahahi | ZOOM |
| **Action**    | Nút thao tác                                                     | ✓               | ✓    |

**Action button** → Click chọn **Attendance History** để xem lịch sử check-in trong ngày.

***

**3.6 Lịch Sử Check-in Trong Ngày**

🎯 _Mục tiêu: Tra cứu thời điểm cụ thể học viên check-in trong ngày_

**Bước 1:** Tại bảng danh sách chuyên cần, click nút **Action** → chọn **"Attendance History"**.

Hệ thống hiển thị danh sách toàn bộ lịch sử check-in trong ngày học đó (sắp xếp từ sớm đến muộn).

**Mục đích:** Dùng để tra cứu thời điểm cụ thể học viên check-in trong ngày.

***

**3.7 Điểm Danh Bù&#x20;**_**(Chỉ áp dụng cho lớp Zoom)**_

🎯 _Mục tiêu: Thực hiện điểm danh bù cho học viên khi cần thiết_

Hệ thống cho phép vận hành thực hiện chỉnh sửa thông tin điểm danh của học viên qua chức năng **điểm danh bù**.

**Bước 1:** Tại màn hình Class Detail, người dùng bấm nút **Action** tại học viên cần thực hiện điểm danh bù → chọn **Add Attendance**.

**Bước 2:** Hệ thống hiển thị danh sách các buổi học viên có thể điểm danh bù.

**Bước 3:** Người dùng tích chọn vào các buổi cần thực hiện điểm danh bù → ấn **Add**.

**Bước 4:** Hệ thống hiển thị Pop-up nhập lý do điểm danh bù → người dùng nhập lý do → ấn **Save** để lưu.

***

**3.8 Chỉnh Sửa Điểm Danh&#x20;**_**(Chỉ áp dụng cho lớp Zoom)**_

🎯 _Mục tiêu: Chỉnh sửa lại thông tin điểm danh bù (Absent ⇒ Present)_

Hệ thống cho phép người dùng **chỉnh sửa** lại thông tin điểm danh **đối với các trường hợp điểm danh bù (từ Absent ⇒ Present)**.

**Bước 1:** Người dùng bấm nút **Action** tại buổi học cần chỉnh sửa → chọn **Edit Attendance**.

**Bước 2:** Hệ thống hiển thị Pop-up **Edit Attendance** → người dùng chọn lại trạng thái điểm danh và lý do thay đổi → ấn **Save** để lưu.

***

#### IV. Lưu Ý & Quy Tắc Nghiệp Vụ

**4.1 Rule Điểm Danh – Dahahi**

Áp dụng cho các lớp học sử dụng thiết bị điểm danh Dahahi (Offline / Hybrid offline).

**Trường hợp 1: Chỉ có 1 ca học trong ngày**

* Xác định **Present** nếu: Có dữ liệu check-in trong khoảng **0:00 – 23:59**. Hệ thống ghi nhận và hiển thị **thời gian check-in hợp lệ sớm nhất**.
* Xác định **Absent** (ghi nhận lúc 23:59 cùng ngày) nếu: **Không có dữ liệu check-in**.

**Trường hợp 2: Có nhiều hơn 1 ca học trong ngày**

* Tại Attendance History: hệ thống lưu trữ và hiển thị **tất cả lịch sử check-in** trong ngày.
* Xác định **Present** nếu: Có check-in trong khoảng **±1 giờ 30 phút** so với **start time** của từng ca học. Hệ thống ghi nhận và hiển thị thời điểm **hợp lệ sớm nhất**.
* Xác định **Absent** nếu: Không có check-in hợp lệ theo khoảng trên → Hệ thống cập nhật Status = **Absent** (ghi nhận lúc 23:59 cuối ngày buổi học tương ứng).

> ⚠️ **Ví dụ minh họa:**
>
> * Start time ca học: 9:00 → check-in hợp lệ từ 7:30 đến 10:30
> * Check-in lúc 11:00 → không hợp lệ → Cập nhật Status = Absent (vào 23:59 cuối ngày)

***

**4.2 Rule Điểm Danh – Zoom**

Áp dụng cho các lớp học có hình thức **Live Online** hoặc **Hybrid** qua Zoom.

**Logic mapping buổi học:**

Sau khi ghi nhận thời gian vào – ra của học viên, hệ thống xác định thời gian đó thuộc buổi học nào theo lịch học của học viên. Thời gian vào – ra link Zoom được tính là của buổi học A nếu đồng thời thỏa mãn 2 điều kiện:

* **Start time buổi A – 60 phút < Thời gian học viên vào học < End time buổi A**
* **Start time buổi A < Thời gian học viên rời buổi < End time buổi A + 60 phút**

> ⚠️ Ví dụ: Lịch học cố định buổi A từ 8:00 → 11:00, học viên vào link Zoom từ 7:30 → 11:30 → Hệ thống xác định khoảng 7:30 → 11:30 thuộc buổi A, sau đó tính tiếp thời lượng điểm danh.

**Các quy tắc tính thời lượng:**

* Thời lượng buổi học được tính theo **lịch cố định trên LMS**, không theo thời gian host mở lớp thực tế.
  * Ví dụ: Lịch học 8:00 → 11:00, host mở lớp Zoom thực tế 7:50 → 11:30 → Thời lượng vẫn tính theo 8:00 → 11:00.
* Hệ thống tính thời lượng học viên tham gia dựa trên **tổng thời gian có mặt trong khung giờ chính thức**, các thời gian ngoài khung sẽ tự động bị loại bỏ.
  * Ví dụ: Lịch học 8:00 → 11:00. Học viên tham gia 2 lần: lần 1 từ 7:45 → 9:00, lần 2 từ 9:10 → 11:15. Thời gian tính điểm danh: 8:00 → 9:00 và 9:10 → 11:00.
* Nếu lớp có **phòng chờ**, chỉ tính thời gian sau khi học viên được host thêm vào phòng chính.
* Khi học viên vào – ra nhiều lần hoặc dùng nhiều thiết bị cùng lúc, hệ thống tự động **hợp nhất thời gian và loại bỏ trùng lặp**.
  * Ví dụ: Thiết bị 1: 8:00 → 9:00. Thiết bị 2: 8:45 → 9:30. Do 8:45 → 9:00 bị trùng → Hệ thống chỉ tính 8:00 → 9:30.

**Kết quả điểm danh:**

* **Có điểm danh (Present):** nếu tham gia ≥ 2/3 thời lượng buổi học
* **Không điểm danh (Absent):** nếu tham gia < 2/3 thời lượng buổi học

***

**4.3 Rule Gửi Email Nhắc Nhở&#x20;**_**(Áp dụng cho cả Dahahi và Zoom)**_

> ⚠️ **Lưu ý quan trọng**
>
> * Nếu học viên **vắng mặt 2 buổi học liên tiếp trong cùng 1 lớp**, hệ thống sẽ gửi email nhắc nhở vào **8:00 sáng ngày liền sau**.
> * Nội dung email theo mẫu tại: [Google Sheet - Email Template](https://docs.google.com/spreadsheets/d/1rrs3Iug8tBOYZuRPczybSDJvEfuzQVkIdt_MfOuCsQY/edit?gid=1967552428#gid=1967552428)

***

#### V. Các Lỗi Thường Gặp Và Cách Xử Lý

| Lỗi / Tình huống                               | Nguyên nhân                                                                    | Cách xử lý                                                  |
| ---------------------------------------------- | ------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Không tìm thấy dữ liệu                         | Sai bộ lọc                                                                     | Kiểm tra lại điều kiện tìm kiếm, bấm Reset rồi thử lại      |
| Học viên có mặt nhưng hiển thị Absent (Dahahi) | Check-in ngoài khung thời gian hợp lệ (±1h30 so với start time)                | Kiểm tra Attendance History; liên hệ Ops nếu cần điều chỉnh |
| Học viên có mặt nhưng hiển thị Absent (Zoom)   | Thời gian tham gia < 2/3 thời lượng buổi học; hoặc ở phòng chờ chưa được admit | Kiểm tra Attendance History; thực hiện điểm danh bù nếu cần |
| Không thực hiện được điểm danh bù              | Không đủ quyền hoặc buổi học chưa đủ điều kiện                                 | Kiểm tra quyền Admin CX; liên hệ Admin hệ thống             |

***

#### VI. Câu Hỏi Thường Gặp

**Q: Dữ liệu điểm danh từ Dahahi và Zoom có đồng bộ về LMS theo thời gian thực không?**\
A: Dữ liệu được đồng bộ tự động; thời gian cập nhật phụ thuộc vào cấu hình hệ thống.

**Q: Chức năng điểm danh bù và chỉnh sửa điểm danh có áp dụng cho lớp Dahahi không?**\
A: Hiện tại chức năng này chỉ áp dụng cho lớp học qua Zoom.

**Q: Khi học viên dùng nhiều thiết bị Zoom cùng lúc, hệ thống tính thế nào?**\
A: Hệ thống tự động hợp nhất thời gian và loại bỏ khoảng thời gian trùng lặp giữa các thiết bị.

***

📩 _Mọi thắc mắc vui lòng liên hệ: \[kênh hỗ trợ Ops]_
