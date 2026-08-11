# Tải lên tài liệu cho khóa học (Resource)

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 25, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn Admin cách sử dụng chức năng **Resource** để tải lên hoặc chọn tài liệu học tập cho khóa học trên hệ thống **OPS**.

Chức năng **Resource** cho phép Admin quản lý danh sách tài liệu đính kèm của khóa học, bao gồm tài liệu được upload trong quá trình tạo **Course Content** và tài liệu được upload trực tiếp tại bước **Resource**. Sau khi tài liệu được thêm vào khóa học, Admin có thể xem danh sách, tìm kiếm, tải thêm tài liệu, tải xuống hoặc xóa tài liệu khỏi danh sách Resource của khóa học.

***

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                            | Quyền hạn                                                      |
| --------- | ---------------------------------- | -------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành khóa học   | Có quyền thêm, xóa, tải xuống và quản lý tài liệu của khóa học |
| SX        | Người phụ trách nội dung học thuật | Có quyền kiểm tra và bổ sung học liệu cho khóa học             |

***

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Resource
* **Module liên quan:**
  * Course Info
  * Course Content
  * Resources
  * LMS học viên

Phạm vi của chức năng **Resource** bao gồm:

* Xem danh sách tài liệu đã được thêm vào khóa học.
* Tìm kiếm tài liệu theo tên file.
* Upload tài liệu trực tiếp từ thiết bị cá nhân.
* Chọn tài liệu có sẵn từ kho học liệu của hệ thống.
* Hiển thị thông tin tài liệu gồm tên file, dung lượng và ngày tạo.
* Tải xuống tài liệu đã thêm vào khóa học.
* Xóa tài liệu khỏi danh sách Resource của khóa học nếu được phép.
* Chuyển sang bước **Certificate** sau khi hoàn tất cấu hình tài liệu.

***

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản người dùng có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công tại bước **Course Info**.
* Nội dung khóa học đã được tạo hoặc kiểm tra tại bước **Course Content**.
* Người dùng đã truy cập đến bước **Resource** trong quy trình tạo/chỉnh sửa khóa học.
* Đối với upload từ thiết bị, người dùng cần chuẩn bị file đúng định dạng và dung lượng hệ thống hỗ trợ.
* Đối với chọn từ kho học liệu, tài liệu cần đã tồn tại trong **Resources** của hệ thống.

***

## II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>

Màn hình **Resource** là bước thứ 3 trong quy trình tạo khóa học. Tại màn hình này, Admin có thể xem danh sách tài liệu đã được gắn với khóa học, tìm kiếm tài liệu và tải thêm tài liệu mới.

Thanh tiến trình phía trên màn hình hiển thị các bước:

| Bước       | Tên bước       | Mô tả                                           |
| ---------- | -------------- | ----------------------------------------------- |
| **Step 1** | Course Info    | Nhập thông tin chung của khóa học               |
| **Step 2** | Course Content | Tạo nội dung bài học                            |
| **Step 3** | Resource       | Tải lên hoặc chọn tài liệu cho khóa học         |
| **Step 4** | Certificate    | Chọn chứng chỉ cho học viên hoàn thành khóa học |

***

### Các thành phần chính trên màn hình Resource

| Khu vực / Thành phần        | Mô tả                                                                          |
| --------------------------- | ------------------------------------------------------------------------------ |
| **Search**                  | Cho phép Admin nhập từ khóa để tìm kiếm tài liệu theo tên file.                |
| **Search button**           | Thực hiện tìm kiếm tài liệu theo từ khóa đã nhập.                              |
| **Upload File**             | Mở popup upload/chọn tài liệu để thêm vào khóa học.                            |
| **Bảng danh sách Resource** | Hiển thị danh sách tài liệu đã được thêm vào khóa học.                         |
| **Checkbox chọn dòng**      | Cho phép chọn tài liệu trên danh sách nếu hệ thống hỗ trợ thao tác hàng loạt.  |
| **File name**               | Tên tài liệu.                                                                  |
| **Size**                    | Dung lượng tài liệu.                                                           |
| **Created date**            | Thời gian tài liệu được tạo/tải lên hệ thống.                                  |
| **Action/Menu ba chấm**     | Cho phép thao tác với từng tài liệu, ví dụ tải xuống hoặc xóa tài liệu.        |
| **Phân trang**              | Cho phép chuyển trang và điều chỉnh số lượng tài liệu hiển thị trên mỗi trang. |

***

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Xem danh sách tài liệu của khóa học

_**Bước 1:**_ Sau khi hoàn thành bước **Course Content**, Admin chuyển sang bước **Resource**.

<figure><img src="../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình danh sách tài liệu của khóa học.

_**Bước 2:**_ Admin xem danh sách tài liệu với các thông tin:

