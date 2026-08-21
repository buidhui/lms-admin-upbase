# Chỉnh sửa điểm danh

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Chuẩn hóa nội dung lên GitBook | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Class Detail → cột Action tại buổi học → Edit Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Module liên quan:** Class, Student
* **Hệ thống tích hợp:** Zoom
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

Đã đăng nhập, có quyền chỉnh sửa chuyên cần. Chỉ áp dụng cho các trường hợp **điểm danh bù** (đổi Absent → Present).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Chỉnh sửa thông tin điểm danh</summary>

{% stepper %}
{% step %}
**Bấm nút Action tại buổi học cần chỉnh sửa → chọn "Edit Attendance"**
{% endstep %}

{% step %}
**Chọn lại trạng thái và nhập lý do**

Hệ thống hiển thị pop-up Edit Attendance. Người dùng chọn lại trạng thái điểm danh và nhập lý do thay đổi, sau đó ấn **Save** để lưu.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chức năng chỉnh sửa **chỉ áp dụng cho các trường hợp điểm danh bù** (Absent → Present).
2. Bắt buộc nhập lý do thay đổi để phục vụ tra soát.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống               | Nguyên nhân                                  | Hướng dẫn khắc phục                             |
| ------------------------------ | -------------------------------------------- | ----------------------------------------------- |
| Không hiển thị Edit Attendance | Buổi học không thuộc trường hợp điểm danh bù | Chỉ buổi đã điểm danh bù mới cho phép chỉnh sửa |
| Không lưu được thay đổi        | Chưa nhập lý do thay đổi                     | Nhập đầy đủ lý do trước khi ấn Save             |
