# Lịch sử check-in trong ngày

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Chuẩn hóa nội dung lên GitBook | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Màn chi tiết chuyên cần → cột Action → Attendance History
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class, Student
* **Hệ thống tích hợp:** Zoom
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

Đang ở giao diện chi tiết chuyên cần của học viên.
{% endhint %}

## II. Hướng dẫn chi tiết

{% stepper %}
{% step %}
### Tại bảng danh sách chuyên cần, cột Action → chọn "Attendance History"
{% endstep %}

{% step %}
### Đọc danh sách lịch sử check-in

Hệ thống hiển thị danh sách toàn bộ lịch sử check-in được ghi nhận trong ngày học đó, **sắp xếp từ sớm đến muộn**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="info" %}
### Mục đích

Dùng để tra cứu thời điểm cụ thể học viên check-in trong ngày, phục vụ đối chiếu khi trạng thái điểm danh chưa đúng kỳ vọng.
{% endhint %}

{% hint style="warning" %}
### Lưu ý quan trọng

1. Lịch sử thể hiện toàn bộ các lần vào – ra được ghi nhận trong ngày, kể cả khi học viên vào/ra nhiều lần hoặc dùng nhiều thiết bị.
2. Cách hệ thống hợp nhất các khoảng thời gian và tính thời lượng tham gia xem tại trang **Business Rules — Chuyên cần học viên qua Zoom**.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống       | Nguyên nhân                                            | Hướng dẫn khắc phục                                          |
| ---------------------- | ------------------------------------------------------ | ------------------------------------------------------------ |
| Lịch sử check-in trống | Dữ liệu Zoom chưa đồng bộ hoặc học viên không tham gia | Kiểm tra trạng thái đồng bộ; nếu cần, thực hiện điểm danh bù |
