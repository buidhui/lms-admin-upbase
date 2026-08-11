# Tạo đơn xin nghỉ / đổi ca

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Receptionist Part-time, Facility Manager, Substitute Receptionist

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Request

#### Phạm vi & Module liên quan

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Request / Create Request
* **Module liên quan:** Receptionist Shift, Facility, Staff / Receptionist, Email Notification
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Receptionist Request** và quyền tạo đề xuất.
* Tài khoản có **Job Title = Receptionist Part-time**.
* Người dùng đã có ca trực trên hệ thống để chọn khi tạo đề xuất.
* Cơ sở của ca trực đã có **Facility Manager** để hệ thống gán người duyệt.
{% endhint %}

{% hint style="info" %}
Có 2 loại đề xuất: **Timeoff** (xin nghỉ một/nhiều ca) và **Shift Change** (đổi ca với một Lễ tân Part-time khác). Sau khi tạo thành công, đề xuất ở trạng thái **Pending** và gửi tới **Facility Manager** của cơ sở để duyệt.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Tạo đề xuất xin nghỉ ca trực (Timeoff)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Request**

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu.

<figure><img src="../../.gitbook/assets/image (551).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình **Receptionist Request List**.
{% endstep %}

{% step %}
**Chọn Create Request**

Lễ tân Part-time chọn **Create Request**.

<figure><img src="../../.gitbook/assets/image (552).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình tạo mới đề xuất.

<figure><img src="../../.gitbook/assets/image (553).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Request Name**

Lễ tân Part-time nhập **Request Name** (trường bắt buộc).
{% endstep %}

{% step %}
**Chọn Request Type = Timeoff**

Lễ tân Part-time chọn **Request Type = Timeoff**.

<figure><img src="../../.gitbook/assets/image (554).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị các trường thông tin tương ứng với đề xuất xin nghỉ.

<figure><img src="../../.gitbook/assets/image (555).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Facility và Shift**

Chọn **Facility** (cơ sở chứa ca trực muốn xin nghỉ) và **Shift** (danh sách chỉ hiển thị các ca trực của người tạo tại cơ sở đã chọn).
{% endstep %}

{% step %}
**Chọn Substitute (nếu có)**

Lễ tân Part-time chọn **Substitute** nếu đã có người trực thay (không bắt buộc với đề xuất xin nghỉ).
{% endstep %}

{% step %}
**Nhập Reason**

Lễ tân Part-time nhập **Reason** (trường bắt buộc) để ghi rõ lý do xin nghỉ.
{% endstep %}

{% step %}
**Upload Attached Document (nếu cần)**

Lễ tân Part-time upload **Attached Document** nếu cần. Hệ thống hỗ trợ tối đa 3 file, mỗi file tối đa 10MB.
{% endstep %}

{% step %}
**Thêm/xóa ca xin nghỉ (nếu cần)**

Chọn **Add Timeoff** để thêm ca xin nghỉ (tối đa 2 khoảng thời gian/ca trong một đề xuất); chọn **Delete Timeoff** để xóa ca đã thêm.

<figure><img src="../../.gitbook/assets/image (557).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (556).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Save**

Lễ tân Part-time chọn **Save**. Hệ thống tạo đề xuất với trạng thái **Pending**, gán người duyệt là **Facility Manager** của cơ sở đã chọn và gửi email thông báo cho người liên quan.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo đề xuất đổi ca trực (Shift Change)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Request**

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu.

<figure><img src="../../.gitbook/assets/image (558).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình **Receptionist Request List**.
{% endstep %}

{% step %}
**Chọn Create Request**

Lễ tân Part-time chọn **Create Request**.

<figure><img src="../../.gitbook/assets/image (559).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình tạo mới đề xuất.

<figure><img src="../../.gitbook/assets/image (560).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Request Name**

Lễ tân Part-time nhập **Request Name** (trường bắt buộc).
{% endstep %}

{% step %}
**Chọn Request Type = Shift Change**

Lễ tân Part-time chọn **Request Type = Shift Change**.

<figure><img src="../../.gitbook/assets/image (561).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị các trường thông tin tương ứng với đề xuất đổi ca.

<figure><img src="../../.gitbook/assets/image (562).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Facility và Shift**

Chọn **Facility** (cơ sở chứa ca trực muốn đổi) và **Shift** (ca trực gốc của người tạo tại cơ sở đã chọn).
{% endstep %}

{% step %}
**Chọn Substitute Shift và Substitute**

Chọn **Substitute Shift** (ca trực muốn đổi sang) và **Substitute** (người đang trực tại Substitute Shift đã chọn, chỉ có thể là **Lễ tân Part-time**).
{% endstep %}

{% step %}
**Nhập Reason**

Lễ tân Part-time nhập **Reason** (trường bắt buộc) để ghi rõ lý do đổi ca.
{% endstep %}

{% step %}
**Upload Attached Document (nếu cần)**

Lễ tân Part-time upload **Attached Document** nếu cần. Hệ thống hỗ trợ tối đa 3 file, mỗi file tối đa 10MB.
{% endstep %}

{% step %}
**Chọn Save**

