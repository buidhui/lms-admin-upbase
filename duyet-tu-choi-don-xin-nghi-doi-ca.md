# Duyệt / từ chối đơn xin nghỉ / đổi ca

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Facility Manager, Admin/Ops User, Receptionist Part-time

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Request

**Phạm vi & Module liên quan**

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Request / Approve & Reject Request
* **Module liên quan:** Receptionist Shift, Facility, Staff / Receptionist, Email Notification

**Điều kiện tiên quyết:**

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Receptionist Request** và quyền duyệt/từ chối đề xuất.
* Người dùng là **Facility Manager** của cơ sở diễn ra ca trực trong đề xuất.
* Đề xuất cần xử lý đang ở trạng thái **Pending**.

Trạng thái đề xuất: **Pending** (chờ duyệt), **Approved** (đã chấp thuận), **Rejected** (đã từ chối), **Cancelled** (đã duyệt trước đó nhưng sau đó bị hủy). Chỉ đề xuất **Pending** mới có thể duyệt/từ chối.

## II. Hướng dẫn chi tiết

### Xem chi tiết đề xuất cần duyệt/từ chối

{% stepper %}
{% step %}
## Truy cập màn hình Receptionist Request

Facility Manager truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu. Hệ thống hiển thị màn hình **Receptionist Request List**.
{% endstep %}

{% step %}
## Tìm đề xuất cần xử lý

Facility Manager tìm đề xuất cần xử lý tại màn hình **Receptionist Request List**. Có thể tìm kiếm theo Request Name, Request Type, Status hoặc khoảng thời gian tạo.
{% endstep %}

{% step %}
## Mở chi tiết đề xuất

Facility Manager nhấp vào **Request Name** hoặc chọn **Action → View** tại đề xuất cần xử lý. Hệ thống mở màn hình chi tiết đề xuất.
{% endstep %}

{% step %}
## Kiểm tra thông tin đề xuất

Facility Manager kiểm tra loại đề xuất, ca trực, cơ sở, người tạo, người thay thế, lý do và tài liệu đính kèm nếu có.
{% endstep %}
{% endstepper %}

### Duyệt đề xuất xin nghỉ / đổi ca

{% stepper %}
{% step %}
## Mở chi tiết đề xuất cần duyệt

Facility Manager mở màn hình chi tiết của đề xuất cần duyệt. Hệ thống hiển thị đầy đủ thông tin đề xuất.
{% endstep %}

{% step %}
## Chọn Approve

Facility Manager chọn **Approve** tại màn hình chi tiết đề xuất. Hệ thống cập nhật trạng thái đề xuất từ **Pending** sang **Approved**.
{% endstep %}

{% step %}
## Hệ thống gửi email thông báo

Hệ thống gửi email thông báo kết quả duyệt cho người tạo đề xuất. Đề xuất được ghi nhận là đã được chấp thuận.
{% endstep %}
{% endstepper %}

### Từ chối đề xuất xin nghỉ / đổi ca

{% stepper %}
{% step %}
## Mở chi tiết đề xuất cần từ chối

Facility Manager mở màn hình chi tiết của đề xuất cần từ chối. Hệ thống hiển thị đầy đủ thông tin đề xuất.
{% endstep %}

{% step %}
## Chọn Reject

Facility Manager chọn **Reject** tại màn hình chi tiết đề xuất. Hệ thống cập nhật trạng thái đề xuất từ **Pending** sang **Rejected**.
{% endstep %}

{% step %}
## Hệ thống gửi email thông báo

Hệ thống gửi email thông báo kết quả từ chối cho người tạo đề xuất. Đề xuất được ghi nhận là đã bị từ chối.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền duyệt/từ chối đề xuất để nhìn thấy/sử dụng nút **Approve** và **Reject**.
2. Chỉ **Facility Manager** của cơ sở diễn ra ca trực trong đề xuất mới được duyệt hoặc từ chối.
3. Chỉ đề xuất có trạng thái **Pending** mới có thể được duyệt hoặc từ chối; đề xuất Approved/Rejected/Cancelled không thể xử lý lại.
4. Nên kiểm tra kỹ thông tin ca trực, người thay thế và tài liệu đính kèm trước khi xử lý.
5. Sau khi duyệt/từ chối, hệ thống gửi email thông báo cho người tạo đề xuất.
6. Với đề xuất **Timeoff** được duyệt: hệ thống cập nhật lịch trực theo thông tin xin nghỉ và người thay thế nếu có.
7. Với đề xuất **Shift Change** được duyệt: hệ thống cập nhật việc đổi ca giữa người tạo đề xuất và người thay thế.
8. Với đề xuất bị từ chối: hệ thống chỉ cập nhật trạng thái và không thay đổi lịch trực.

