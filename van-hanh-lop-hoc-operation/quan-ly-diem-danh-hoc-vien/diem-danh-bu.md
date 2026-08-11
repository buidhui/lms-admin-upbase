# Điểm danh bù

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>Jun 24, 2026</td><td>Nguyễn Duy Hiếu</td><td>A</td><td>Chuẩn hóa nội dung lên GitBook</td><td>1.0.0</td><td>Jun 24, 2026</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Class Detail → cột Action của học viên → Add Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class, Student
* **Hệ thống tích hợp:** Zoom
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

Đã đăng nhập, có quyền chỉnh sửa chuyên cần và đang ở màn Class Detail.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Thực hiện điểm danh bù cho học viên</summary>

{% stepper %}
{% step %}
**Tại màn Class Detail, bấm nút Action ở học viên cần điểm danh bù → chọn "Add Attendance"**

_Chọn Add Attendance từ nút Action_
{% endstep %}

{% step %}
**Chọn các buổi cần điểm danh bù**

Hệ thống hiển thị danh sách các buổi học viên có thể điểm danh bù. Người dùng tích chọn các buổi cần thực hiện rồi ấn **Add**.

_Danh sách buổi có thể điểm danh bù_
{% endstep %}

{% step %}
**Nhập lý do và lưu**

Hệ thống hiển thị pop-up nhập lý do điểm danh bù. Người dùng nhập lý do và ấn **Save** để lưu.

_Pop-up nhập lý do điểm danh bù_
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ những buổi học đủ điều kiện mới xuất hiện trong danh sách điểm danh bù.
2. Lý do điểm danh bù là thông tin nên nhập rõ ràng để phục vụ tra soát về sau.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                  | Nguyên nhân                                              | Hướng dẫn khắc phục                                    |
| --------------------------------- | -------------------------------------------------------- | ------------------------------------------------------ |
| Không có buổi nào để điểm danh bù | Học viên đã được điểm danh đầy đủ hoặc buổi chưa diễn ra | Kiểm tra lại lịch học và trạng thái điểm danh hiện tại |
| Không lưu được lý do              | Bỏ trống trường lý do                                    | Nhập đầy đủ lý do trước khi ấn Save                    |