Lễ tân Part-time chọn **Save**. Hệ thống tạo đề xuất với trạng thái **Pending**, gán người duyệt là **Facility Manager** của cơ sở đã chọn và gửi email thông báo cho người liên quan.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chức năng tạo đề xuất chỉ áp dụng cho tài khoản có **Job Title = Receptionist Part-time**.
2. Người dùng cần có quyền tạo đề xuất để nhìn thấy/sử dụng nút **Create Request**.
3. Các trường có dấu **(\*)** là trường bắt buộc.
4. Sau khi tạo thành công, đề xuất có trạng thái mặc định là **Pending**; người duyệt là **Facility Manager** của cơ sở được chọn.
5. Người dùng được tạo tối đa **03 request cùng loại trong 01 tháng**.
6. Sau khi tạo thành công, hệ thống gửi email cho **Facility Manager**; nếu có chọn **Substitute**, gửi thêm email cho người trực thay/người đổi ca.
7. Tài liệu đính kèm không bắt buộc.
{% endhint %}

### Quy tắc tạo đề xuất Timeoff

<table data-search="false"><thead><tr><th>Trường thông tin</th><th>Bắt buộc</th><th>Quy tắc</th></tr></thead><tbody><tr><td>Request Name</td><td>Có</td><td>Tên đề xuất xin nghỉ.</td></tr><tr><td>Request Type</td><td>Có</td><td>Chọn <strong>Timeoff</strong>.</td></tr><tr><td>Facility</td><td>Có</td><td>Cơ sở chứa ca trực muốn xin nghỉ.</td></tr><tr><td>Shift</td><td>Có</td><td>Chỉ hiển thị ca trực của người tạo tại Facility đã chọn.</td></tr><tr><td>Substitute</td><td>Không</td><td>Người trực thay cho người tạo đề xuất nếu có.</td></tr><tr><td>Reason</td><td>Có</td><td>Lý do xin nghỉ.</td></tr><tr><td>Attached Document</td><td>Không</td><td>Tối đa 3 file, mỗi file tối đa 10MB.</td></tr><tr><td>Add Timeoff</td><td>Không</td><td>Cho phép thêm tối đa 2 ca/khoảng thời gian xin nghỉ trong một đề xuất.</td></tr><tr><td>Delete Timeoff</td><td>Không</td><td>Cho phép xóa ca/khoảng thời gian xin nghỉ đã thêm.</td></tr></tbody></table>

### Quy tắc tạo đề xuất Shift Change

<table data-search="false"><thead><tr><th>Trường thông tin</th><th>Bắt buộc</th><th>Quy tắc</th></tr></thead><tbody><tr><td>Request Name</td><td>Có</td><td>Tên đề xuất đổi ca.</td></tr><tr><td>Request Type</td><td>Có</td><td>Chọn <strong>Shift Change</strong>.</td></tr><tr><td>Facility</td><td>Có</td><td>Cơ sở chứa ca trực muốn đổi.</td></tr><tr><td>Shift</td><td>Có</td><td>Ca trực gốc của người tạo tại Facility đã chọn.</td></tr><tr><td>Substitute Shift</td><td>Có</td><td>Ca trực mà người tạo muốn đổi sang.</td></tr><tr><td>Substitute</td><td>Có</td><td>Người đang trực tại Substitute Shift đã chọn. Chỉ có thể chọn Lễ tân Part-time.</td></tr><tr><td>Reason</td><td>Có</td><td>Lý do đổi ca.</td></tr><tr><td>Attached Document</td><td>Không</td><td>Tối đa 3 file, mỗi file tối đa 10MB.</td></tr></tbody></table>

### Quy tắc giới hạn số lượng request

| Quy tắc                     | Mô tả                                                           |
| --------------------------- | --------------------------------------------------------------- |
| Giới hạn theo loại request  | Người dùng được tạo tối đa 03 request cùng loại trong 01 tháng. |
| Request Type = Timeoff      | Tối đa 03 đề xuất Timeoff/tháng.                                |
| Request Type = Shift Change | Tối đa 03 đề xuất Shift Change/tháng.                           |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

<table data-search="false"><thead><tr><th>Lỗi / Tình huống</th><th>Nguyên nhân</th><th>Cách xử lý</th></tr></thead><tbody><tr><td>Không thấy nút Create Request</td><td>Tài khoản không phải Receptionist Part-time hoặc chưa có quyền tạo đề xuất</td><td>Kiểm tra Job Title và phân quyền</td></tr><tr><td>Không lưu được đề xuất</td><td>Thiếu trường bắt buộc</td><td>Kiểm tra các trường có dấu <strong>(*)</strong></td></tr><tr><td>Không thấy Shift cần xin nghỉ</td><td>Người dùng chưa có ca trực tại Facility đã chọn</td><td>Kiểm tra lại Facility hoặc lịch trực của người dùng</td></tr><tr><td>Không thấy Substitute Shift</td><td>Facility đã chọn chưa có ca phù hợp để đổi</td><td>Kiểm tra lại cơ sở hoặc lịch trực</td></tr><tr><td>Không chọn được Substitute</td><td>Người trực thay không thuộc Substitute Shift hoặc không phải Part-time</td><td>Chọn đúng người đang trực tại ca muốn đổi</td></tr><tr><td>Upload file bị lỗi</td><td>File sai định dạng, vượt quá 10MB hoặc vượt quá 3 file</td><td>Kiểm tra định dạng, dung lượng và số lượng file</td></tr><tr><td>Không tạo được thêm request</td><td>Đã đạt tối đa 03 request cùng loại trong tháng</td><td>Kiểm tra lại số request đã tạo trong tháng</td></tr><tr><td>Đề xuất không gửi tới người duyệt</td><td>Cơ sở chưa có Facility Manager hoặc dữ liệu người duyệt chưa đúng</td><td>Kiểm tra thông tin Facility Manager của cơ sở</td></tr></tbody></table>
