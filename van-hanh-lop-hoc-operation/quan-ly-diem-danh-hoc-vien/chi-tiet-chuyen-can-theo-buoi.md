# Chi tiết chuyên cần theo buổi

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Chuẩn hóa nội dung lên GitBook | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** tab Student → click số liệu chuyên cần của học viên
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class, Student
* **Hệ thống tích hợp:** Zoom
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

Đã mở giao diện chi tiết chuyên cần của học viên (từ việc click vào số liệu chuyên cần).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Lọc và tra cứu chi tiết chuyên cần</summary>

{% stepper %}
{% step %}
**Sử dụng thanh bộ lọc tìm kiếm**

* **Lesson:** tìm kiếm theo tên buổi học (gõ ký tự gần đúng hoặc chính xác).
* **Status:** dropdown gồm `Present` (Có mặt) / `Absent` (Vắng mặt) — chọn tối đa 1 giá trị.
* **From Date – To Date:** lọc theo khoảng thời gian diễn ra buổi học (chọn ngày bắt đầu và ngày kết thúc).
{% endstep %}

{% step %}
**Áp dụng hoặc xóa bộ lọc**

* **Search:** áp dụng bộ lọc và hiển thị kết quả.
* **Reset:** xóa bộ lọc, hiển thị lại toàn bộ dữ liệu.
{% endstep %}

{% step %}
**Đọc bảng danh sách chuyên cần**

Bảng hiển thị các buổi học của học viên với các cột: Lesson, Date, Check-in, Check-out, Status, Device, Action.
{% endstep %}

{% step %}
**Xem lịch sử check-in trong ngày**

Tại cột **Action**, click chọn **Attendance History** để xem lịch sử check-in trong ngày. Xem hướng dẫn tại trang **Xem lịch sử check-in trong ngày**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Mô tả các cột trên Bảng danh sách chuyên cần</summary>

| **Cột**   | **Mô tả**                                                          |
| --------- | ------------------------------------------------------------------ |
| Lesson    | Tên buổi học                                                       |
| Date      | Ngày diễn ra buổi học và thời gian bắt đầu – kết thúc của buổi học |
| Check-in  | Thời gian check-in sớm nhất (dd/mm/yyyy hh:mm)                     |
| Check-out | Thời gian check-out muộn nhất (dd/mm/yyyy hh:mm)                   |
| Status    | Present / Absent / -                                               |
| Device    | ZOOM                                                               |
| Action    | Action button → click chọn Attendance History                      |

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Status `-` thể hiện buổi học chưa có dữ liệu điểm danh (ví dụ buổi chưa diễn ra).
2. Check-in/Check-out hiển thị thời điểm sớm nhất / muộn nhất được ghi nhận trong ngày.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Kết hợp filter Lesson + Status + khoảng ngày để tìm nhanh buổi cần đối chiếu.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                              | Nguyên nhân                                  | Hướng dẫn khắc phục                                        |
| --------------------------------------------- | -------------------------------------------- | ---------------------------------------------------------- |
| Không tìm thấy buổi học                       | Sai bộ lọc Lesson/Status/khoảng ngày         | Kiểm tra lại điều kiện, bấm Reset                          |
| Status hiển thị Absent dù học viên có vào lớp | Thời gian tham gia < 2/3 thời lượng buổi học | Đối chiếu lịch sử check-in; nếu cần thực hiện điểm danh bù |
