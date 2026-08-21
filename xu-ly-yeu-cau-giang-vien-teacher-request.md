# Xử lý yêu cầu giảng viên (Teacher Request)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

**Dành cho:** Admin, CX

**Đường dẫn:** Customer Experience → Teacher → List Request

#### Phạm vi & Module liên quan

* **Module chính:** Teacher Request Management
* **Chức năng chính:** Process Teacher Request
* **Module liên quan:** Teacher Calendar, Class Calendar, Classroom Schedule, Teacher Weekly Norm, Timeoff Request, LMS Notification

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **OPS/LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Customer Experience > Teacher** và quyền chỉnh sửa/xử lý trạng thái yêu cầu.
* Yêu cầu cần xử lý đã tồn tại trên hệ thống và đang ở trạng thái cho phép xử lý.

List Request gồm 2 tab: **Personal Schedule Request** (Busy Schedule, Weekly Norm) và **Timeoff Request** (Timeoff, Teaching Mode Change). Trạng thái: **Pending, Approved, Rejected, Cancelled**.

## II. Hướng dẫn chi tiết

### Duyệt yêu cầu giảng viên

{% stepper %}
{% step %}
## Truy cập màn hình danh sách yêu cầu

Người dùng chọn **Customer Experience > Teacher** trên hệ thống LMS Operations.

![](<.gitbook/assets/image (649)>)

Hệ thống hiển thị màn hình danh sách yêu cầu.
{% endstep %}

{% step %}
## Chọn tab chứa yêu cầu cần xử lý

Người dùng chọn **Personal Schedule Request** hoặc **Timeoff Request** tùy loại yêu cầu.

![](<.gitbook/assets/image (650)>)
{% endstep %}

{% step %}
## Chọn Action → Edit

Người dùng chọn **Action → Edit** tại dòng yêu cầu cần xử lý.

![](<.gitbook/assets/image (651)>)

Hệ thống mở màn hình chỉnh sửa yêu cầu.
{% endstep %}

{% step %}
## Chọn trạng thái Approved

Người dùng chọn trạng thái **Approved** tại màn hình chỉnh sửa yêu cầu.

![](<.gitbook/assets/image (652)>)
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống cập nhật yêu cầu sang trạng thái **Approved** và xử lý dữ liệu liên quan theo từng loại yêu cầu.
{% endstep %}
{% endstepper %}

### Từ chối yêu cầu giảng viên

{% stepper %}
{% step %}
## Mở List Request và chọn tab

Người dùng chọn **List Request** trên hệ thống OPS/LMS Operations, sau đó chọn tab chứa yêu cầu cần xử lý.
{% endstep %}

{% step %}
## Chọn Action → Edit

Người dùng chọn **Action → Edit** tại dòng yêu cầu cần từ chối. Hệ thống mở màn hình chỉnh sửa yêu cầu.
{% endstep %}

{% step %}
## Chọn trạng thái Rejected

Người dùng chọn trạng thái **Rejected** tại màn hình chỉnh sửa yêu cầu.

![](<.gitbook/assets/image (653)>)
{% endstep %}

{% step %}
## Nhập Note (nếu cần)

Người dùng nhập **Note** nếu cần ghi chú lý do từ chối.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống cập nhật yêu cầu sang trạng thái **Rejected** và gửi thông báo tới giảng viên.
{% endstep %}
{% endstepper %}

### Hủy yêu cầu đã duyệt

{% stepper %}
{% step %}
## Mở List Request và chọn tab

Người dùng chọn **List Request** trên hệ thống OPS/LMS Operations, sau đó chọn tab chứa yêu cầu cần hủy.
{% endstep %}

{% step %}
## Chọn Action → Edit (yêu cầu Approved)

Người dùng chọn **Action → Edit** tại dòng yêu cầu đang có trạng thái **Approved**. Hệ thống mở màn hình chỉnh sửa yêu cầu.

![](<.gitbook/assets/image (654)>)
{% endstep %}

{% step %}
## Chọn trạng thái Cancelled

Người dùng chọn trạng thái **Cancelled** tại màn hình chỉnh sửa yêu cầu.

![](<.gitbook/assets/image (655)>)
{% endstep %}

{% step %}
## Nhập Note (nếu cần)

