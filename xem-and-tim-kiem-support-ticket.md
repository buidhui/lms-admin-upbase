# Xem & tìm kiếm Support Ticket

## Record of changes

_A - Add, M - Modify, D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Receptionist, Customer Experience, CX Admin

**Đường dẫn:** [https://ops.sapp.edu.vn/support-ticket?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/support-ticket?page_index=1\&page_size=10)

**Phạm vi & Module liên quan**

* **Module chính:** Support Ticket
* **Chức năng chính:** Support Ticket List / Support Ticket Detail
* **Module liên quan:** Facility, Receptionist, Customer Experience, HubSpot Ticket, Student/Contact

**Điều kiện tiên quyết:**

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập màn hình **Support Ticket**.
* Hệ thống đã có dữ liệu Support Ticket để hiển thị.
* Với một số ticket đồng bộ từ HubSpot, người dùng cần có quyền xem dữ liệu liên quan theo phân quyền hệ thống.

Trạng thái xử lý ticket: **Received** (mới tạo, mặc định), **Processing** (đang xử lý), **Success** (xử lý thành công), **Failure** (xử lý thất bại).

## II. Hướng dẫn chi tiết

### Xem danh sách Support Ticket

{% stepper %}
{% step %}
## Truy cập màn hình Support Ticket List

Người dùng truy cập **LMS → Support Ticket** trên thanh menu.

![](<.gitbook/assets/image (748)>)

Hệ thống hiển thị màn hình **Support Ticket List**.
{% endstep %}

{% step %}
## Xem danh sách ticket

Người dùng xem danh sách tại màn hình **Support Ticket List**. Hệ thống hiển thị: Name, Group, Facility, Time, Priority, Status, Owner, Created date và Updated date.
{% endstep %}
{% endstepper %}

### Tìm kiếm Support Ticket

{% stepper %}
{% step %}
## Nhập từ khóa tìm kiếm

Người dùng nhập từ khóa vào ô **Search** tại màn hình **Support Ticket List** (tìm theo **Ticket name** hoặc **Creator**).

![](<.gitbook/assets/image (749)>)
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách ticket thỏa mãn từ khóa tìm kiếm.
{% endstep %}
{% endstepper %}

### Lọc danh sách Support Ticket

{% stepper %}
{% step %}
## Chọn điều kiện lọc

Người dùng chọn điều kiện lọc tại màn hình **Support Ticket List** (**Status, Priority, Facility, Group, From date - To date**).

![](<.gitbook/assets/image (750)>)
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách ticket thỏa mãn điều kiện lọc.
{% endstep %}

{% step %}
## Chọn Reset (nếu cần)

Người dùng chọn **Reset** nếu muốn xóa toàn bộ điều kiện. Hệ thống hiển thị lại danh sách ticket theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết Support Ticket

{% stepper %}
{% step %}
## Mở Support Ticket Detail

Người dùng nhấp vào **Name** của ticket cần xem tại màn hình **Support Ticket List**.

![](<.gitbook/assets/image (751)>)

Hệ thống mở màn hình **Support Ticket Detail**.

![](<.gitbook/assets/image (752)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin chi tiết

Người dùng kiểm tra thông tin tại màn hình **Support Ticket Detail**: thông tin ticket, trạng thái xử lý, SLA, thông tin phân loại, người tạo, người xử lý và các thông tin kết quả nếu ticket đã được đóng.
{% endstep %}
{% endstepper %}

### Kiểm tra SLA của Support Ticket

{% stepper %}
{% step %}
## Mở Support Ticket Detail

Người dùng mở màn hình **Support Ticket Detail** của ticket cần kiểm tra.
{% endstep %}

{% step %}
## Xem thông tin SLA

Người dùng xem thông tin **Time to Close SLA Due Date** và **Time to Close SLA Status**. Hệ thống hiển thị thời hạn xử lý và trạng thái SLA tương ứng của ticket.

![](<.gitbook/assets/image (753)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền truy cập **Support Ticket** để xem danh sách và chi tiết ticket.
2. Có thể tìm kiếm ticket theo **Ticket name** hoặc **Creator**; lọc theo **Status, Priority, Facility, Group** và khoảng thời gian tạo.
3. Nút **Reset** chỉ xóa điều kiện tìm kiếm/lọc, không xóa dữ liệu ticket.
4. Trạng thái mặc định của ticket mới tạo là **Received**.
5. Các thông tin **BU** và **Class construction mode** chỉ hiển thị khi ticket thuộc Group = **Yêu cầu/Phản hồi học viên**.
6. Các thông tin **Result** và **Evidence** chỉ hiển thị khi ticket có Status = **Success** hoặc **Failure**.
7. **Closed date** và **Time to close** chỉ có dữ liệu khi ticket đã được đóng/xử lý xong.
8. Thời hạn xử lý ticket được tính theo **Created date + thời gian xử lý theo Priority**, chính xác đến giờ/phút/giây.

### Quy tắc trạng thái ticket

| Status     | Quy tắc                                                |
| ---------- | ------------------------------------------------------ |
| Received   | Ticket đã được tiếp nhận và đang chờ xử lý.            |
| Processing | Ticket đang được Owner xử lý.                          |
| Success    | Ticket đã được xử lý thành công.                       |
| Failure    | Ticket xử lý thất bại hoặc không thể xử lý thành công. |

### Quy tắc SLA theo Priority

| Priority | Thời hạn xử lý |
| -------- | -------------- |
| Urgent   | 4 giờ          |
| High     | 8 giờ          |
| Medium   | 56 giờ         |
| Low      | 120 giờ        |

### Quy tắc hiển thị thông tin chi tiết

| Điều kiện                                          | Thông tin hiển thị                                       |
| -------------------------------------------------- | -------------------------------------------------------- |
| Ticket thuộc Group = **Yêu cầu/Phản hồi học viên** | Hiển thị thêm **BU** và **Class construction mode**.     |
| Ticket có Status = **Success**                     | Hiển thị thêm **Result** và **Evidence** nếu có dữ liệu. |
| Ticket có Status = **Failure**                     | Hiển thị thêm **Result** và **Evidence** nếu có dữ liệu. |
| Ticket đã được đóng                                | Hiển thị **Closed date** và **Time to close**.           |

### Mẹo sử dụng

1. Cần kiểm tra nhanh các ticket chưa xử lý: lọc **Status = Received** hoặc **Processing**.
2. Cần xử lý ticket gấp: lọc theo **Priority = Urgent** hoặc **High**.
3. Cần xem ticket theo từng cơ sở: dùng bộ lọc **Facility**.
4. Cần kiểm tra ticket liên quan đến học viên: lọc theo **Group = Yêu cầu/Phản hồi học viên**.
5. Cần kiểm tra tiến độ xử lý: mở chi tiết ticket để xem **SLA Due Date** và **SLA Status**.
6. Khi tìm ticket cụ thể, nên tìm theo tên phiếu hoặc người tạo để ra kết quả nhanh hơn.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                      | Nguyên nhân                                                                    | Cách xử lý                                    |
| ------------------------------------- | ------------------------------------------------------------------------------ | --------------------------------------------- |
| Không thấy menu Support Ticket        | Tài khoản chưa có quyền truy cập chức năng                                     | Liên hệ Admin hệ thống để kiểm tra phân quyền |
| Danh sách không có dữ liệu            | Chưa có ticket hoặc bộ lọc đang quá hẹp                                        | Chọn **Reset** và tìm kiếm lại                |
| Không tìm thấy ticket cần xem         | Nhập sai từ khóa hoặc chọn sai điều kiện lọc                                   | Kiểm tra lại Ticket name, Creator và bộ lọc   |
| Không mở được chi tiết ticket         | Tài khoản không có quyền xem chi tiết hoặc ticket không thuộc phạm vi được xem | Kiểm tra lại phân quyền                       |
| Không thấy BU/Class construction mode | Ticket không thuộc Group = Yêu cầu/Phản hồi học viên                           | Đây là logic hiển thị bình thường             |
| Không thấy Result/Evidence            | Ticket chưa ở trạng thái Success hoặc Failure                                  | Kiểm tra lại Status của ticket                |
| Không thấy Closed date/Time to close  | Ticket chưa được đóng/xử lý xong                                               | Kiểm tra trạng thái xử lý của ticket          |
