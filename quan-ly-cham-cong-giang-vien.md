# Quản lý chấm công giảng viên

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description                                         | Version |
| -------------- | --------------- | ----- | ---------------------------------------------------------- | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo tài liệu hướng dẫn chức năng Chấm công Giảng viên | 1.0.0   |

## I. Thông tin chung

**Dành cho:** Admin, Admin CX

**Đường dẫn:** https://ops.sapp.edu.vn/

#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Class (Quản lý lớp học), Teacher (Quản lý giảng viên), Operations – Customer Experience
* **Hệ thống tích hợp:** Zoom (lớp Online), Dahahi (lớp Offline)

#### Điều kiện tiên quyết:

Đã đăng nhập và được cấp quyền truy cập module Chấm công Giảng viên trên hệ thống OPS.

## II. Giới thiệu chung

Chức năng **Tự động chấm công Giảng viên** giúp hệ thống LMS/OPS **tự động ghi nhận và đồng bộ** dữ liệu chấm công của giảng viên cho cả hai hình thức giảng dạy Online và Offline, thay cho việc CX phải chấm công thủ công như trước đây.

Hệ thống tự động lấy log tham gia giảng dạy từ **Zoom** (lớp Online) và **Dahahi** (lớp Offline), xác định check-in/check-out hợp lệ theo từng buổi học và tính số công thực tế của giảng viên dựa trên thời gian dạy thực tế. Toàn bộ dữ liệu được quản lý tập trung trên một nền tảng duy nhất.

**Phạm vi áp dụng:** các lớp học hình thức **Offline / Hybrid / Blended / Live Online**.

## III. Danh sách chức năng

| STT | Chức năng                                               | Mô tả ngắn                                                                                                       |
| --- | ------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 1   | Xem chấm công giảng viên theo Lớp học                   | Xem cột Attendance (công thực tế / công chuẩn) của từng giảng viên trong một lớp tại Class Detail → tab Teacher. |
| 2   | Xem chi tiết chấm công theo từng buổi (trong lớp)       | Mở màn \[Tên GV]'s Attendance từ lớp để xem check-in/out, công thực tế và lịch sử chấm công theo từng buổi.      |
| 3   | Xem bảng chấm công theo Giảng viên                      | Xem tổng hợp chấm công theo tháng tại Operations → Customer Experience → Teacher → tab Attendance.               |
| 4   | Xem chi tiết chấm công theo từng buổi (theo giảng viên) | Mở màn \[Tên GV]'s Attendance từ tab Teacher để xem chi tiết theo từng buổi, lọc theo lớp và hình thức học.      |
| 5   | Business Rules — Chấm công Giảng viên                   | Quy tắc xác định ca dạy, gộp ca, mapping dữ liệu Zoom/Dahahi và cách tính công của giảng viên.                   |

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Dữ liệu chấm công được hệ thống ghi nhận **tự động**, CX không cần chấm công thủ công cho lớp Online, Offline.
2. Chỉ những buổi học **đã diễn ra** mới có dữ liệu công; buổi học chưa diễn ra để trống.
3. Chi tiết cách tính công, gộp ca và ngưỡng cho phép được mô tả tại trang **Business Rules — Chấm công Giảng viên**.

### Mẹo sử dụng

1. Dùng bộ lọc theo tháng/lớp/buổi học để khoanh vùng dữ liệu cần xem nhanh hơn.
2. Click trực tiếp vào dữ liệu cột Attendance để mở màn chi tiết theo từng buổi.
