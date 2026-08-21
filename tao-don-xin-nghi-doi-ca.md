# Tạo đơn xin nghỉ / đổi ca

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Receptionist Part-time, Facility Manager, Substitute Receptionist

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Request

#### Phạm vi & Module liên quan

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Request / Create Request
* **Module liên quan:** Receptionist Shift, Facility, Staff / Receptionist, Email Notification

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Receptionist Request** và quyền tạo đề xuất.
* Tài khoản có **Job Title = Receptionist Part-time**.
* Người dùng đã có ca trực trên hệ thống để chọn khi tạo đề xuất.
* Cơ sở của ca trực đã có **Facility Manager** để hệ thống gán người duyệt.

Có 2 loại đề xuất: **Timeoff** (xin nghỉ một/nhiều ca) và **Shift Change** (đổi ca với một Lễ tân Part-time khác). Sau khi tạo thành công, đề xuất ở trạng thái **Pending** và gửi tới **Facility Manager** của cơ sở để duyệt.

## II. Hướng dẫn chi tiết

### Tạo đề xuất xin nghỉ ca trực (Timeoff)

{% stepper %}
{% step %}
## Truy cập màn hình Receptionist Request

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu.

![](<.gitbook/assets/image (736)>)

Hệ thống hiển thị màn hình **Receptionist Request List**.
{% endstep %}

{% step %}
## Chọn Create Request

Lễ tân Part-time chọn **Create Request**.

![](<.gitbook/assets/image (737)>)

Hệ thống mở màn hình tạo mới đề xuất.

![](<.gitbook/assets/image (738)>)
{% endstep %}

{% step %}
## Nhập Request Name

Lễ tân Part-time nhập **Request Name** (trường bắt buộc).
{% endstep %}

{% step %}
## Chọn Request Type = Timeoff

Lễ tân Part-time chọn **Request Type = Timeoff**.

![](<.gitbook/assets/image (739)>)

Hệ thống hiển thị các trường thông tin tương ứng với đề xuất xin nghỉ.

![](<.gitbook/assets/image (740)>)
{% endstep %}

{% step %}
## Chọn Facility và Shift

Chọn **Facility** (cơ sở chứa ca trực muốn xin nghỉ) và **Shift** (danh sách chỉ hiển thị các ca trực của người tạo tại cơ sở đã chọn).
{% endstep %}

{% step %}
## Chọn Substitute (nếu có)

Lễ tân Part-time chọn **Substitute** nếu đã có người trực thay (không bắt buộc với đề xuất xin nghỉ).
{% endstep %}

{% step %}
## Nhập Reason

Lễ tân Part-time nhập **Reason** (trường bắt buộc) để ghi rõ lý do xin nghỉ.
{% endstep %}

{% step %}
## Upload Attached Document (nếu cần)

Lễ tân Part-time upload **Attached Document** nếu cần. Hệ thống hỗ trợ tối đa 3 file, mỗi file tối đa 10MB.
{% endstep %}

{% step %}
## Thêm/xóa ca xin nghỉ (nếu cần)

Chọn **Add Timeoff** để thêm ca xin nghỉ (tối đa 2 khoảng thời gian/ca trong một đề xuất); chọn **Delete Timeoff** để xóa ca đã thêm.

![](<.gitbook/assets/image (741)>)

![](<.gitbook/assets/image (742)>)
{% endstep %}

{% step %}
## Chọn Save

Lễ tân Part-time chọn **Save**. Hệ thống tạo đề xuất với trạng thái **Pending**, gán người duyệt là **Facility Manager** của cơ sở đã chọn và gửi email thông báo cho người liên quan.
{% endstep %}
{% endstepper %}

### Tạo đề xuất đổi ca trực (Shift Change)

{% stepper %}
{% step %}
## Truy cập màn hình Receptionist Request

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Request** trên thanh menu.

![](<.gitbook/assets/image (743)>)

Hệ thống hiển thị màn hình **Receptionist Request List**.
{% endstep %}

{% step %}
## Chọn Create Request

Lễ tân Part-time chọn **Create Request**.

![](<.gitbook/assets/image (744)>)

Hệ thống mở màn hình tạo mới đề xuất.

![](<.gitbook/assets/image (745)>)
{% endstep %}

{% step %}
## Nhập Request Name

Lễ tân Part-time nhập **Request Name** (trường bắt buộc).
{% endstep %}

{% step %}
## Chọn Request Type = Shift Change

Lễ tân Part-time chọn **Request Type = Shift Change**.

![](<.gitbook/assets/image (746)>)

Hệ thống hiển thị các trường thông tin tương ứng với đề xuất đổi ca.

![](<.gitbook/assets/image (747)>)
{% endstep %}

{% step %}
## Chọn Facility và Shift

Chọn **Facility** (cơ sở chứa ca trực muốn đổi) và **Shift** (ca trực gốc của người tạo tại cơ sở đã chọn).
{% endstep %}

{% step %}
## Chọn Substitute Shift và Substitute

Chọn **Substitute Shift** (ca trực muốn đổi sang) và **Substitute** (người đang trực tại Substitute Shift đã chọn, chỉ có thể là **Lễ tân Part-time**).
{% endstep %}

{% step %}
## Nhập Reason

Lễ tân Part-time nhập **Reason** (trường bắt buộc) để ghi rõ lý do đổi ca.
{% endstep %}

