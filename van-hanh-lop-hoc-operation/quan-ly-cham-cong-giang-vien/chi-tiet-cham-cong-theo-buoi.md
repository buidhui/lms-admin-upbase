# Chi tiết chấm công theo buổi (theo Lớp học)

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>Jun 24, 2026</td><td>Nguyễn Duy Hiếu</td><td>A</td><td>Khởi tạo nội dung hướng dẫn</td><td>1.0.0</td><td>Jun 24, 2026</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** Class → Class Detail → tab Teacher → click cột Attendance
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Class (Quản lý lớp học)
* **Hệ thống tích hợp:** Zoom, Dahahi
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Đã đăng nhập thành công vào hệ thống OPS và có quyền xem chi tiết chấm công.
* Đang ở màn Class Detail → tab Teacher của lớp cần xem.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem chi tiết chấm công theo từng buổi của giảng viên</summary>

{% stepper %}
{% step %}
**Tại tab Teacher, click vào dữ liệu cột "Attendance" của giảng viên**

Hệ thống mở màn `[Tên giảng viên]'s Attendance` — chi tiết chấm công theo từng buổi học.

<figure><img src="../../.gitbook/assets/image (1412).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sử dụng bộ lọc để tìm buổi học mong muốn**

* **Lesson:** chọn một hoặc nhiều buổi học Zoom của lớp.
* **From Date – To Date:** tìm các buổi học có ngày nằm trong khoảng tìm kiếm.

<figure><img src="../../.gitbook/assets/image (1413).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Đọc thông tin chấm công theo từng buổi**

Danh sách hiển thị theo thứ tự ngày diễn ra buổi học từ mới nhất đến cũ nhất.
{% endstep %}

{% step %}
**Xem lịch sử chấm công của một buổi**

Tại cột **Action**, click để hiển thị nút **Attendance History** → mở bảng lịch sử check-in của giảng viên (STT, Check-in, Check-out, Device).

<figure><img src="../../.gitbook/assets/image (1414).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (1415).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Mô tả các trường thông tin trên màn [Tên giảng viên]'s Attendance</summary>

Nội dung hiển thị:

<table data-header-hidden><thead><tr><th width="247"></th><th></th></tr></thead><tbody><tr><td><strong>Name</strong></td><td><strong>Description</strong></td></tr><tr><td><em>Filter</em></td><td></td></tr><tr><td>Lesson</td><td>Danh sách các buổi học Zoom của lớp. Có thể chọn nhiều</td></tr><tr><td>From Date - To Date</td><td>Tìm kiếm buổi học có date nằm trong khoảng tìm kiếm.</td></tr><tr><td><em>Thông tin hiển thị (hiển thị theo thứ tự ngày diễn ra buổi học từ mới nhất đến cũ nhất)</em></td><td></td></tr><tr><td>Lesson</td><td>Tên buổi học</td></tr><tr><td>Date</td><td>Ngày diễn ra buổi học, format dd/mm/yyyy start time - end time</td></tr><tr><td>Check-in</td><td><p>Thời gian check in</p><p>Format: ddmmyyyy hh:ss</p></td></tr><tr><td>Check-out</td><td><p>Thời gian check out</p><p>Format: ddmmyyyy hh:ss</p></td></tr><tr><td>Attendance Tracking</td><td><p>Công thực tế theo từng buổi của giảng viên</p><ul><li>Trong TH buổi học <strong>chưa diễn ra</strong> thì để trống</li><li><p>Trong TH buổi học <strong>đã diễn ra</strong> thì tính theo logic sau:</p><ul><li>Công chuẩn của buổi học: mỗi buổi học 3 tiếng có công chuẩn = 3 (mỗi tiếng = 1 công)</li><li><p>Công được tính theo thời gian thực tế giảng viên giảng dạy:</p><ul><li>Tổng thời gian đi muộn và về sớm trong mỗi buổi dạy ≤ 15 phút: được tính đủ công (=3).</li><li>Trường hợp tổng thời gian đi muộn và về sớm > 15 phút: thời gian làm việc được tính theo thời gian chấm công thực tế</li><li>Cách thức tính công thực tế của giảng viên: <strong>Công thực tế = Thời gian dạy thực tế/ Thời gian buổi học của 1 công (Đơn vị tính theo giây, làm tròn 4 số sau dấu phẩy)</strong></li><li><em>VD: Buổi học diễn ra 8:00 - 11:00. Giảng viên dạy từ 8:20:24 - 11:20:00. Thời gian tính công: Từ 8:20:24 => 11:00. Thời gian dạy thực tế = 2 giờ 39 phút 36 giây => Công = 2 + 39/60 + 36/3600 = 2.66 công</em></li></ul></li></ul></li></ul></td></tr><tr><td>Device</td><td><p>Tên thiết bị:</p><ul><li>Zoom: Với các buổi học online qua Zoom</li><li>Dahahi: Với các buổi học offline</li></ul></td></tr><tr><td>Reason</td><td>Lý do chỉnh sửa chấm công</td></tr><tr><td>Action</td><td>Click vào hiển thị button Attendance History</td></tr><tr><td>Attendance history</td><td><p>Hiển thị lịch sử check in của giảng viên theo dạng bảng, gồm các thông tin:</p><ul><li>STT</li><li>Check-in</li><li>Check-out</li><li>Device</li></ul></td></tr></tbody></table>

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Buổi học **chưa diễn ra** thì cột Attendance Tracking để trống.
2. Cột Device cho biết nguồn dữ liệu chấm công (Zoom cho buổi online, Dahahi cho buổi offline).
3. Cách tính công thực tế theo từng buổi xem tại trang **Business Rules — Chấm công Giảng viên**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Dùng filter Lesson + khoảng ngày để xem nhanh các buổi cần đối chiếu.
2. Mở Attendance History khi cần kiểm tra chi tiết từng lần check-in/check-out của giảng viên.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                            | Nguyên nhân                                                  | Hướng dẫn khắc phục                                              |
| ------------------------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------------- |
| Không hiển thị buổi học nào                 | Bộ lọc Lesson/khoảng ngày quá hẹp hoặc sai                   | Kiểm tra lại điều kiện lọc, mở rộng khoảng ngày                  |
| Cột Attendance Tracking trống               | Buổi học chưa diễn ra                                        | Đây là trạng thái bình thường, công chỉ tính khi buổi đã diễn ra |
| Check-in/Check-out trống dù buổi đã diễn ra | Dữ liệu Zoom/Dahahi chưa đồng bộ hoặc lỗi mapping giảng viên | Liên hệ bộ phận phụ trách để đồng bộ lại dữ liệu chấm công       |