### Quy tắc duyệt đề xuất Timeoff

| Trường hợp                            | Quy tắc xử lý                                                                     |
| ------------------------------------- | --------------------------------------------------------------------------------- |
| Đề xuất Timeoff có trạng thái Pending | Facility Manager có thể chọn **Approve** để duyệt.                                |
| Timeoff có người thay thế             | Hệ thống cập nhật người thay thế vào ca trực tương ứng.                           |
| Timeoff không có người thay thế       | Hệ thống ghi nhận người tạo đề xuất nghỉ ca; ca trực có thể còn thiếu người trực. |
| Sau khi duyệt                         | Trạng thái đề xuất chuyển từ **Pending** sang **Approved**.                       |
| Thông báo                             | Hệ thống gửi email thông báo kết quả duyệt cho người tạo đề xuất.                 |

### Quy tắc duyệt đề xuất Shift Change

| Trường hợp                                 | Quy tắc xử lý                                                     |
| ------------------------------------------ | ----------------------------------------------------------------- |
| Đề xuất Shift Change có trạng thái Pending | Facility Manager có thể chọn **Approve** để duyệt.                |
| Sau khi duyệt                              | Hệ thống đổi ca giữa người tạo đề xuất và người thay thế.         |
| Ca trực gốc                                | Người thay thế nhận ca trực gốc của người tạo đề xuất.            |
| Substitute Shift                           | Người tạo đề xuất nhận ca trực muốn chuyển sang.                  |
| Trạng thái đề xuất                         | Chuyển từ **Pending** sang **Approved**.                          |
| Thông báo                                  | Hệ thống gửi email thông báo kết quả duyệt cho người tạo đề xuất. |

### Quy tắc từ chối đề xuất

| Quy tắc           | Mô tả                                                               |
| ----------------- | ------------------------------------------------------------------- |
| Điều kiện từ chối | Đề xuất phải có trạng thái **Pending**.                             |
| Sau khi từ chối   | Trạng thái đề xuất chuyển từ **Pending** sang **Rejected**.         |
| Lịch trực         | Không thay đổi lịch trực hiện tại.                                  |
| Thông báo         | Hệ thống gửi email thông báo kết quả từ chối cho người tạo đề xuất. |

### Mẹo sử dụng

1. Nên lọc **Status = Pending** để xem nhanh các đề xuất đang chờ xử lý.
2. Trước khi duyệt **Timeoff**, nên kiểm tra xem đề xuất có người thay thế hay không để tránh thiếu Lễ tân trong ca.
3. Trước khi duyệt **Shift Change**, nên kiểm tra đúng ca trực gốc, ca muốn đổi và người đổi ca.
4. Nếu lý do hoặc tài liệu đính kèm chưa rõ ràng, nên liên hệ người tạo đề xuất trước khi duyệt.
5. Sau khi duyệt đề xuất, nên kiểm tra lại màn hình **Receptionist Shift** để đảm bảo lịch trực đã được cập nhật đúng.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                      | Nguyên nhân                                                                      | Cách xử lý                                               |
| ----------------------------------------------------- | -------------------------------------------------------------------------------- | -------------------------------------------------------- |
| Không thấy nút Approve/Reject                         | Tài khoản chưa có quyền duyệt/từ chối hoặc không phải Facility Manager của cơ sở | Kiểm tra phân quyền và cơ sở phụ trách                   |
| Không duyệt/từ chối được đề xuất                      | Đề xuất không còn ở trạng thái Pending                                           | Kiểm tra trạng thái hiện tại của đề xuất                 |
| Không thấy đề xuất cần duyệt                          | Đề xuất không thuộc cơ sở người dùng phụ trách hoặc bộ lọc quá hẹp               | Kiểm tra lại Facility, Status và điều kiện tìm kiếm      |
| Duyệt Timeoff nhưng ca vẫn thiếu người                | Đề xuất không có Substitute                                                      | Cần phân công bổ sung Lễ tân nếu ca trực còn thiếu người |
| Duyệt Shift Change nhưng lịch trực không đúng kỳ vọng | Chọn sai Substitute Shift hoặc Substitute trong đề xuất                          | Kiểm tra lại chi tiết đề xuất và lịch trực liên quan     |
| Người tạo không nhận được email                       | Dữ liệu email người tạo chưa đúng hoặc hệ thống gửi mail lỗi                     | Kiểm tra thông tin tài khoản và log gửi mail nếu cần     |
