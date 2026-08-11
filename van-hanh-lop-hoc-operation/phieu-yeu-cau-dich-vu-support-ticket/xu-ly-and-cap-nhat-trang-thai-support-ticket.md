# Xử lý & cập nhật trạng thái Support Ticket

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description                                    | Version | Effective Date |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- | -------------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   | May 18, 2026   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   | Jun 18, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Owner, Customer Experience Admin, Follower, Receptionist/CX User

**Đường dẫn:** LMS → Support Ticket
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Support Ticket
* **Chức năng chính:** Edit Support Ticket / Update Ticket Status
* **Module liên quan:** Facility, Receptionist, Customer Experience, Staff, HubSpot Ticket
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Ticket đã được tạo thành công trên hệ thống.
* Người dùng là **Owner** của ticket hoặc có title = **Customer Experience Admin**.
* Ticket đang ở trạng thái cho phép chỉnh sửa.
* Người dùng có quyền truy cập và chỉnh sửa Support Ticket.
{% endhint %}

{% hint style="info" %}
Các trạng thái ticket: **Received** (chờ xử lý), **Processing** (đang xử lý), **Success** (thành công), **Failure** (thất bại).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Mở màn hình chỉnh sửa Support Ticket</summary>

{% stepper %}
{% step %}
## Truy cập màn hình Support Ticket List

Người dùng truy cập **LMS → Support Ticket** trên thanh menu. Hệ thống hiển thị màn hình **Support Ticket List**.
{% endstep %}

{% step %}
## Tìm ticket cần xử lý

Người dùng tìm ticket cần xử lý tại màn hình **Support Ticket List** (tìm kiếm/lọc theo Ticket name, Creator, Status, Priority, Facility, Group hoặc khoảng thời gian).
{% endstep %}

{% step %}
## Chọn Edit

Người dùng chọn **Edit** tại ticket cần xử lý. Hệ thống mở màn hình **Edit Support Ticket**. (Có thể nhấp vào **Name** để mở chi tiết, sau đó chọn **Edit** tại màn hình **Support Ticket Detail**.)
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cập nhật ticket từ Received sang Processing</summary>

{% stepper %}
{% step %}
## Mở ticket Received

Owner hoặc Customer Experience Admin mở màn hình **Edit Support Ticket** của ticket có trạng thái **Received**.
{% endstep %}

{% step %}
## Cập nhật thông tin (nếu cần)

Người dùng cập nhật các thông tin cần chỉnh sửa (Name, Owner, Facility, Priority, Image, Follower, Description).
{% endstep %}

{% step %}
## Chọn Status = Processing

Người dùng chọn **Status = Processing** tại màn hình **Edit Support Ticket**.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin, chuyển trạng thái ticket sang **Processing** và hiển thị thông báo **Updated successfully**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cập nhật ticket từ Processing sang Success</summary>

{% stepper %}
{% step %}
## Mở ticket Processing

Owner hoặc Customer Experience Admin mở màn hình **Edit Support Ticket** của ticket có trạng thái **Processing**.
{% endstep %}

{% step %}
## Chọn Status = Success

Người dùng chọn **Status = Success** tại màn hình **Edit Support Ticket**.
{% endstep %}

{% step %}
## Nhập Result và Evidence

Người dùng nhập **Result** và upload **Evidence** nếu hệ thống hiển thị hoặc yêu cầu thông tin kết quả xử lý.
{% endstep %}

{% step %}
## Cập nhật Follower/Description (nếu cần)

Người dùng cập nhật Follower hoặc Description nếu cần.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin, chuyển trạng thái ticket sang **Success** và ghi nhận thời gian đóng ticket.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cập nhật ticket từ Processing sang Failure</summary>

{% stepper %}
{% step %}
## Mở ticket Processing

Owner hoặc Customer Experience Admin mở màn hình **Edit Support Ticket** của ticket có trạng thái **Processing**.
{% endstep %}

{% step %}
## Chọn Status = Failure

Người dùng chọn **Status = Failure** tại màn hình **Edit Support Ticket**.
{% endstep %}