Người dùng nhập **Note** nếu cần ghi chú lý do hủy.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống cập nhật yêu cầu sang trạng thái **Cancelled** và hoàn tác/cập nhật dữ liệu liên quan theo từng loại yêu cầu.
{% endstep %}
{% endstepper %}

### Xử lý yêu cầu từ màn hình chi tiết

{% stepper %}
{% step %}
## Mở Request Detail

Người dùng nhấp vào **Request name** tại màn hình **List Request**.

![](<.gitbook/assets/image (656)>)

Hệ thống mở màn hình **Request Detail**.
{% endstep %}

{% step %}
## Chọn Edit

Người dùng chọn **Edit** tại màn hình **Request Detail**.

![](<.gitbook/assets/image (657)>)

Hệ thống mở màn hình chỉnh sửa yêu cầu.
{% endstep %}

{% step %}
## Chọn trạng thái cần cập nhật

Người dùng chọn **Approved**, **Rejected** hoặc **Cancelled** tùy trạng thái hiện tại của yêu cầu.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống cập nhật trạng thái yêu cầu và xử lý dữ liệu liên quan.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền xử lý yêu cầu để thay đổi trạng thái Teacher Request.
2. Chỉ yêu cầu ở trạng thái **Pending** mới có thể chuyển sang **Approved** hoặc **Rejected**.
3. Chỉ yêu cầu ở trạng thái **Approved** mới có thể chuyển sang **Cancelled**.
4. Yêu cầu ở trạng thái **Rejected** hoặc **Cancelled** không tiếp tục được xử lý.
5. Khi trạng thái yêu cầu thay đổi, hệ thống gửi thông báo qua LMS tới giảng viên.
6. Với yêu cầu **Timeoff** và **Teaching Mode Change**, việc xử lý có thể ảnh hưởng đến lịch lớp học, lịch giảng viên và lịch phòng học.
7. Nên kiểm tra kỹ thông tin yêu cầu trước khi duyệt hoặc hủy để tránh ảnh hưởng đến lịch vận hành.
8. Chức năng này không bao gồm tạo mới hoặc xóa yêu cầu khỏi hệ thống.

### Quy tắc xử lý Personal Schedule Request (Busy Schedule, Weekly Norm)

| Trạng thái chuyển đổi | Quy tắc xử lý                                                          |
| --------------------- | ---------------------------------------------------------------------- |
| Pending → Approved    | Hệ thống chấp thuận yêu cầu và gửi thông báo qua LMS tới giảng viên.   |
| Pending → Rejected    | Hệ thống từ chối yêu cầu và gửi thông báo qua LMS tới giảng viên.      |
| Approved → Cancelled  | Hệ thống hủy yêu cầu đã duyệt và gửi thông báo qua LMS tới giảng viên. |

**Tác động theo loại yêu cầu:**

| Loại yêu cầu  | Khi Approved                                             | Khi Cancelled                                                               |
| ------------- | -------------------------------------------------------- | --------------------------------------------------------------------------- |
| Busy Schedule | Hệ thống ghi nhận lịch bận trên Calendar của giảng viên. | Hệ thống xóa các lịch bận đã tạo trước đó trên Calendar của giảng viên.     |
| Weekly Norm   | Hệ thống ghi nhận định mức tuần mới của giảng viên.      | Hệ thống khôi phục lại số lượng định mức trước khi đề xuất được chấp thuận. |

### Quy tắc xử lý Timeoff Request

| Trạng thái chuyển đổi | Quy tắc xử lý                                                                                       |
| --------------------- | --------------------------------------------------------------------------------------------------- |
| Pending → Approved    | Hệ thống chấp thuận yêu cầu, gửi thông báo tới giảng viên và cập nhật Calendar liên quan.           |
| Pending → Rejected    | Hệ thống từ chối yêu cầu, gửi thông báo tới giảng viên và không cập nhật lịch giảng viên/lớp học.   |
| Approved → Cancelled  | Hệ thống hủy yêu cầu đã duyệt và xử lý hoàn tác thông tin lịch theo tình trạng giảng viên thay thế. |

**Tác động khi duyệt Timeoff:** Cập nhật Calendar của giảng viên, lịch lớp học, lịch phòng học (nếu liên quan) và đồng bộ thay đổi sang LMS.

**Tác động khi hủy Timeoff đã duyệt:**

