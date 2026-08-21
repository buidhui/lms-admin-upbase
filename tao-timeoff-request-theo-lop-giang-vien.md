# Tạo Timeoff Request theo Lớp/Giảng viên

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version |
| -------------- | --------------- | ----- | ------------------ | ------- |
| Jul 16, 2026   | Nguyễn Duy Hiếu | A     |                    | 1.0.0   |

## I. Giới Thiệu Chung

**Dành cho:** Admin CX

**Đường dẫn:** https://ops.sapp.edu.vn/

#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance) – Attendance Adjustment
* **Chức năng chính:** Tạo phiếu Timeoff Request loại Attendance Adjustment để điều chỉnh chấm công
* **Trường hợp áp dụng:** Quên chấm công, hệ thống không ghi nhận đủ công, ghi nhận sai công, chấm công bù…
* **Module liên quan:**
  * Class (Quản lý lớp học)
  * Teacher (Quản lý giảng viên)
  * Timeoff Request
  * Resource Manager (Attendance Evidence)

#### Điều kiện tiên quyết

* User đã đăng nhập thành công vào hệ thống OPS.
* User có quyền tạo Timeoff Request: User là CX Admin của lớp giảng viên dạy

## II. Hướng dẫn chi tiết

### Cách 1 — Tạo Timeoff Request theo Lớp học

> 🎯 _Mục tiêu: Tạo phiếu Attendance Adjustment cho buổi học của giảng viên từ màn chi tiết lớp._

{% stepper %}
{% step %}
## Đăng nhập hệ thống OPS
{% endstep %}

{% step %}
## Chọn Class
{% endstep %}

{% step %}
## Tại màn hình Class Detail, chọn tab Teacher
{% endstep %}

{% step %}
## Chọn thông tin Attendance theo từng Teacher
{% endstep %}

{% step %}
## Bấm nút "Action" → chọn "Create Timeoff Request"

![](<.gitbook/assets/image (775)>)
{% endstep %}

{% step %}
## Nhập thông tin request và bấm "Save"
{% endstep %}
{% endstepper %}

### Cách 2 — Tạo Timeoff Request theo Giảng viên

> 🎯 _Mục tiêu: Tạo phiếu Attendance Adjustment cho giảng viên từ bảng chấm công theo giảng viên._

{% stepper %}
{% step %}
## Đăng nhập hệ thống OPS
{% endstep %}

{% step %}
## Chọn Department → Operations
{% endstep %}

{% step %}
## Chọn Customer Experience
{% endstep %}

{% step %}
## Chọn Teacher
{% endstep %}

{% step %}
## Chọn tab Attendance
{% endstep %}

{% step %}
## Chọn thông tin Attendance theo từng Teacher
{% endstep %}

{% step %}
## Bấm nút "Action" → chọn "Create Timeoff Request"

![](<.gitbook/assets/image (776)>)
{% endstep %}

{% step %}
## Nhập thông tin request và bấm "Save"
{% endstep %}
{% endstepper %}

### Thông tin phiếu Create Request

Khi click **Create Timeoff Request**, hệ thống hiển thị màn hình nhập thông tin **Create Request**:

| Trường               | Bắt buộc? | Mô tả                                                                                                                                 |
| -------------------- | --------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Request Name         | Y         | Tên yêu cầu. Helper text: `[Tên người tạo]`_`[Loại request]`_`[Tháng năm tạo request]`. VD: `Nguyễn Văn A_Attendance Adjustment_0325` |
| Request Type         | Y         | Hiển thị mặc định: **Attendance Adjustment**                                                                                          |
| Teacher Name         | Y         | Hiển thị tên giảng viên được tạo Timeoff Request                                                                                      |
| Class Code           | Y         | Hiển thị Class Code của buổi học được chọn                                                                                            |
| Timeoff Date         | Y         | Hiển thị ngày/buổi học cần điều chỉnh công                                                                                            |
| Reason               | Y         | Lý do tạo request                                                                                                                     |
| Upload Evidence      | Y         | Upload bằng chứng (hình ảnh, video record buổi giảng…). Xem chi tiết quy tắc bên dưới                                                 |
| Check-in – Check-out | Y         | Điền thời gian check-in, check-out thực tế. Format: **HH:mm**                                                                         |

![](<.gitbook/assets/image (777)>)

### Quy tắc Upload Evidence

* **Cách upload:** Upload trực tiếp **hoặc** chọn từ Resource có sẵn.
* **Định dạng hỗ trợ:** MP4, MP3, WAV, M4A, PDF, DOCX, DOC, XLS, XLSX, CSV, TXT, PPT, PPTX, ZIP, JPG, JPEG, PNG, GIF, WEBP.
* **Giới hạn:** Tối đa **500MB/file**, tối đa **10 file**.
* **Lưu trữ:** File sau khi tải lên tự động được cập nhật vào Resource Manager theo địa chỉ `Attendance Evidence/[Tên File]`.
* **Quy tắc đặt tên file:** `[Tên GV]`_`[Class Code]`_`[Timeoff Date - ngày buổi học book timeoff, DD/MM/YYYY]_[Tên file gốc]`.

### Email thông báo gửi Approver khi tạo mới

Khi tạo mới request thành công, hệ thống gửi email đến Approver tương ứng:

* **Title:** Thông báo request cần phê duyệt: `[Tên request]`
* **Nội dung:** Thân gửi `[Tên người duyệt]`. Bạn có một request Attendance Adjustment từ `[Tên giảng viên được tạo Timeoff]` cần duyệt. Để xem thông tin chi tiết về request, vui lòng truy cập vào website của hệ thống: _\<Link>_.

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng — Rule validate khi tạo/chỉnh sửa

1. **Request Name** không được để trống.
2. **Reason** không được để trống.
3. **Upload Evidence** bắt buộc có ít nhất **1 file**.
4. **Check-in, Check-out** không được để trống.
5. **Check-in, Check-out** phải đúng format **HH:mm**.
6. **Check-in phải nhỏ hơn Check-out.**

{% hint style="warning" %}
Nếu không nhập các trường Required, màn hình hiển thị message thông báo lỗi và **không thể click nút Save**.
{% endhint %}

### Mẹo sử dụng

1. Đặt Request Name theo helper text gợi ý để dễ tra cứu về sau.
2. Chuẩn bị sẵn file bằng chứng (video/ảnh buổi giảng) trước khi tạo phiếu.
3. Kiểm tra Check-in/Check-out thực tế trước khi Save để tránh phải chỉnh sửa lại.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                  | Nguyên nhân                                                     | Cách xử lý                                                                                 |
| ------------------------------------------------- | --------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Không click được nút "Save"                       | Chưa nhập đủ các trường Required                                | Điền đầy đủ Request Name, Reason, Evidence (≥1 file), Check-in, Check-out                  |
| Báo lỗi Check-in/Check-out                        | Sai format hoặc Check-in ≥ Check-out                            | Nhập đúng format HH:mm và đảm bảo Check-in nhỏ hơn Check-out                               |
| Cảnh báo trùng phiếu Pending (chặn cứng)          | Đã tồn tại phiếu Pending cùng Teacher/Timeoff Date/Check-in-out | Bấm **Edit existing request** để chỉnh sửa phiếu cũ thay vì tạo mới (xem _Business Rules_) |
| Cảnh báo trùng phiếu Approved (xác nhận tiếp tục) | Đã tồn tại phiếu Approved trùng và công đã được cập nhật        | Cân nhắc, nếu vẫn cần tạo phiếu mới thì bấm **Yes** để tiếp tục Save                       |