{% step %}
## Nhập Result và Evidence

Người dùng nhập **Result** và upload **Evidence** nếu hệ thống hiển thị hoặc yêu cầu thông tin kết quả xử lý.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin, chuyển trạng thái ticket sang **Failure** và ghi nhận thời gian đóng ticket.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chuyển ticket từ Success về Processing</summary>

{% stepper %}
{% step %}
## Mở ticket Success

Owner hoặc Customer Experience Admin mở màn hình **Edit Support Ticket** của ticket có trạng thái **Success**.
{% endstep %}

{% step %}
## Chọn Status = Processing

Người dùng chọn **Status = Processing** tại màn hình **Edit Support Ticket**.
{% endstep %}

{% step %}
## Cập nhật Follower/Description (nếu cần)

Người dùng cập nhật Follower hoặc Description nếu cần.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin và chuyển trạng thái ticket từ **Success** về **Processing**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cập nhật Owner/Follower của ticket</summary>

{% stepper %}
{% step %}
## Mở ticket cần cập nhật

Owner hoặc Customer Experience Admin mở màn hình **Edit Support Ticket** của ticket cần cập nhật.
{% endstep %}

{% step %}
## Chọn trường Owner/Follower

Người dùng chọn trường **Owner** hoặc **Follower**. Hệ thống mở danh sách Staff hợp lệ.
{% endstep %}

{% step %}
## Tìm kiếm Staff (nếu cần)

Người dùng tìm kiếm Staff theo **Name, Code, Title** hoặc **Department** nếu cần.
{% endstep %}

{% step %}
## Chọn Staff

Người dùng chọn Staff cần gán làm Owner hoặc Follower.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin và gửi email thông báo cho Owner mới hoặc Follower mới.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Hủy thao tác chỉnh sửa Support Ticket</summary>

{% stepper %}
{% step %}
## Chọn Cancel

Người dùng chọn **Cancel** tại màn hình **Edit Support Ticket**. Hệ thống hiển thị popup xác nhận hủy thao tác.
{% endstep %}

{% step %}
## Xác nhận hủy

Người dùng chọn xác nhận hủy tại popup. Hệ thống hủy thao tác chỉnh sửa và quay lại màn hình **Support Ticket List**.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ **Owner** của ticket hoặc người dùng có title = **Customer Experience Admin** mới được chỉnh sửa ticket.
2. Ticket ở trạng thái **Received** hoặc **Processing** có thể được chỉnh sửa nhiều thông tin xử lý.
3. Ticket ở trạng thái **Success** chỉ được chỉnh sửa một số thông tin giới hạn.
4. Ticket ở trạng thái **Failure** không thể chỉnh sửa thông tin.
5. Khi cập nhật Owner hoặc Follower, người mới được gán sẽ nhận email thông báo về ticket.
6. Khi ticket chuyển sang **Success** hoặc **Failure**, hệ thống ghi nhận **Closed date** và **Time to close**.
7. Với ticket cần đồng bộ HubSpot, cần đảm bảo Owner là Staff đã có tài khoản HubSpot.
8. Nếu chọn **Cancel**, các thay đổi chưa lưu sẽ không được ghi nhận.
{% endhint %}

### Quy tắc chuyển trạng thái ticket

| Trạng thái hiện tại | Trạng thái có thể chuyển | Quy tắc                                                                 |
| ------------------- | ------------------------ | ----------------------------------------------------------------------- |
| Received            | Processing               | Ticket bắt đầu được xử lý.                                              |
| Processing          | Success                  | Ticket được xử lý thành công.                                           |
| Processing          | Failure                  | Ticket xử lý thất bại hoặc không thể xử lý thành công.                  |
| Success             | Processing               | Mở lại ticket do kết quả xử lý chưa đạt yêu cầu hoặc cần xử lý bổ sung. |
| Failure             | Không cho phép chuyển    | Ticket ở trạng thái Failure không thể chỉnh sửa.                        |

### Quy tắc chỉnh sửa theo trạng thái