| Thông tin        | Mô tả                           |
| ---------------- | ------------------------------- |
| **File name**    | Tên tài liệu.                   |
| **Size**         | Dung lượng tài liệu.            |
| **Created date** | Thời gian tạo/tải lên tài liệu. |

***

### 3.2 Tìm kiếm tài liệu

_**Bước 1:**_ Admin nhập từ khóa vào ô **Search**.

<figure><img src="../../.gitbook/assets/image (847).png" alt=""><figcaption></figcaption></figure>

Admin nhập từ khóa vào ô **Search**.

_**Bước 2:**_ Admin chọn **Search**.

<figure><img src="../../.gitbook/assets/image (848).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách tài liệu có tên phù hợp với từ khóa đã nhập.

***

### 3.3 Upload tài liệu từ thiết bị

_**Bước 1:**_ Tại màn hình **Resource**, Admin chọn **Upload File**.

<figure><img src="../../.gitbook/assets/image (849).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup upload tài liệu.

_**Bước 2:**_ Admin chọn tab **Upload File**.

<figure><img src="../../.gitbook/assets/image (850).png" alt=""><figcaption></figcaption></figure>

_**Bước 3:**_ Admin có thể chọn file bằng một trong hai cách:

* Kéo thả file vào vùng upload.
* Chọn **Browse** để chọn file từ thiết bị cá nhân.

_**Bước 4:**_ Admin kiểm tra file trước khi upload:

| Điều kiện                               | Quy định                                                                                                  |
| --------------------------------------- | --------------------------------------------------------------------------------------------------------- |
| **Định dạng file**                      | .jpg, .jpeg, .png, .gif, .webp, .mp4, .pdf, .docx, .doc, .xls, .xlsx, .csv, .txt, .ppt, .pptx, .zip, .mp3 |
| **Dung lượng tối đa mỗi file**          | 500MB                                                                                                     |
| **Số lượng file tối đa mỗi lần upload** | 10 file                                                                                                   |

_**Bước 5:**_ Admin chọn **Upload** để tải tài liệu lên hệ thống.

Sau khi upload thành công, tài liệu được thêm vào danh sách Resource của khóa học và đồng thời được lưu vào kho học liệu của hệ thống.

***

### 3.4 Chọn tài liệu từ kho Resources

_**Bước 1:**_ Tại màn hình **Resource**, Admin chọn **Upload File**.

_**Bước 2:**_ Trong popup upload, Admin chuyển sang tab **Resources**.

<figure><img src="../../.gitbook/assets/Screenshot 2026-05-25 111408.png" alt=""><figcaption></figcaption></figure>

_**Bước 3:**_ Admin có thể tìm kiếm/lọc danh sách tài liệu có sẵn trong kho học liệu.

_**Bước 4:**_ Admin tick chọn một hoặc nhiều tài liệu cần thêm vào khóa học.

_**Bước 5:**_ Admin chọn **Save** để thêm các tài liệu đã chọn vào danh sách Resource của khóa học.

***

### 3.5 Tải xuống tài liệu

_**Bước 1:**_ Tại danh sách Resource, Admin xác định tài liệu cần tải xuống.

_**Bước 2:**_ Admin chọn biểu tượng **Action/Menu ba chấm** tại dòng tài liệu tương ứng.

_**Bước 3:**_ Admin chọn **Download**.

Hệ thống tải tài liệu về thiết bị của người dùng.

***

### 3.6 Xóa tài liệu khỏi khóa học

_**Bước 1:**_ Tại danh sách **Resource**, Admin xác định tài liệu cần xóa.

_**Bước 2:**_ Admin chọn biểu tượng **Action/Menu ba chấm** tại dòng tài liệu tương ứng.

_**Bước 3:**_ Admin chọn **Delete**.

Hệ thống xóa tài liệu khỏi danh sách Resource của khóa học nếu thao tác được phép.

> Lưu ý: Thao tác xóa tại danh sách Resource được hiểu là xóa tài liệu khỏi khóa học. Tùy theo cấu hình hệ thống, tài liệu gốc trong kho học liệu có thể vẫn được lưu trong **Resources**.

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Bước **Resource** là bước thứ 3 trong quy trình tạo khóa học.
* Danh sách Resource có thể bao gồm tài liệu upload từ bước **Course Content** và tài liệu upload trực tiếp tại bước **Resource**.
* Admin có thể thêm tài liệu bằng 2 cách:
  * Upload trực tiếp từ thiết bị.
  * Chọn tài liệu có sẵn từ kho **Resources**.
* Mỗi lần upload tối đa **10 file**.
* Dung lượng tối đa mỗi file là **500MB**.

***

### 💡 Mẹo sử dụng

* Nên đặt tên file rõ ràng theo cấu trúc môn học/chương/bài để dễ tìm kiếm.
* Với tài liệu đã có sẵn trong hệ thống, nên dùng tab **Resources** để tái sử dụng thay vì upload lại.
