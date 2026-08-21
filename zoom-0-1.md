# ZOOM 0\~1

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Chuẩn hóa nội dung lên GitBook | 1.0.0   |

## I. Thông tin chung

**Dành cho:** Admin CX

**Đường dẫn:** LMS Operation → Classes → chọn lớp → tab Student

#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class (Quản lý lớp học), Student
* **Hệ thống tích hợp:** Zoom

#### Điều kiện tiên quyết:

Đã đăng nhập và được cấp quyền truy cập module quản lý chuyên cần học viên trên hệ thống LMS Operation.

## II. Giới thiệu chung

Tài liệu hướng dẫn người dùng sử dụng chức năng quản lý chuyên cần học viên trên hệ thống LMS, bao gồm: tra cứu, lọc thông tin điểm danh, xem lịch sử check-in, điểm danh bù, chỉnh sửa điểm danh và hiểu logic đồng bộ/xử lý dữ liệu điểm danh từ Zoom về LMS.

* **Đối tượng:** các lớp học hình thức **Live Online** hoặc **Hybrid** qua Zoom.
* **Chức năng:** tự động đồng bộ điểm danh từ Zoom → LMS.
* **Người dùng:** Admin CX.

## III. Access Flow

{% stepper %}
{% step %}
## Truy cập hệ thống LMS Operation
{% endstep %}

{% step %}
## Chọn mục "Classes"
{% endstep %}

{% step %}
## Chọn lớp học mong muốn
{% endstep %}

{% step %}
## Chọn tab "Student"
{% endstep %}
{% endstepper %}

## IV. Danh sách chức năng

| STT | Chức năng                                     | Mô tả ngắn                                                                              |
| --- | --------------------------------------------- | --------------------------------------------------------------------------------------- |
| 1   | Xem thông tin chuyên cần học viên             | Xem cột Attendance dạng \[số buổi đã điểm danh / tổng số buổi] trong tab Student.       |
| 2   | Xem chi tiết chuyên cần theo buổi             | Mở giao diện chi tiết chuyên cần: bộ lọc và bảng danh sách các buổi học của học viên.   |
| 3   | Xem lịch sử check-in trong ngày               | Xem toàn bộ lịch sử check-in được ghi nhận trong một ngày học (Attendance History).     |
| 4   | Điểm danh bù (Add Attendance)                 | Bổ sung điểm danh cho học viên ở các buổi đủ điều kiện, kèm lý do.                      |
| 5   | Chỉnh sửa điểm danh (Edit Attendance)         | Chỉnh sửa trạng thái điểm danh cho trường hợp điểm danh bù (Absent → Present).          |
| 6   | Business Rules — Chuyên cần học viên qua Zoom | Quy tắc điểm danh (mapping buổi, thời lượng, ngưỡng 2/3) và quy tắc gửi email nhắc nhở. |

## V. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chỉ áp dụng cho lớp học hình thức **Live Online / Hybrid** qua Zoom.
2. Dữ liệu điểm danh được hệ thống **tự động đồng bộ** từ Zoom; người dùng chỉ chỉnh sửa trong các trường hợp được phép (điểm danh bù).
3. Logic xác định "có điểm danh / không điểm danh" mô tả tại trang **Business Rules — Chuyên cần học viên qua Zoom**.

### Mẹo sử dụng

1. Click trực tiếp vào số liệu chuyên cần để mở màn chi tiết theo từng buổi.