| Trạng thái ticket | Thông tin được chỉnh sửa                                              |
| ----------------- | --------------------------------------------------------------------- |
| Received          | Name, Owner, Facility, Priority, Image, Status, Follower, Description |
| Processing        | Name, Owner, Facility, Priority, Image, Status, Follower, Description |
| Success           | Name, Status, Follower, Description                                   |
| Failure           | Không được chỉnh sửa                                                  |

### Quy tắc Owner/Follower

| Quy tắc         | Mô tả                                                                       |
| --------------- | --------------------------------------------------------------------------- |
| Owner           | Người phụ trách xử lý ticket.                                               |
| Follower        | Người theo dõi tiến độ ticket.                                              |
| Danh sách Staff | Hiển thị danh sách Staff hợp lệ để chọn Owner/Follower.                     |
| Tìm kiếm Staff  | Có thể tìm kiếm theo Name, Code hoặc lọc theo Title, Department.            |
| Email thông báo | Owner mới và Follower mới nhận email khi ticket được cập nhật.              |
| HubSpot         | Với ticket cần đồng bộ HubSpot, Owner cần là Staff đã có tài khoản HubSpot. |

### Quy tắc SLA khi xử lý ticket

| Priority | Thời hạn xử lý |
| -------- | -------------- |
| Urgent   | 4 giờ          |
| High     | 8 giờ          |
| Medium   | 56 giờ         |
| Low      | 120 giờ        |

SLA Due Date = **Created Date + thời gian xử lý theo Priority**. Khi ticket chuyển sang **Success** hoặc **Failure**, hệ thống ghi nhận thời gian đóng ticket để tính **Time to close**.

{% hint style="info" %}
### Mẹo sử dụng

1. Khi bắt đầu xử lý ticket, nên chuyển trạng thái từ **Received** sang **Processing**.
2. Nếu ticket đã xử lý xong, nên cập nhật trạng thái **Success** và bổ sung kết quả xử lý rõ ràng.
3. Nếu ticket không thể xử lý thành công, nên cập nhật **Failure** và ghi rõ lý do/kết quả.
4. Trước khi đổi Owner, cần kiểm tra đúng người phụ trách và tài khoản HubSpot nếu ticket có đồng bộ HubSpot.
5. Nên thêm Follower nếu có người cần theo dõi tiến độ xử lý.
6. Không nên chuyển ticket sang Failure nếu vẫn còn khả năng xử lý tiếp, vì trạng thái Failure không cho phép chỉnh sửa sau đó.
7. Với ticket đã Success nhưng cần xử lý lại, có thể chuyển về **Processing**.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                              | Nguyên nhân                                                         | Cách xử lý                                        |
| ------------------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------- |
| Không thấy nút Edit                                           | Người dùng không phải Owner và không phải Customer Experience Admin | Kiểm tra quyền hoặc liên hệ người có quyền        |
| Không lưu được ticket                                         | Thiếu trường bắt buộc                                               | Kiểm tra các trường required trước khi Save       |
| Không chuyển được trạng thái                                  | Trạng thái hiện tại không cho phép chuyển sang trạng thái đã chọn   | Kiểm tra lại rule chuyển trạng thái               |
| Không chỉnh sửa được ticket Failure                           | Ticket ở trạng thái Failure không cho phép chỉnh sửa                | Không thao tác tiếp trên ticket Failure           |
| Không chỉnh sửa được Owner/Facility/Priority ở ticket Success | Ticket Success chỉ cho phép sửa một số trường giới hạn              | Chuyển về Processing nếu cần xử lý lại            |
| Owner mới không nhận email                                    | Email/tài khoản Staff không hợp lệ hoặc lỗi gửi mail                | Kiểm tra thông tin Staff và log gửi mail nếu cần  |
| Ticket HubSpot đồng bộ lỗi                                    | Owner chưa có tài khoản HubSpot hoặc dữ liệu không hợp lệ           | Kiểm tra Owner và thông tin đồng bộ HubSpot       |
| Time to close chưa hiển thị                                   | Ticket chưa chuyển sang Success hoặc Failure                        | Cập nhật trạng thái đóng ticket nếu đã xử lý xong |
