# Bảng chấm công theo Giảng viên

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description          | Version |
| -------------- | --------------- | ----- | --------------------------- | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo nội dung hướng dẫn | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Operations → Customer Experience → Teacher → tab Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Teacher (Quản lý giảng viên), Operations – Customer Experience
* **Hệ thống tích hợp:** Zoom, Dahahi
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Đã đăng nhập thành công vào hệ thống OPS.
* Có quyền xem bảng chấm công giảng viên.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem bảng chấm công theo giảng viên</summary>

{% stepper %}
{% step %}
**Vào Department "Operations" → chọn "Customer Experience" → chọn "Teacher"**

<figure><img src="../../.gitbook/assets/image (1416).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn tab "Attendance"**

Hệ thống hiển thị bảng chấm công của các giảng viên theo tháng.

<figure><img src="../../.gitbook/assets/image (1417).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sử dụng bộ lọc để tìm giảng viên / khoảng thời gian mong muốn**

Có thể lọc theo mã/tên giảng viên, Gender, Class, Teaching Status, Program, Subject, Section, Person in Charge và Date Filter (mặc định là tháng hiện tại).

<figure><img src="../../.gitbook/assets/image (1418).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Đọc dữ liệu chấm công theo tháng**

Bảng hiển thị công thực tế / công chuẩn, số lần đi muộn–về sớm, số phút muộn và công theo từng ngày trong tháng.

<figure><img src="../../.gitbook/assets/image (1419).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào dữ liệu cột "Attendance" để xem chi tiết theo từng buổi**

Hệ thống mở màn `[Tên giảng viên]'s Attendance`. Xem hướng dẫn tại trang **Xem chi tiết chấm công theo từng buổi (theo giảng viên)**.

<figure><img src="../../.gitbook/assets/image (1420).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Mô tả các trường thông tin trên tab Attendance</summary>

| **Name**                           | **Description**                                                                                                                                                                                              |
| ---------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Search teacher code, name (Filter) | Tìm kiếm theo mã, tên giảng viên                                                                                                                                                                             |
| Gender (Filter)                    | Tìm kiếm theo giới tính                                                                                                                                                                                      |
| Class (Filter)                     | Tìm kiếm theo lớp giảng dạy                                                                                                                                                                                  |
| Teaching Status (Filter)           | Tìm kiếm theo tình trạng giảng dạy                                                                                                                                                                           |
| Program (Filter)                   | Tìm kiếm theo chương trình học                                                                                                                                                                               |
| Subject (Filter)                   | Tìm kiếm theo môn học                                                                                                                                                                                        |
| Section (Filter)                   | Tìm kiếm theo section trong môn học                                                                                                                                                                          |
| Person in Charge (Filter)          | Tìm kiếm theo người phụ trách                                                                                                                                                                                |
| Date Filter (Filter)               | Lọc theo tháng. Mặc định tháng hiện tại                                                                                                                                                                      |
| Code                               | Mã giảng viên                                                                                                                                                                                                |
| Teacher Name                       | Tên giảng viên                                                                                                                                                                                               |
| Attendance                         | Công giảng viên trong tháng. Format: **Thời gian chấm công thực tế / Công chuẩn**. Thực tế = tổng công thực tế các buổi đã dạy; Công chuẩn = tổng công chuẩn các buổi giảng viên dạy trong tháng theo filter |
| Late Count                         | Số lần đi muộn / về sớm trong tháng                                                                                                                                                                          |
| Late Minutes                       | Tổng số phút đi muộn / về sớm                                                                                                                                                                                |
| Thời gian chấm công                | Hiển thị theo cột tất cả các ngày trong tháng — số công thực tế theo từng ngày                                                                                                                               |

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Date Filter mặc định là **tháng hiện tại**; thay đổi để xem tháng khác.
2. Công chuẩn được tính theo các buổi giảng viên dạy **trong tháng theo filter đang chọn**.
3. Đi muộn = check-in muộn hơn giờ vào lớp; về sớm = check-out sớm hơn giờ kết thúc lớp.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Kết hợp các bộ lọc (Program, Subject, Person in Charge…) để khoanh vùng nhóm giảng viên cần theo dõi.
2. Click vào cột Attendance để mở chi tiết theo từng buổi và đối chiếu nguyên nhân lệch công.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống          | Nguyên nhân                                              | Hướng dẫn khắc phục                                         |
| ------------------------- | -------------------------------------------------------- | ----------------------------------------------------------- |
| Không tìm thấy giảng viên | Sai bộ lọc hoặc giảng viên không có buổi dạy trong tháng | Kiểm tra lại điều kiện tìm kiếm, đổi Date Filter, bấm Reset |
| Công thực tế = 0 cả tháng | Buổi học chưa diễn ra hoặc dữ liệu chưa đồng bộ          | Kiểm tra lịch dạy và trạng thái đồng bộ Zoom/Dahahi         |
| Late Count cao bất thường | Giảng viên check-in muộn / check-out sớm nhiều buổi      | Mở màn chi tiết để xác minh từng buổi theo Business Rules   |
