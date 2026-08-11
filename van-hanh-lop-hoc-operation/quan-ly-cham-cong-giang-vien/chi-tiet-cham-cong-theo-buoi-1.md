# Chi tiết chấm công theo buổi (theo Giảng viên)

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description          | Version | Effective Date |
| -------------- | --------------- | ----- | --------------------------- | ------- | -------------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo nội dung hướng dẫn | 1.0.0   | Jun 24, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Operations → Customer Experience → Teacher → tab Attendance → click cột Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Teacher (Quản lý giảng viên)
* **Hệ thống tích hợp:** Zoom, Dahahi
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Đã đăng nhập thành công vào hệ thống OPS và có quyền xem chấm công.
* Đang ở tab Attendance của màn Teacher.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem chi tiết chấm công theo từng buổi của giảng viên</summary>

{% stepper %}
{% step %}
**Tại tab Attendance, click vào dữ liệu cột "Attendance" của giảng viên**

Hệ thống mở màn `[Tên giảng viên]'s Attendance` — chi tiết chấm công theo từng buổi học.

<figure><img src="../../.gitbook/assets/image (1421).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sử dụng bộ lọc để khoanh vùng dữ liệu**

* **Lesson:** chọn một hoặc nhiều buổi học.
* **Class:** danh sách các lớp giảng viên dạy trong tháng filter.
* **Construction Mode:** danh sách hình thức học.

<figure><img src="../../.gitbook/assets/image (1422).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Đọc thông tin chấm công theo từng buổi**

Danh sách hiển thị theo thứ tự ngày diễn ra buổi học từ mới nhất đến cũ nhất, kèm tên lớp tương ứng từng buổi.
{% endstep %}

{% step %}
**Xem lịch sử chấm công của một buổi**

Tại cột **Action**, click để hiển thị nút **Attendance History** → mở bảng lịch sử check-in (STT, Check-in, Check-out, Device).

<figure><img src="../../.gitbook/assets/image (1423).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1424).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Mô tả các trường thông tin trên màn [Tên giảng viên]'s Attendance</summary>

| **Name**                   | **Description**                                                                                           |
| -------------------------- | --------------------------------------------------------------------------------------------------------- |
| Lesson (Filter)            | Danh sách các buổi học. Có thể chọn nhiều                                                                 |
| Class (Filter)             | Danh sách các lớp học giảng viên dạy trong tháng filter                                                   |
| Construction Mode (Filter) | Danh sách hình thức học                                                                                   |
| Class                      | Tên lớp học                                                                                               |
| Lesson                     | Tên buổi học                                                                                              |
| Date                       | Ngày diễn ra buổi học, format dd/mm/yyyy start time – end time                                            |
| Check-in                   | Thời gian check-in. Format: ddmmyyyy hh:ss                                                                |
| Check-out                  | Thời gian check-out. Format: ddmmyyyy hh:ss                                                               |
| Attendance Tracking        | Công thực tế theo từng buổi. Buổi **chưa diễn ra** để trống; buổi **đã diễn ra** tính theo Business Rules |
| Device                     | Tên thiết bị: Zoom (buổi online) / Dahahi (buổi offline)                                                  |
| Reason                     | Lý do chỉnh sửa chấm công (nếu có)                                                                        |
| Action                     | Click để hiển thị nút Attendance History                                                                  |
| Attendance History         | Lịch sử check-in dạng bảng: STT, Check-in, Check-out, Device                                              |

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Một giảng viên có thể dạy nhiều lớp trong tháng — dùng filter **Class** để tách dữ liệu theo lớp.
2. Buổi học **chưa diễn ra** thì cột Attendance Tracking để trống.
3. Cách tính công thực tế theo từng buổi xem tại trang **Business Rules — Chấm công Giảng viên**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Lọc theo Construction Mode để phân biệt buổi Online (Zoom) và Offline (Dahahi).
2. Mở Attendance History khi cần kiểm tra chi tiết từng lần check-in/check-out.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                            | Nguyên nhân                                                | Hướng dẫn khắc phục                                        |
| ------------------------------------------- | ---------------------------------------------------------- | ---------------------------------------------------------- |
| Không hiển thị buổi học nào                 | Bộ lọc Lesson/Class/Construction Mode quá hẹp              | Kiểm tra lại điều kiện lọc, mở rộng phạm vi                |
| Thiếu lớp trong filter Class                | Giảng viên không có buổi dạy của lớp đó trong tháng filter | Đổi Date Filter ở màn Teacher để chọn đúng tháng           |
| Check-in/Check-out trống dù buổi đã diễn ra | Dữ liệu Zoom/Dahahi chưa đồng bộ hoặc lỗi mapping          | Liên hệ bộ phận phụ trách để đồng bộ lại dữ liệu chấm công |