| Trường hợp                                                  | Quy tắc xử lý                                                                                                |
| ----------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Buổi học vẫn đang trống giảng viên                          | Hệ thống tạo lại event lịch học trên Calendar của giảng viên cũ và điền lại tên giảng viên vào lịch lớp học. |
| Buổi học đã được gắn giảng viên thay thế                    | Sau khi hủy yêu cầu, thông tin giảng viên tại buổi học đó không thay đổi.                                    |
| Tất cả buổi học trong yêu cầu đều đã có giảng viên thay thế | Hệ thống không cho phép hủy yêu cầu và hiển thị lỗi: _"Các buổi học đã có giảng viên thay thế"_.             |

### Quy tắc xử lý Teaching Mode Change

| Trạng thái chuyển đổi | Quy tắc xử lý                                                                                     |
| --------------------- | ------------------------------------------------------------------------------------------------- |
| Pending → Approved    | Hệ thống chấp thuận yêu cầu, gửi thông báo tới giảng viên và cập nhật Calendar liên quan.         |
| Pending → Rejected    | Hệ thống từ chối yêu cầu, gửi thông báo tới giảng viên và không cập nhật lịch giảng viên/lớp học. |
| Approved → Cancelled  | Hệ thống hủy yêu cầu đã duyệt và hoàn tác hình thức dạy nếu đủ điều kiện.                         |

**Tác động khi duyệt Teaching Mode Change:** Cập nhật hình thức dạy của buổi học, lịch lớp học, lịch giảng viên, lịch phòng học (nếu liên quan) và đồng bộ thay đổi sang LMS.

**Tác động khi hủy Teaching Mode Change đã duyệt:**

| Trường hợp                                                  | Quy tắc xử lý                                                                                                                |
| ----------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------- |
| Phòng học cũ còn trống tại thời điểm buổi học diễn ra       | Hệ thống cập nhật lại hình thức buổi học, thêm lại thông tin phòng học cũ và tạo lại bản ghi lịch phòng học.                 |
| Phòng học cũ đã có lịch khác tại thời điểm buổi học diễn ra | Hệ thống cập nhật lại hình thức buổi học nhưng để trống thông tin phòng học, đồng thời không tạo lại bản ghi lịch phòng học. |

### Quy tắc thông báo LMS

| Trạng thái chuyển đổi | Nội dung thông báo                                                         |
| --------------------- | -------------------------------------------------------------------------- |
| Pending → Approved    | Hệ thống gửi thông báo cho giảng viên rằng CX Admin đã chấp thuận yêu cầu. |
| Pending → Rejected    | Hệ thống gửi thông báo cho giảng viên rằng CX Admin đã từ chối yêu cầu.    |
| Approved → Cancelled  | Hệ thống gửi thông báo cho giảng viên rằng CX Admin đã hủy bỏ yêu cầu.     |

Thông báo cho phép giảng viên nhấp vào để chuyển tới màn hình xem chi tiết yêu cầu.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                 | Nguyên nhân                                                         | Cách xử lý                                                      |
| ------------------------------------------------ | ------------------------------------------------------------------- | --------------------------------------------------------------- |
| Không chuyển được sang Approved/Rejected         | Yêu cầu không ở trạng thái **Pending**                              | Chỉ xử lý duyệt/từ chối với yêu cầu đang Pending                |
| Không hủy được yêu cầu                           | Yêu cầu không ở trạng thái **Approved**                             | Chỉ hủy (Cancelled) được với yêu cầu đang Approved              |
| Lỗi "Các buổi học đã có giảng viên thay thế"     | Tất cả buổi học trong yêu cầu Timeoff đều đã có giảng viên thay thế | Không thể hủy yêu cầu trong trường hợp này                      |
| Hủy Teaching Mode Change nhưng mất phòng học     | Phòng học cũ đã có lịch khác tại thời điểm buổi học                 | Hệ thống để trống phòng học; cần gán lại phòng thủ công nếu cần |
| Không thực hiện được thao tác xử lý              | Tài khoản chưa có quyền xử lý yêu cầu                               | Liên hệ quản trị để được cấp quyền xử lý Teacher Request        |
| Yêu cầu Rejected/Cancelled không xử lý tiếp được | Đây là các trạng thái kết thúc của yêu cầu                          | Không thao tác thêm; tạo yêu cầu mới nếu cần                    |
