# Tạo Support Ticket

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Receptionist, Customer Experience, CX Admin, Owner, Follower

**Đường dẫn:** LMS → Support Ticket

#### Phạm vi & Module liên quan

* **Module chính:** Support Ticket
* **Chức năng chính:** Create Support Ticket
* **Module liên quan:** Facility, Receptionist, Customer Experience, Staff, Student/Contact, HubSpot Ticket

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Support Ticket** và quyền tạo Support Ticket.
* Tài khoản có title là **Receptionist**, **Customer Experience** hoặc **Customer Experience Admin**.
* Với ticket nhóm **Yêu cầu/Phản hồi học viên**: hệ thống cần có dữ liệu học viên/contact liên quan nếu muốn gắn contact trên HubSpot.
* Với trường **Owner**: người được chọn cần là Staff đã có tài khoản HubSpot nếu ticket cần đồng bộ HubSpot.

{% hint style="info" %}
Sau khi tạo thành công, ticket có trạng thái mặc định **Received**. Với ticket nhóm **Yêu cầu/Phản hồi học viên**, hệ thống tự động tạo ticket tương ứng trên **HubSpot**.
{% endhint %}

## II. Hướng dẫn chi tiết

### Tạo Support Ticket

{% stepper %}
{% step %}
## Truy cập màn hình Support Ticket List

Người dùng truy cập **LMS → Support Ticket** trên thanh menu. Hệ thống hiển thị màn hình **Support Ticket List**.
{% endstep %}

{% step %}
## Chọn +Create Support ticket

Người dùng chọn **+Create Support ticket** tại màn hình **Support Ticket List**. Hệ thống mở màn hình tạo mới Support Ticket.
{% endstep %}

{% step %}
## Nhập Name

Người dùng nhập **Name** (tên phiếu tiếp nhận yêu cầu, trường bắt buộc).
{% endstep %}

{% step %}
## Chọn Facility

Người dùng chọn **Facility**. Hệ thống hiển thị danh sách cơ sở theo quyền và title của người dùng.
{% endstep %}

{% step %}
## Chọn Time

Người dùng chọn **Time** (thời gian phát sinh vấn đề/yêu cầu hỗ trợ).
{% endstep %}

{% step %}
## Chọn Group và Type

Người dùng chọn **Group** (Cơ sở vật chất, Quy trình, Nội bộ hoặc Yêu cầu/Phản hồi học viên) và **Type** (hiển thị tương ứng với Group đã chọn).
{% endstep %}

{% step %}
## Nhập thông tin học viên (nếu Group = Yêu cầu/Phản hồi học viên)

Người dùng nhập thêm **BU**, **Class construction mode** và **Student** nếu Group = **Yêu cầu/Phản hồi học viên**. Các trường này phục vụ ghi nhận thông tin học viên và đồng bộ ticket lên HubSpot.
{% endstep %}

{% step %}
## Kiểm tra Priority

Người dùng kiểm tra **Priority** (hệ thống tự động điền dựa theo từng vấn đề/yêu cầu đã chọn).
{% endstep %}

{% step %}
## Upload Image (nếu cần)

Người dùng upload **Image** nếu cần đính kèm hình ảnh hoặc tài liệu thực tế. Hệ thống hỗ trợ tối đa 3 file/form, mỗi file tối đa 10MB.
{% endstep %}

{% step %}
## Nhập Description (nếu cần)

Người dùng nhập **Description** nếu cần mô tả thêm vấn đề (không bắt buộc).
{% endstep %}

{% step %}
## Chọn Owner và Follower

Người dùng chọn **Owner** (người phụ trách xử lý ticket) và **Follower** nếu cần thêm người theo dõi (Follower sẽ nhận email thông báo khi ticket được tạo mới).
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống kiểm tra dữ liệu bắt buộc, lưu ticket và hiển thị thông báo **Create successfully** nếu thông tin hợp lệ.
{% endstep %}
{% endstepper %}

### Hủy tạo mới Support Ticket

{% stepper %}
{% step %}
## Chọn Cancel

Người dùng chọn **Cancel** tại màn hình **Create Support Ticket**. Hệ thống hiển thị popup xác nhận hủy thao tác.
{% endstep %}

{% step %}
## Xác nhận hủy

Người dùng chọn xác nhận hủy tại popup. Hệ thống hủy thao tác tạo mới và quay lại màn hình **Support Ticket List**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có title là **Receptionist, Customer Experience** hoặc **Customer Experience Admin** để tạo Support Ticket.
2. Các trường bắt buộc cần được nhập đầy đủ trước khi lưu ticket.
3. Trạng thái mặc định của ticket mới tạo là **Received**.
4. Với Group = **Yêu cầu/Phản hồi học viên**: hiển thị thêm **BU, Class construction mode, Student**; trong đó **Student** là bắt buộc.
5. Với Group = **Yêu cầu/Phản hồi học viên**: hệ thống tự động tạo ticket trên HubSpot sau khi tạo ticket thành công trên LMS.
6. Nếu Email chính, Email phụ hoặc số điện thoại của Student không khớp contact nào trên HubSpot, ticket HubSpot vẫn được tạo nhưng không gắn được contact.
7. Khi chọn **Owner** cho ticket cần đồng bộ HubSpot, phải chọn Staff đã có tài khoản HubSpot.
8. Follower sẽ nhận email thông báo khi ticket được tạo mới.
9. Nút **Cancel** chỉ hủy thao tác tạo mới, không ảnh hưởng đến các ticket đã có.

