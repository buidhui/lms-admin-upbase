# Gắn chứng chỉ cho khóa học (Certificate)

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 25, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn Admin cách sử dụng bước **Certificate** để gán mẫu chứng chỉ cho khóa học trên hệ thống **OPS**.

Chức năng **Certificate** cho phép Admin chọn một mẫu chứng chỉ đã được tạo sẵn trên hệ thống để gắn vào Course. Sau khi học viên hoàn thành khóa học và đáp ứng điều kiện nhận chứng chỉ, hệ thống sẽ sử dụng mẫu chứng chỉ đã chọn để cấp chứng chỉ cho học viên.

***

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                            | Quyền hạn                                                       |
| --------- | ---------------------------------- | --------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành khóa học   | Có quyền chọn và gán chứng chỉ cho khóa học                     |
| SX        | Người phụ trách nội dung học thuật | Có thể kiểm tra mẫu chứng chỉ phù hợp với chương trình/khóa học |

***

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Course 4 Level / Certificate
* **Module liên quan:**
  * Course Info
  * Course Content
  * Resource
  * Certificate Template
  * LMS học viên

Phạm vi của chức năng **Certificate** bao gồm:

* Truy cập bước Certificate trong quy trình tạo/chỉnh sửa khóa học.
* Chọn mẫu chứng chỉ từ danh sách template có sẵn.
* Xác nhận mẫu chứng chỉ cần gán cho khóa học.
* Hoàn tất quy trình tạo/cấu hình khóa học.
* Thay đổi mẫu chứng chỉ đã gán nếu khóa học được phép chỉnh sửa.

***

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản người dùng có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công tại bước **Course Info**.

***

## II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (851).png" alt=""><figcaption></figcaption></figure>

Màn hình **Certificate** là bước cuối cùng trong quy trình tạo khóa học. Tại màn hình này, Admin chọn mẫu chứng chỉ để gán cho khóa học.

Thanh tiến trình phía trên màn hình hiển thị 4 bước:

| Bước       | Tên bước       | Mô tả                                   |
| ---------- | -------------- | --------------------------------------- |
| **Step 1** | Course Info    | Nhập thông tin chung của khóa học       |
| **Step 2** | Course Content | Tạo nội dung bài học                    |
| **Step 3** | Resource       | Tải lên hoặc chọn tài liệu cho khóa học |
| **Step 4** | Certificate    | Gán mẫu chứng chỉ cho khóa học          |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Gán chứng chỉ cho khóa học

_**Bước 1:**_ Admin chọn bước **Certificate** trên thanh process hoặc tiếp tục từ bước **Resource**.

<figure><img src="../../.gitbook/assets/image (853).png" alt=""><figcaption></figcaption></figure>

_**Bước 2:**_ Admin chọn **Choose Template** để mở danh sách mẫu chứng chỉ.

<figure><img src="../../.gitbook/assets/image (854).png" alt=""><figcaption></figcaption></figure>

_**Bước 3:**_ Hệ thống hiển thị popup **Choose Certificate Template** với danh sách các mẫu chứng chỉ có thể chọn.

<figure><img src="../../.gitbook/assets/image (855).png" alt=""><figcaption></figcaption></figure>

_**Bước 4:**_ Admin tick chọn mẫu chứng chỉ muốn gán cho khóa học.

Mỗi mẫu chứng chỉ hiển thị thông tin preview và tên template để Admin kiểm tra trước khi chọn.

_**Bước 5:**_ Admin chọn **Confirm** để xác nhận mẫu chứng chỉ đã chọn.

Sau khi xác nhận, hệ thống đóng popup và gán mẫu chứng chỉ vào khóa học.

<figure><img src="../../.gitbook/assets/image (856).png" alt=""><figcaption></figcaption></figure>

***

### 3.2 Thay đổi mẫu chứng chỉ đã gán

_**Bước 1:**_ Admin mở khóa học cần chỉnh sửa và truy cập bước **Certificate**.

_**Bước 2:**_ Admin chọn Icon đổi chứng chỉ để mở lại danh sách mẫu chứng chỉ.

<figure><img src="../../.gitbook/assets/image (852).png" alt=""><figcaption></figcaption></figure>

_**Bước 3:**_ Admin tick chọn mẫu chứng chỉ mới muốn sử dụng.

_**Bước 4:**_ Admin chọn **Confirm** để cập nhật mẫu chứng chỉ.

_**Bước 5:**_ Admin chọn **Finish** hoặc **Save** theo giao diện hệ thống để lưu thay đổi.

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* **Certificate** là bước cuối cùng trong quy trình tạo khóa học.
* Admin cần chọn mẫu chứng chỉ phù hợp với chương trình/khóa học.
* Nếu chưa có Certificate Template phù hợp, Admin cần tạo hoặc yêu cầu tạo template trước trong chức năng **Certificates**.
* Việc thay đổi chứng chỉ của khóa học có thể ảnh hưởng đến chứng chỉ học viên nhận được sau khi hoàn thành khóa học.

***

### 💡 Mẹo sử dụng

* Nên kiểm tra trước tên và hình ảnh preview của Certificate Template trước khi chọn.
* Nên đặt tên Certificate Template rõ ràng theo chương trình, môn học hoặc loại khóa học để dễ nhận diện.
* Nếu danh sách template nhiều, nên kiểm tra kỹ template cần chọn để tránh gán nhầm chứng chỉ.
