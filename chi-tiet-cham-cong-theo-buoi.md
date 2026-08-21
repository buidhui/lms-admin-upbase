# Chi tiết chấm công theo buổi

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description          | Version |
| -------------- | --------------- | ----- | --------------------------- | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Khởi tạo nội dung hướng dẫn | 1.0.0   |

## I. Thông tin chung

**Dành cho:** Admin CX

**Đường dẫn:** Class → Class Detail → tab Teacher → click cột Attendance

#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance)
* **Module liên quan:** Class (Quản lý lớp học)
* **Hệ thống tích hợp:** Zoom, Dahahi

#### Điều kiện tiên quyết:

* Đã đăng nhập thành công vào hệ thống OPS và có quyền xem chi tiết chấm công.
* Đang ở màn Class Detail → tab Teacher của lớp cần xem.

## II. Hướng dẫn chi tiết

### Xem chi tiết chấm công theo từng buổi của giảng viên

{% stepper %}
{% step %}
## Tại tab Teacher, click vào dữ liệu cột "Attendance" của giảng viên

Hệ thống mở màn `[Tên giảng viên]'s Attendance` — chi tiết chấm công theo từng buổi học.

![](<.gitbook/assets/image (758)>)
{% endstep %}

{% step %}
## Sử dụng bộ lọc để tìm buổi học mong muốn

* **Lesson:** chọn một hoặc nhiều buổi học Zoom của lớp.
* **From Date – To Date:** tìm các buổi học có ngày nằm trong khoảng tìm kiếm.

![](<.gitbook/assets/image (759)>)
{% endstep %}

{% step %}
## Đọc thông tin chấm công theo từng buổi

Danh sách hiển thị theo thứ tự ngày diễn ra buổi học từ mới nhất đến cũ nhất.
{% endstep %}

{% step %}
## Xem lịch sử chấm công của một buổi

Tại cột **Action**, click để hiển thị nút **Attendance History** → mở bảng lịch sử check-in của giảng viên (STT, Check-in, Check-out, Device).

![](<.gitbook/assets/image (760)>)

![](<.gitbook/assets/image (761)>)
{% endstep %}
{% endstepper %}

### Mô tả các trường thông tin trên màn \[Tên giảng viên]'s Attendance

Nội dung hiển thị:

| Name                                                                                      | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ----------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _Filter_                                                                                  |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Lesson                                                                                    | Danh sách các buổi học Zoom của lớp. Có thể chọn nhiều                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| From Date - To Date                                                                       | Tìm kiếm buổi học có date nằm trong khoảng tìm kiếm.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| _Thông tin hiển thị (hiển thị theo thứ tự ngày diễn ra buổi học từ mới nhất đến cũ nhất)_ |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Lesson                                                                                    | Tên buổi học                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Date                                                                                      | Ngày diễn ra buổi học, format dd/mm/yyyy start time - end time                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| Check-in                                                                                  | <p>Thời gian check in<br><br>Format: ddmmyyyy hh:ss</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| Check-out                                                                                 | <p>Thời gian check out<br><br>Format: ddmmyyyy hh:ss</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| Attendance Tracking                                                                       | <p>Công thực tế theo từng buổi của giảng viên<br><br>- Trong TH buổi học <strong>chưa diễn ra</strong> thì để trống<br>- Trong TH buổi học <strong>đã diễn ra</strong> thì tính theo logic sau:<br>  - Công chuẩn của buổi học: mỗi buổi học 3 tiếng có công chuẩn = 3 (mỗi tiếng = 1 công)<br>  - Công được tính theo thời gian thực tế giảng viên giảng dạy:<br>    - Tổng thời gian đi muộn và về sớm trong mỗi buổi dạy ≤ 15 phút: được tính đủ công (=3).<br>    - Trường hợp tổng thời gian đi muộn và về sớm > 15 phút: thời gian làm việc được tính theo thời gian chấm công thực tế<br>    - Cách thức tính công thực tế của giảng viên: <strong>Công thực tế = Thời gian dạy thực tế/ Thời gian buổi học của 1 công (Đơn vị tính theo giây, làm tròn 4 số sau dấu phẩy)</strong><br>    - <em>VD: Buổi học diễn ra 8:00 - 11:00. Giảng viên dạy từ 8:20:24 - 11:20:00. Thời gian tính công: Từ 8:20:24 => 11:00. Thời gian dạy thực tế = 2 giờ 39 phút 36 giây => Công = 2 + 39/60 + 36/3600 = 2.66 công</em></p> |
| Device                                                                                    | <p>Tên thiết bị:<br><br>- Zoom: Với các buổi học online qua Zoom<br>- Dahahi: Với các buổi học offline</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| Reason                                                                                    | Lý do chỉnh sửa chấm công                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| Action                                                                                    | Click vào hiển thị button Attendance History                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| Attendance history                                                                        | <p>Hiển thị lịch sử check in của giảng viên theo dạng bảng, gồm các thông tin:<br><br>- STT<br>- Check-in<br>- Check-out<br>- Device</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Buổi học **chưa diễn ra** thì cột Attendance Tracking để trống.
2. Cột Device cho biết nguồn dữ liệu chấm công (Zoom cho buổi online, Dahahi cho buổi offline).
3. Cách tính công thực tế theo từng buổi xem tại trang **Business Rules — Chấm công Giảng viên**.

### Mẹo sử dụng

1. Dùng filter Lesson + khoảng ngày để xem nhanh các buổi cần đối chiếu.
2. Mở Attendance History khi cần kiểm tra chi tiết từng lần check-in/check-out của giảng viên.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                            | Nguyên nhân                                                  | Hướng dẫn khắc phục                                              |
| ------------------------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------------- |
| Không hiển thị buổi học nào                 | Bộ lọc Lesson/khoảng ngày quá hẹp hoặc sai                   | Kiểm tra lại điều kiện lọc, mở rộng khoảng ngày                  |
| Cột Attendance Tracking trống               | Buổi học chưa diễn ra                                        | Đây là trạng thái bình thường, công chỉ tính khi buổi đã diễn ra |
| Check-in/Check-out trống dù buổi đã diễn ra | Dữ liệu Zoom/Dahahi chưa đồng bộ hoặc lỗi mapping giảng viên | Liên hệ bộ phận phụ trách để đồng bộ lại dữ liệu chấm công       |
