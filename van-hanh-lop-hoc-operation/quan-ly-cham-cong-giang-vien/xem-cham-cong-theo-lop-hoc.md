# Xem chấm công theo Lớp học

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description          | Version | Effective Date |
| -------------- | --------------- | ----- | --------------------------- | ------- | -------------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo nội dung hướng dẫn | 1.0.0   | Jun 24, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Class → Class Detail → tab Teacher
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Class (Quản lý lớp học)
* **Hệ thống tích hợp:** Zoom, Dahahi
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Đã đăng nhập thành công vào hệ thống OPS.
* Có quyền xem chi tiết lịch sử chấm công của giảng viên.
* Áp dụng cho tất cả Construction Mode của Class.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem cột Attendance của giảng viên trong lớp</summary>

{% stepper %}
{% step %}
**Vào "Class"→ Class List → chọn lớp học cần xem để mở màn Class Detail**

<figure><img src="../../.gitbook/assets/image (1408).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tại màn Class Detail, chọn tab "Teacher"**

Hệ thống hiển thị danh sách giảng viên giảng dạy trong lớp.

<figure><img src="../../.gitbook/assets/image (1409).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem dữ liệu tại cột "Attendance"**

Cột Attendance hiển thị: **Số công ghi nhận thực tế / Số công chuẩn** của giảng viên trong lớp (chỉ tính các buổi mà giảng viên đó dạy trong lớp).

<figure><img src="../../.gitbook/assets/image (1410).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào dữ liệu cột "Attendance" để xem chi tiết theo từng buổi**

Hệ thống mở màn `[Tên giảng viên]'s Attendance`. Xem hướng dẫn chi tiết tại trang **Xem chi tiết chấm công theo từng buổi (trong lớp)**.

<figure><img src="../../.gitbook/assets/image (1411).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Số công tại cột Attendance chỉ tính trên **các buổi mà giảng viên đó dạy trong lớp**, không phải toàn bộ buổi của lớp.
2. Buổi học chưa diễn ra sẽ không được tính vào số công thực tế.
3. Cách tính số công chuẩn và công thực tế xem tại trang **Business Rules — Chấm công Giảng viên**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Click thẳng vào con số ở cột Attendance để xem nhanh chi tiết từng buổi mà không cần rời màn lớp.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                       | Nguyên nhân                                                         | Hướng dẫn khắc phục                                                                        |
| -------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Cột Attendance trống / chưa có số công | Buổi học chưa diễn ra hoặc dữ liệu chưa được đồng bộ từ Zoom/Dahahi | Kiểm tra lại lịch học; đợi hệ thống đồng bộ hoặc liên hệ bộ phận phụ trách đồng bộ dữ liệu |
| Số công không đúng kỳ vọng             | Giảng viên đi muộn/về sớm vượt ngưỡng cho phép                      | Mở màn chi tiết để xem check-in/out và đối chiếu theo Business Rules                       |
