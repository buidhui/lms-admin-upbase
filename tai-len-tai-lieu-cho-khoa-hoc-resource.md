# Tải lên tài liệu cho khóa học (Resource)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

**Dành cho:** Admin, SX

**Đường dẫn:** https://ops.sapp.edu.vn/course-full/undefined

#### Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Resource
* **Module liên quan:**
  * Course Info
  * Course Content
  * Resources
  * LMS học viên

#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản người dùng có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công tại bước **Course Info**.

## II. Hướng dẫn chi tiết

### Xem danh sách tài liệu của khóa học

{% stepper %}
{% step %}
## Sau khi hoàn thành bước Course Content, Admin chuyển sang bước Resource.

![](<.gitbook/assets/image (474)>)

Hệ thống hiển thị màn hình danh sách tài liệu của khóa học.
{% endstep %}

{% step %}
## Admin xem danh sách tài liệu với các thông tin:

| Thông tin        | Mô tả                           |
| ---------------- | ------------------------------- |
| **File name**    | Tên tài liệu.                   |
| **Size**         | Dung lượng tài liệu.            |
| **Created date** | Thời gian tạo/tải lên tài liệu. |
{% endstep %}
{% endstepper %}

### Tìm kiếm tài liệu

{% stepper %}
{% step %}
## Admin nhập từ khóa vào ô Search.

![](<.gitbook/assets/image (475)>)
{% endstep %}

{% step %}
## Admin chọn Search.

![](<.gitbook/assets/image (476)>)

Hệ thống hiển thị danh sách tài liệu có tên phù hợp với từ khóa đã nhập.
{% endstep %}
{% endstepper %}

### Upload tài liệu từ thiết bị

{% stepper %}
{% step %}
## Tại màn hình Resource, Admin chọn Upload File.

![](<.gitbook/assets/image (477)>)
{% endstep %}

{% step %}
## Admin chọn tab Upload File.

![](<.gitbook/assets/image (478)>)
{% endstep %}

{% step %}
## Admin có thể chọn file bằng một trong hai cách:

* Kéo thả file vào vùng upload.
* Chọn **Browse** để chọn file từ thiết bị cá nhân.
{% endstep %}

{% step %}
## Admin kiểm tra file trước khi upload:

| Điều kiện                               | Quy định                                                                                                  |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Định dạng file**                      | .jpg, .jpeg, .png, .gif, .webp, .mp4, .pdf, .docx, .doc, .xls, .xlsx, .csv, .txt, .ppt, .pptx, .zip, .mp3 |
| **Dung lượng tối đa mỗi file**          | 500MB                                                                                                     |
| **Số lượng file tối đa mỗi lần upload** | 10 file                                                                                                   |
{% endstep %}

{% step %}
## Admin chọn Upload để tải tài liệu lên hệ thống.

Sau khi upload thành công, tài liệu được thêm vào danh sách Resource của khóa học và đồng thời được lưu vào kho học liệu của hệ thống.
{% endstep %}
{% endstepper %}

### Chọn tài liệu từ kho Resources

{% stepper %}
{% step %}
## Tại màn hình Resource, Admin chọn Upload File.
{% endstep %}

{% step %}
## Trong popup upload, Admin chuyển sang tab Resources.

![](<.gitbook/assets/image (479)>)
{% endstep %}

{% step %}
## Admin có thể tìm kiếm/lọc danh sách tài liệu có sẵn trong kho học liệu.
{% endstep %}

{% step %}
## Admin tick chọn một hoặc nhiều tài liệu cần thêm vào khóa học.
{% endstep %}

{% step %}
## Admin chọn Save để thêm các tài liệu đã chọn vào danh sách Resource của khóa học.
{% endstep %}
{% endstepper %}

### Tải xuống tài liệu

{% stepper %}
{% step %}
## Tại danh sách Resource, Admin xác định tài liệu cần tải xuống.
{% endstep %}

{% step %}
## Admin chọn biểu tượng Action/Menu ba chấm tại dòng tài liệu tương ứng.
{% endstep %}

{% step %}
## Admin chọn Download.

Hệ thống tải tài liệu về thiết bị của người dùng.
{% endstep %}
{% endstepper %}

### Xóa tài liệu khỏi khóa học

{% stepper %}
{% step %}
## Tại danh sách Resource, Admin xác định tài liệu cần xóa.
{% endstep %}

{% step %}
## Admin chọn biểu tượng Action/Menu ba chấm tại dòng tài liệu tương ứng.
{% endstep %}

{% step %}
## Admin chọn Delete.

Hệ thống xóa tài liệu khỏi danh sách Resource của khóa học nếu thao tác được phép.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
**Lưu ý:** Thao tác xóa tại danh sách Resource được hiểu là xóa tài liệu khỏi khóa học. Tùy theo cấu hình hệ thống, tài liệu gốc trong kho học liệu có thể vẫn được lưu trong **Resources**.
{% endhint %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Bước **Resource** là bước thứ 3 trong quy trình tạo khóa học.
2. Danh sách Resource có thể bao gồm tài liệu upload từ bước **Course Content** và tài liệu upload trực tiếp tại bước **Resource**.
3. Admin có thể thêm tài liệu bằng 2 cách:
   * Upload trực tiếp từ thiết bị.
   * Chọn tài liệu có sẵn từ kho **Resources**.
4. Mỗi lần upload tối đa **10 file**.
5. Dung lượng tối đa mỗi file là **500MB**.

### Mẹo sử dụng

1. Nên đặt tên file rõ ràng theo cấu trúc môn học/chương/bài để dễ tìm kiếm.
2. Với tài liệu đã có sẵn trong hệ thống, nên dùng tab **Resources** để tái sử dụng thay vì upload lại.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                        | Nguyên nhân                                                         | Cách xử lý                                                 |
| --------------------------------------- | ------------------------------------------------------------------- | ---------------------------------------------------------- |
| Không thấy nút Upload File              | Tài khoản chưa có quyền upload/chỉnh sửa khóa học                   | Liên hệ Admin hệ thống để kiểm tra phân quyền              |
| Không upload được file                  | File không đúng định dạng hoặc vượt quá dung lượng cho phép         | Kiểm tra định dạng file và dung lượng tối đa 500MB         |
| Không upload được nhiều file            | Số lượng file vượt quá giới hạn mỗi lần upload                      | Chỉ upload tối đa 10 file/lần                              |
| File upload xong không hiển thị         | Upload chưa thành công hoặc danh sách đang bị lọc theo từ khóa      | Kiểm tra thông báo upload, xóa từ khóa tìm kiếm và tìm lại |
| Không tìm thấy tài liệu trong Resources | Tài liệu chưa được upload vào kho học liệu hoặc bộ lọc chưa phù hợp | Upload tài liệu mới hoặc điều chỉnh điều kiện tìm kiếm     |
| Không xóa được tài liệu                 | Tài khoản không có quyền hoặc tài liệu bị ràng buộc dữ liệu         | Kiểm tra quyền tài khoản hoặc liên hệ Admin                |
| Tải xuống không thành công              | File không còn tồn tại hoặc kết nối bị gián đoạn                    | Tải lại hoặc kiểm tra file trên hệ thống                   |
