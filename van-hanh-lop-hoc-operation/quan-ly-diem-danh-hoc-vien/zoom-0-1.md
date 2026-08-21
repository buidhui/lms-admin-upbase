# ZOOM 0\~1

## Record of changes

_A - Add M - Modify D - Delete_

<table data-first-column-sticky><thead><tr><th width="146">Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>Jun 24, 2026</td><td>Nguyễn Duy Hiếu</td><td>A</td><td>Chuẩn hóa nội dung lên GitBook</td><td>1.0.0</td><td>Jun 24, 2026</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** LMS Operation → Classes → chọn lớp → tab Student
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class (Quản lý lớp học), Student
* **Hệ thống tích hợp:** Zoom
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

Đã đăng nhập và được cấp quyền truy cập module quản lý chuyên cần học viên trên hệ thống LMS Operation.
{% endhint %}

## II. Giới thiệu chung

Tài liệu hướng dẫn người dùng sử dụng chức năng quản lý chuyên cần học viên trên hệ thống LMS, bao gồm: tra cứu, lọc thông tin điểm danh, xem lịch sử check-in, điểm danh bù, chỉnh sửa điểm danh và hiểu logic đồng bộ/xử lý dữ liệu điểm danh từ Zoom về LMS.

* **Đối tượng:** các lớp học hình thức **Live Online** hoặc **Hybrid** qua Zoom.
* **Chức năng:** tự động đồng bộ điểm danh từ Zoom → LMS.
* **Người dùng:** Admin CX.

## III. Access Flow

{% stepper %}
{% step %}
**Truy cập hệ thống LMS Operation**
{% endstep %}

{% step %}
**Chọn mục "Classes"**
{% endstep %}

{% step %}
**Chọn lớp học mong muốn**
{% endstep %}

{% step %}
**Chọn tab "Student"**
{% endstep %}
{% endstepper %}

## IV. Danh sách chức năng

<table><thead><tr><th width="75">STT</th><th>Chức năng</th><th>Mô tả ngắn</th></tr></thead><tbody><tr><td>1</td><td>Xem thông tin chuyên cần học viên</td><td>Xem cột Attendance dạng [số buổi đã điểm danh / tổng số buổi] trong tab Student.</td></tr><tr><td>2</td><td>Xem chi tiết chuyên cần theo buổi</td><td>Mở giao diện chi tiết chuyên cần: bộ lọc và bảng danh sách các buổi học của học viên.</td></tr><tr><td>3</td><td>Xem lịch sử check-in trong ngày</td><td>Xem toàn bộ lịch sử check-in được ghi nhận trong một ngày học (Attendance History).</td></tr><tr><td>4</td><td>Điểm danh bù (Add Attendance)</td><td>Bổ sung điểm danh cho học viên ở các buổi đủ điều kiện, kèm lý do.</td></tr><tr><td>5</td><td>Chỉnh sửa điểm danh (Edit Attendance)</td><td>Chỉnh sửa trạng thái điểm danh cho trường hợp điểm danh bù (Absent → Present).</td></tr><tr><td>6</td><td>Business Rules — Chuyên cần học viên qua Zoom</td><td>Quy tắc điểm danh (mapping buổi, thời lượng, ngưỡng 2/3) và quy tắc gửi email nhắc nhở.</td></tr></tbody></table>

## V. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ áp dụng cho lớp học hình thức **Live Online / Hybrid** qua Zoom.
2. Dữ liệu điểm danh được hệ thống **tự động đồng bộ** từ Zoom; người dùng chỉ chỉnh sửa trong các trường hợp được phép (điểm danh bù).
3. Logic xác định "có điểm danh / không điểm danh" mô tả tại trang **Business Rules — Chuyên cần học viên qua Zoom**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Click trực tiếp vào số liệu chuyên cần để mở màn chi tiết theo từng buổi.
{% endhint %}