### Quy tắc Facility

| Loại tài khoản            | Quy tắc hiển thị Facility                  |
| ------------------------- | ------------------------------------------ |
| Receptionist              | Chỉ hiển thị các cơ sở người đó phụ trách. |
| Customer Experience       | Hiển thị tất cả cơ sở.                     |
| Customer Experience Admin | Hiển thị tất cả cơ sở.                     |

### Quy tắc Group = Yêu cầu/Phản hồi học viên

| Trường thông tin        | Quy tắc                                                                                                 |
| ----------------------- | ------------------------------------------------------------------------------------------------------- |
| BU                      | Hiển thị và bắt buộc nhập/chọn.                                                                         |
| Class construction mode | Hiển thị và bắt buộc nhập/chọn.                                                                         |
| Student                 | Hiển thị và bắt buộc chọn.                                                                              |
| HubSpot Ticket          | Hệ thống tự động tạo ticket trên HubSpot sau khi ticket LMS được tạo thành công.                        |
| HubSpot Contact         | Nếu email/số điện thoại của Student khớp với contact trên HubSpot, contact được gắn với ticket HubSpot. |
| Owner                   | Staff được chọn làm Owner phải có tài khoản HubSpot.                                                    |

### Quy tắc file đính kèm

| Quy tắc                    | Mô tả                     |
| -------------------------- | ------------------------- |
| Số lượng file tối đa       | 03 file/form.             |
| Dung lượng tối đa mỗi file | 10MB/file.                |
| Tổng dung lượng tối đa     | 30MB/form.                |
| Định dạng hỗ trợ           | PDF, JPG, PNG, DOC, DOCX. |
| Bắt buộc upload            | Không bắt buộc.           |

### Quy tắc trạng thái sau khi tạo

| Thông tin             | Quy tắc                                                               |
| --------------------- | --------------------------------------------------------------------- |
| Status mặc định       | Received.                                                             |
| Message thành công    | Create successfully.                                                  |
| Follower notification | Follower nhận email thông báo khi ticket được tạo mới.                |
| HubSpot sync          | Chỉ tự động tạo ticket HubSpot với Group = Yêu cầu/Phản hồi học viên. |

### Mẹo sử dụng

1. Nên đặt tên ticket ngắn gọn nhưng đủ rõ, ví dụ: "Máy chiếu phòng NEU 301 không hoạt động" hoặc "Học viên phản hồi về lịch học".
2. Nên chọn đúng **Group** trước vì hệ thống sẽ hiển thị **Type** và các trường liên quan theo Group đã chọn.
3. Với vấn đề liên quan đến học viên, nên chọn đúng Student để hỗ trợ đồng bộ HubSpot chính xác.
4. Nên kiểm tra kỹ Owner, đặc biệt với ticket cần đồng bộ HubSpot.
5. Nếu có hình ảnh/tài liệu minh chứng, nên upload kèm để Owner dễ xử lý.
6. Nên thêm Follower nếu có người cần theo dõi tiến độ xử lý ticket.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                              | Nguyên nhân                                                                               | Cách xử lý                                                        |
| --------------------------------------------- | ----------------------------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Không thấy nút Create Support ticket          | Tài khoản chưa có quyền tạo ticket hoặc title không phù hợp                               | Kiểm tra phân quyền và title người dùng                           |
| Không lưu được ticket                         | Thiếu trường bắt buộc                                                                     | Kiểm tra và nhập đầy đủ các trường required                       |
| Không thấy Facility cần chọn                  | Tài khoản Receptionist chỉ hiển thị cơ sở được phân công                                  | Kiểm tra lại cơ sở phụ trách hoặc dùng tài khoản có quyền phù hợp |
| Không thấy BU/Class construction mode/Student | Group chưa phải Yêu cầu/Phản hồi học viên                                                 | Kiểm tra lại Group đã chọn                                        |
| Không tạo được ticket HubSpot                 | Owner chưa có tài khoản HubSpot hoặc dữ liệu đồng bộ không hợp lệ                         | Kiểm tra Owner và thông tin đồng bộ                               |
| Ticket HubSpot không gắn contact              | Email chính, email phụ hoặc số điện thoại của Student không khớp contact nào trên HubSpot | Kiểm tra thông tin Student/contact trên HubSpot                   |
| Upload file bị lỗi                            | File sai định dạng, vượt quá 10MB/file hoặc quá 3 file/form                               | Kiểm tra định dạng, dung lượng và số lượng file                   |
| Follower không nhận được email                | Chưa chọn Follower hoặc email người dùng không hợp lệ                                     | Kiểm tra lại danh sách Follower và thông tin email                |
