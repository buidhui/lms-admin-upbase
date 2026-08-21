# Đồng bộ support ticket từ HubSpot về LMS

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

**Dành cho:** Customer Experience Admin, Owner, CX User, Admin/Ops User

**Đường dẫn:** LMS → Support Ticket (và HubSpot Ticket)

#### Phạm vi & Module liên quan

* **Module chính:** Support Ticket
* **Chức năng chính:** Sync from HubSpot
* **Module liên quan:** LMS Support Ticket, HubSpot Ticket, Student/Contact, Staff/Owner, HubSpot Integration

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Support Ticket**.
* Ticket đã tồn tại trên LMS và có liên kết với ticket tương ứng trên HubSpot.
* Người dùng có quyền xem hoặc chỉnh sửa ticket cần đồng bộ.
* Hệ thống tích hợp giữa LMS và HubSpot đang hoạt động.

Có 3 cách đồng bộ: nút **Sync from HubSpot** ở màn **Support Ticket Detail**, nút **Sync from HubSpot** ở màn **Edit Support Ticket**, hoặc chọn **Trạng thái đồng bộ = Đồng bộ lại** trên HubSpot Ticket.

## II. Hướng dẫn chi tiết

### Đồng bộ từ màn hình xem chi tiết LMS Ticket

{% stepper %}
{% step %}
## Truy cập màn hình Support Ticket List

Người dùng truy cập **LMS → Support Ticket** trên thanh menu. Hệ thống hiển thị màn hình **Support Ticket List**.
{% endstep %}

{% step %}
## Mở Support Ticket Detail

Người dùng nhấp vào **Name** của ticket cần đồng bộ. Hệ thống mở màn hình **Support Ticket Detail**.
{% endstep %}

{% step %}
## Chọn Sync from HubSpot

Người dùng chọn **Sync from HubSpot** tại màn hình **Support Ticket Detail**. Hệ thống thực hiện đồng bộ dữ liệu mới nhất từ HubSpot về LMS.
{% endstep %}

{% step %}
## Kiểm tra lại thông tin ticket

Người dùng kiểm tra lại thông tin ticket sau khi đồng bộ. Hệ thống hiển thị dữ liệu đã được cập nhật nếu quá trình đồng bộ thành công.
{% endstep %}
{% endstepper %}

### Đồng bộ từ màn hình chỉnh sửa LMS Ticket

{% stepper %}
{% step %}
## Truy cập màn hình Support Ticket List

Người dùng truy cập **LMS → Support Ticket** trên thanh menu. Hệ thống hiển thị màn hình **Support Ticket List**.
{% endstep %}

{% step %}
## Chọn Edit

Người dùng chọn **Edit** tại ticket cần đồng bộ. Hệ thống mở màn hình **Edit Support Ticket**.
{% endstep %}

{% step %}
## Chọn Sync from HubSpot

Người dùng chọn **Sync from HubSpot** tại màn hình **Edit Support Ticket**. Hệ thống thực hiện đồng bộ dữ liệu mới nhất từ HubSpot về LMS.
{% endstep %}

{% step %}
## Kiểm tra lại thông tin ticket

Người dùng kiểm tra lại thông tin ticket tại màn hình chỉnh sửa. Hệ thống hiển thị dữ liệu đã được cập nhật từ HubSpot nếu đồng bộ thành công.
{% endstep %}
{% endstepper %}

### Đồng bộ lại từ HubSpot Ticket

{% stepper %}
{% step %}
## Mở ticket trên HubSpot

Người dùng mở ticket tương ứng trên HubSpot. Hệ thống hiển thị thông tin HubSpot Ticket.
{% endstep %}

{% step %}
## Tìm property Trạng thái đồng bộ

Người dùng tìm property **Trạng thái đồng bộ** trên HubSpot Ticket.
{% endstep %}

{% step %}
## Chọn giá trị Đồng bộ lại

Người dùng chọn giá trị **Đồng bộ lại** tại property **Trạng thái đồng bộ**. Hệ thống ghi nhận yêu cầu đồng bộ lại.
{% endstep %}

{% step %}
## Quay lại LMS kiểm tra

Người dùng quay lại LMS để kiểm tra ticket tương ứng. Dữ liệu trên LMS được cập nhật sau khi quá trình đồng bộ hoàn tất.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chức năng **Sync from HubSpot** dùng khi cần đồng bộ thủ công dữ liệu từ HubSpot về LMS.
2. Ticket cần có liên kết với HubSpot Ticket thì mới có thể đồng bộ dữ liệu từ HubSpot về LMS.
3. Có thể đồng bộ từ màn hình xem chi tiết hoặc màn hình chỉnh sửa ticket trên LMS, hoặc kích hoạt bằng property **Trạng thái đồng bộ = Đồng bộ lại** trên HubSpot.
4. Với ticket thuộc Group = **Yêu cầu/Phản hồi học viên**, hệ thống có thể đồng bộ dữ liệu liên quan từ HubSpot về LMS.
5. Nếu dữ liệu Student/Contact trên HubSpot không khớp hoặc không tồn tại, một số thông tin liên quan đến contact có thể không được cập nhật đầy đủ.
6. Nếu Owner trên HubSpot không có tài khoản hợp lệ trên LMS hoặc không khớp dữ liệu Staff, hệ thống có thể không cập nhật được Owner tương ứng.
7. Nên kiểm tra lại ticket sau khi đồng bộ để xác nhận dữ liệu đã được cập nhật đúng.
8. Nếu đồng bộ thất bại nhiều lần, cần liên hệ Admin/IT để kiểm tra log đồng bộ và cấu hình tích hợp HubSpot.

