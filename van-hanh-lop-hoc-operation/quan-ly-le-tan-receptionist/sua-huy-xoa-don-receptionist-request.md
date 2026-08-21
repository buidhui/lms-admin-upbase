# Sửa / hủy / xóa đơn Receptionist Request

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Receptionist Part-time, Facility Manager, Substitute Receptionist

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Request
{% endhint %}

{% hint style="info" %}
**Phạm vi & Module liên quan**

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Request
* **Module liên quan:** Receptionist Shift, Facility, Staff / Receptionist, Email Notification
{% endhint %}

{% hint style="warning" %}
**Điều kiện tiên quyết:**

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Receptionist Request**.
* Người dùng là **người tạo đề xuất**.
* Với thao tác sửa: cần có quyền chỉnh sửa đề xuất. Với thao tác xóa: cần có quyền xóa đề xuất.
* Đề xuất cần thao tác phải đang ở trạng thái cho phép xử lý.
{% endhint %}

{% hint style="info" %}
Theo trạng thái: **Pending** (có thể sửa hoặc xóa), **Approved** (có thể hủy bằng cách chuyển sang Cancelled), **Rejected**/**Cancelled** (không sửa/hủy/xóa).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Chỉnh sửa đề xuất đang chờ duyệt (Pending)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Request**

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu.

<figure><img src="../../.gitbook/assets/image (1331).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình danh sách đề xuất.
{% endstep %}

{% step %}
**Tìm đề xuất cần chỉnh sửa**

Lễ tân Part-time tìm đề xuất cần chỉnh sửa tại màn hình **Receptionist Request** (tìm theo Request Name, Request Type, Status hoặc khoảng thời gian tạo).
{% endstep %}

{% step %}
**Chọn Action → Edit**

Lễ tân Part-time chọn **Action → Edit** tại đề xuất cần chỉnh sửa. Hệ thống mở màn hình chỉnh sửa đề xuất.
{% endstep %}

{% step %}
**Cập nhật thông tin đề xuất**

Với đề xuất **Timeoff**: chỉnh sửa Request Name, Shift, Substitute, Reason, Attached Document và thêm/xóa ca xin nghỉ nếu cần. Với đề xuất **Shift Change**: chỉnh sửa Request Name, Shift, Substitute Shift, Substitute, Reason và Attached Document.
{% endstep %}

{% step %}
**Chọn Save**

Lễ tân Part-time chọn **Save**. Hệ thống lưu thông tin mới của đề xuất và giữ trạng thái là **Pending**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Hủy đề xuất đã được duyệt (Approved → Cancelled)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Request**

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu. Hệ thống hiển thị danh sách đề xuất.
{% endstep %}

{% step %}
**Chọn Action → Edit (đề xuất Approved)**

Lễ tân Part-time chọn **Action → Edit** tại đề xuất có trạng thái **Approved**. Hệ thống mở màn hình chỉnh sửa đề xuất.
{% endstep %}

{% step %}
**Chuyển trạng thái sang Cancelled**

Lễ tân Part-time chuyển trạng thái đề xuất từ **Approved** sang **Cancelled** tại màn hình chỉnh sửa.
{% endstep %}

{% step %}
**Chọn Save**

Lễ tân Part-time chọn **Save**. Hệ thống hiển thị popup xác nhận hủy đề xuất.
{% endstep %}

{% step %}
**Xác nhận hủy**

Lễ tân Part-time chọn **Yes** tại popup xác nhận. Hệ thống cập nhật trạng thái đề xuất từ **Approved** sang **Cancelled** và xử lý lại thông tin lịch trực theo loại đề xuất.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa đề xuất đang chờ duyệt (Pending)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Request**

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu. Hệ thống hiển thị màn hình danh sách đề xuất.
{% endstep %}

{% step %}
**Chọn Action → Delete**

Lễ tân Part-time chọn **Action → Delete** tại đề xuất cần xóa. Chỉ đề xuất có trạng thái **Pending** mới được phép xóa.
{% endstep %}

{% step %}
**Xác nhận xóa**

Lễ tân Part-time chọn **Yes** tại popup xác nhận xóa. Hệ thống xóa đề xuất khỏi danh sách và gửi email thông báo cho người duyệt đề xuất.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
**Lưu ý quan trọng**

1. Người dùng chỉ được sửa, hủy hoặc xóa đề xuất do chính mình tạo.
2. Đề xuất **Pending** có thể được chỉnh sửa hoặc xóa.
3. Đề xuất **Approved** chỉ có thể được hủy bằng cách chuyển trạng thái sang **Cancelled**.
4. Đề xuất **Rejected** hoặc **Cancelled** không được chỉnh sửa, hủy hoặc xóa.
5. Sau khi xóa đề xuất thành công, hệ thống gửi email thông báo cho người duyệt.
6. Sau khi hủy đề xuất đã duyệt, hệ thống cập nhật lại thông tin lịch trực theo loại đề xuất.
7. Cần kiểm tra kỹ trước khi chọn **Yes** tại popup xác nhận vì thao tác xóa/hủy có thể ảnh hưởng đến lịch trực.
{% endhint %}

### Quy tắc chỉnh sửa đề xuất Pending

| Loại đề xuất | Thông tin được chỉnh sửa                                                                |
| ------------ | --------------------------------------------------------------------------------------- |
| Timeoff      | Request Name, Shift, Substitute, Reason, Attached Document, Add Timeoff, Delete Timeoff |
| Shift Change | Request Name, Shift, Substitute Shift, Substitute, Reason, Attached Document            |

**Quy tắc tài liệu đính kèm:**

| Quy tắc              | Mô tả                    |
| -------------------- | ------------------------ |
| Số lượng file tối đa | 03 file/đề xuất          |
| Dung lượng tối đa    | 10MB/file                |
| Định dạng hỗ trợ     | pdf, jpg, png, doc, docx |

### Quy tắc hủy đề xuất Approved

| Loại đề xuất | Quy tắc sau khi hủy                                                                                                                                    |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Timeoff      | Nếu ca trực trong đề xuất vẫn đang trống Lễ tân, hệ thống điền lại tên Lễ tân đã hủy đề xuất vào ca trực đó.                                           |
| Timeoff      | Nếu ca trực trong đề xuất đã được gắn với Lễ tân khác, hệ thống giữ nguyên thông tin Lễ tân hiện tại.                                                  |
| Timeoff      | Nếu tất cả ca trực trong đề xuất đều đã được gắn với Lễ tân khác, hệ thống không cho phép hủy và hiển thị lỗi **"Các ca trực đã có lễ tân thay thế"**. |
| Shift Change | Hệ thống đổi ngược lại ca trực, Lễ tân trực đúng ca như ban đầu trước khi đề xuất được duyệt.                                                          |

### Quy tắc xóa đề xuất

| Quy tắc         | Mô tả                                                 |
| --------------- | ----------------------------------------------------- |
| Điều kiện xóa   | Đề xuất phải có trạng thái **Pending**.               |
| Người được xóa  | Chỉ người tạo đề xuất được phép xóa đề xuất.          |
| Xác nhận xóa    | Hệ thống hiển thị popup xác nhận trước khi xóa.       |
| Sau khi xóa     | Hệ thống xóa đề xuất khỏi danh sách.                  |
| Email thông báo | Hệ thống gửi email thông báo cho người duyệt đề xuất. |

{% hint style="info" %}
**Mẹo sử dụng**

1. Nếu phát hiện sai thông tin khi đề xuất còn **Pending**, nên chỉnh sửa thay vì xóa rồi tạo lại.
2. Chỉ nên xóa đề xuất khi không còn nhu cầu xử lý đề xuất đó.
3. Nếu đề xuất đã **Approved** nhưng không còn nhu cầu xin nghỉ/đổi ca, dùng thao tác hủy bằng cách chuyển trạng thái sang **Cancelled**.
4. Trước khi hủy đề xuất Timeoff đã duyệt, nên kiểm tra xem ca trực đã có Lễ tân thay thế hay chưa.
5. Với đề xuất Shift Change đã duyệt, lưu ý thao tác hủy sẽ đổi ngược ca trực về như ban đầu.
6. Nên kiểm tra lại danh sách Receptionist Shift sau khi hủy đề xuất để đảm bảo lịch trực được cập nhật đúng.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                    | Nguyên nhân                                                                    | Cách xử lý                                                                          |
| --------------------------------------------------- | ------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------- |
| Không thấy nút Edit                                 | Tài khoản không có quyền chỉnh sửa hoặc không phải người tạo đề xuất           | Kiểm tra quyền và người tạo đề xuất                                                 |
| Không chỉnh sửa được đề xuất                        | Đề xuất không ở trạng thái Pending hoặc người dùng không phải người tạo        | Chỉ chỉnh sửa đề xuất Pending do chính mình tạo                                     |
| Không thấy nút Delete                               | Đề xuất không ở trạng thái Pending hoặc tài khoản không có quyền xóa           | Kiểm tra trạng thái đề xuất và phân quyền                                           |
| Không xóa được đề xuất                              | Đề xuất đã được duyệt, bị từ chối hoặc đã hủy                                  | Chỉ xóa được đề xuất Pending                                                        |
| Không hủy được đề xuất Approved                     | Tất cả ca trực trong đề xuất Timeoff đã có Lễ tân thay thế                     | Hệ thống không cho phép hủy và hiển thị lỗi **"Các ca trực đã có lễ tân thay thế"** |
| File đính kèm bị lỗi                                | File sai định dạng, vượt quá 10MB hoặc vượt quá 3 file                         | Kiểm tra định dạng, dung lượng và số lượng file                                     |
| Hủy đề xuất nhưng lịch trực không đổi như mong muốn | Ca trực đã được gắn với Lễ tân khác nên hệ thống giữ nguyên thông tin hiện tại | Kiểm tra lại logic hủy Timeoff và danh sách Receptionist Shift                      |