{% step %}
## Upload Attached Document (nếu cần)

Lễ tân Part-time upload **Attached Document** nếu cần. Hệ thống hỗ trợ tối đa 3 file, mỗi file tối đa 10MB.
{% endstep %}

{% step %}
## Chọn Save

Lễ tân Part-time chọn **Save**. Hệ thống tạo đề xuất với trạng thái **Pending**, gán người duyệt là **Facility Manager** của cơ sở đã chọn và gửi email thông báo cho người liên quan.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chức năng tạo đề xuất chỉ áp dụng cho tài khoản có **Job Title = Receptionist Part-time**.
2. Người dùng cần có quyền tạo đề xuất để nhìn thấy/sử dụng nút **Create Request**.
3. Các trường có dấu **(\*)** là trường bắt buộc.
4. Sau khi tạo thành công, đề xuất có trạng thái mặc định là **Pending**; người duyệt là **Facility Manager** của cơ sở được chọn.
5. Người dùng được tạo tối đa **03 request cùng loại trong 01 tháng**.
6. Sau khi tạo thành công, hệ thống gửi email cho **Facility Manager**; nếu có chọn **Substitute**, gửi thêm email cho người trực thay/người đổi ca.
7. Tài liệu đính kèm không bắt buộc.

### Quy tắc tạo đề xuất Timeoff

| Trường thông tin  | Bắt buộc | Quy tắc                                                                |
| ----------------- | -------- | ---------------------------------------------------------------------- |
| Request Name      | Có       | Tên đề xuất xin nghỉ.                                                  |
| Request Type      | Có       | Chọn **Timeoff**.                                                      |
| Facility          | Có       | Cơ sở chứa ca trực muốn xin nghỉ.                                      |
| Shift             | Có       | Chỉ hiển thị ca trực của người tạo tại Facility đã chọn.               |
| Substitute        | Không    | Người trực thay cho người tạo đề xuất nếu có.                          |
| Reason            | Có       | Lý do xin nghỉ.                                                        |
| Attached Document | Không    | Tối đa 3 file, mỗi file tối đa 10MB.                                   |
| Add Timeoff       | Không    | Cho phép thêm tối đa 2 ca/khoảng thời gian xin nghỉ trong một đề xuất. |
| Delete Timeoff    | Không    | Cho phép xóa ca/khoảng thời gian xin nghỉ đã thêm.                     |

### Quy tắc tạo đề xuất Shift Change

| Trường thông tin  | Bắt buộc | Quy tắc                                                                         |
| ----------------- | -------- | ------------------------------------------------------------------------------- |
| Request Name      | Có       | Tên đề xuất đổi ca.                                                             |
| Request Type      | Có       | Chọn **Shift Change**.                                                          |
| Facility          | Có       | Cơ sở chứa ca trực muốn đổi.                                                    |
| Shift             | Có       | Ca trực gốc của người tạo tại Facility đã chọn.                                 |
| Substitute Shift  | Có       | Ca trực mà người tạo muốn đổi sang.                                             |
| Substitute        | Có       | Người đang trực tại Substitute Shift đã chọn. Chỉ có thể chọn Lễ tân Part-time. |
| Reason            | Có       | Lý do đổi ca.                                                                   |
| Attached Document | Không    | Tối đa 3 file, mỗi file tối đa 10MB.                                            |

### Quy tắc giới hạn số lượng request

| Quy tắc                     | Mô tả                                                           |
| --------------------------- | --------------------------------------------------------------- |
| Giới hạn theo loại request  | Người dùng được tạo tối đa 03 request cùng loại trong 01 tháng. |
| Request Type = Timeoff      | Tối đa 03 đề xuất Timeoff/tháng.                                |
| Request Type = Shift Change | Tối đa 03 đề xuất Shift Change/tháng.                           |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                  | Nguyên nhân                                                                | Cách xử lý                                          |
| --------------------------------- | -------------------------------------------------------------------------- | --------------------------------------------------- |
| Không thấy nút Create Request     | Tài khoản không phải Receptionist Part-time hoặc chưa có quyền tạo đề xuất | Kiểm tra Job Title và phân quyền                    |
| Không lưu được đề xuất            | Thiếu trường bắt buộc                                                      | Kiểm tra các trường có dấu **(\*)**                 |
| Không thấy Shift cần xin nghỉ     | Người dùng chưa có ca trực tại Facility đã chọn                            | Kiểm tra lại Facility hoặc lịch trực của người dùng |
| Không thấy Substitute Shift       | Facility đã chọn chưa có ca phù hợp để đổi                                 | Kiểm tra lại cơ sở hoặc lịch trực                   |
| Không chọn được Substitute        | Người trực thay không thuộc Substitute Shift hoặc không phải Part-time     | Chọn đúng người đang trực tại ca muốn đổi           |
| Upload file bị lỗi                | File sai định dạng, vượt quá 10MB hoặc vượt quá 3 file                     | Kiểm tra định dạng, dung lượng và số lượng file     |
| Không tạo được thêm request       | Đã đạt tối đa 03 request cùng loại trong tháng                             | Kiểm tra lại số request đã tạo trong tháng          |
| Đề xuất không gửi tới người duyệt | Cơ sở chưa có Facility Manager hoặc dữ liệu người duyệt chưa đúng          | Kiểm tra thông tin Facility Manager của cơ sở       |