### Các cách đồng bộ dữ liệu từ HubSpot về LMS

| Cách thực hiện | Vị trí thao tác                             | Mô tả                                                             |
| -------------- | ------------------------------------------- | ----------------------------------------------------------------- |
| Cách 1         | Màn hình **Support Ticket Detail** trên LMS | Chọn nút **Sync from HubSpot** khi đang xem chi tiết ticket.      |
| Cách 2         | Màn hình **Edit Support Ticket** trên LMS   | Chọn nút **Sync from HubSpot** khi đang chỉnh sửa ticket.         |
| Cách 3         | HubSpot Ticket                              | Chọn giá trị **Đồng bộ lại** tại property **Trạng thái đồng bộ**. |

### Quy tắc dữ liệu đồng bộ

| Nhóm thông tin       | Quy tắc                                                                                                          |
| -------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Thông tin ticket     | Dữ liệu trên LMS được cập nhật theo dữ liệu mới nhất từ HubSpot nếu đồng bộ thành công.                          |
| Status               | Trạng thái ticket có thể được cập nhật theo trạng thái tương ứng từ HubSpot nếu có mapping đồng bộ.              |
| Owner                | Owner chỉ cập nhật đúng nếu dữ liệu người xử lý trên HubSpot khớp với Staff hợp lệ trên LMS.                     |
| Student/Contact      | Contact chỉ được gắn/cập nhật nếu email hoặc số điện thoại khớp với dữ liệu trên HubSpot/LMS theo rule tích hợp. |
| File/ghi chú/kết quả | Các thông tin liên quan được cập nhật theo phạm vi đồng bộ đã cấu hình giữa HubSpot và LMS.                      |

### Quy tắc xử lý khi đồng bộ lỗi

| Tình huống                              | Quy tắc xử lý                                                                  |
| --------------------------------------- | ------------------------------------------------------------------------------ |
| Ticket LMS chưa liên kết HubSpot Ticket | Không thể đồng bộ từ HubSpot về LMS.                                           |
| Owner không khớp Staff LMS              | Hệ thống có thể không cập nhật được Owner tương ứng.                           |
| Contact không khớp                      | Ticket có thể đồng bộ nhưng không gắn được contact/học viên.                   |
| Hệ thống HubSpot hoặc LMS lỗi kết nối   | Đồng bộ có thể thất bại, cần thử lại sau hoặc liên hệ Admin/IT.                |
| Dữ liệu sau đồng bộ chưa đúng           | Người dùng cần kiểm tra lại ticket trên HubSpot, sau đó thực hiện đồng bộ lại. |

### Mẹo sử dụng

1. Nên dùng **Sync from HubSpot** khi thấy dữ liệu trên LMS chưa khớp với HubSpot.
2. Nếu đang kiểm tra ticket, nên đồng bộ từ màn hình **Support Ticket Detail**.
3. Nếu đang xử lý ticket, nên đồng bộ từ màn hình **Edit Support Ticket** trước khi tiếp tục cập nhật.
4. Nếu thao tác từ HubSpot, nên chọn **Trạng thái đồng bộ = Đồng bộ lại** rồi quay lại LMS kiểm tra kết quả.
5. Sau khi đồng bộ, nên kiểm tra các thông tin quan trọng như Status, Owner, Student/Contact, Result và Evidence.
6. Nếu đồng bộ không thành công, nên kiểm tra ticket có liên kết HubSpot hay chưa trước khi báo lỗi.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                       | Nguyên nhân                                                                                   | Cách xử lý                                                  |
| -------------------------------------- | --------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| Không thấy nút Sync from HubSpot       | Tài khoản chưa có quyền, ticket không thuộc phạm vi đồng bộ hoặc ticket chưa liên kết HubSpot | Kiểm tra quyền người dùng và liên kết HubSpot Ticket        |
| Bấm Sync nhưng dữ liệu không thay đổi  | HubSpot chưa có dữ liệu mới hoặc dữ liệu không nằm trong phạm vi đồng bộ                      | Kiểm tra lại dữ liệu trên HubSpot                           |
| Đồng bộ thất bại                       | Lỗi kết nối hoặc lỗi tích hợp giữa LMS và HubSpot                                             | Thử lại sau hoặc liên hệ Admin/IT kiểm tra log              |
| Owner không cập nhật đúng              | Owner trên HubSpot không khớp Staff hợp lệ trên LMS                                           | Kiểm tra tài khoản Staff và tài khoản HubSpot               |
| Student/Contact không được gắn         | Email hoặc số điện thoại không khớp contact trên HubSpot                                      | Kiểm tra dữ liệu contact/học viên                           |
| Dữ liệu LMS vẫn sai sau khi đồng bộ    | Dữ liệu nguồn trên HubSpot chưa đúng hoặc mapping đồng bộ chưa đúng                           | Kiểm tra HubSpot Ticket và báo Admin/IT nếu cần             |
| Không đồng bộ được từ HubSpot property | Property **Trạng thái đồng bộ** chưa được chọn đúng giá trị hoặc luồng tích hợp chưa chạy     | Chọn lại **Đồng bộ lại** và kiểm tra sau khi hệ thống xử lý |
