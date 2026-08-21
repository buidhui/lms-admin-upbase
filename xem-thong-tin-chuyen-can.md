# Xem thông tin chuyên cần

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
* **Module liên quan:** Class, Student
* **Hệ thống tích hợp:** Zoom

#### Điều kiện tiên quyết:

Đã đăng nhập và đang ở tab Student của lớp học cần xem.

## II. Hướng dẫn chi tiết

### Xem thông tin chuyên cần trong tab Student

{% stepper %}
{% step %}
## Tại tab "Student", xem cột "Attendance" của từng học viên

Thông tin hiển thị theo dạng: **\[Số buổi đã điểm danh / Tổng số buổi học]**.

Ví dụ: `0/18` — Học viên đã điểm danh 0 buổi trên tổng số 18 buổi học.

![](<.gitbook/assets/image (778)>)
{% endstep %}

{% step %}
## Click vào số liệu chuyên cần để xem chi tiết

Hệ thống mở giao diện chi tiết chuyên cần của học viên đó (gồm khu vực Filter và danh sách các buổi học). Xem hướng dẫn tại trang **Xem chi tiết chuyên cần theo buổi**.

![](<.gitbook/assets/image (779)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Số liệu `[đã điểm danh / tổng buổi]` chỉ tính trên các buổi học của lớp tương ứng.
2. Trạng thái điểm danh của từng buổi được xác định theo ngưỡng tham gia (xem Business Rules).

### Mẹo sử dụng

1. Click thẳng vào con số chuyên cần để mở nhanh màn chi tiết theo từng buổi.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                 | Nguyên nhân                                                           | Hướng dẫn khắc phục                                          |
| ------------------------------------------------ | --------------------------------------------------------------------- | ------------------------------------------------------------ |
| Số chuyên cần không tăng dù học viên đã tham gia | Thời gian tham gia chưa đạt ngưỡng 2/3 hoặc dữ liệu Zoom chưa đồng bộ | Mở màn chi tiết để kiểm tra check-in/out theo Business Rules |
| Không thấy cột Attendance                        | Tài khoản chưa được cấp quyền                                         | Liên hệ Admin để cấp quyền truy cập                          |
