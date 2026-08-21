# Program Category

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 18, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Program Category** trên hệ thống vận hành.

Chức năng **Program Category** cho phép Admin quản lý danh sách loại chương trình học/nhóm chương trình học trên hệ thống. Thông qua chức năng này, Admin có thể xem danh sách, tìm kiếm, tạo mới và chỉnh sửa thông tin Program Category để phục vụ việc phân loại khóa học trong hệ thống.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                  | Quyền hạn                                                               |
| --------- | ---------------------------------------- | ----------------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành chương trình học | Có quyền xem danh sách, tìm kiếm, tạo mới và chỉnh sửa Program Category |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Course & Materials
* **Chức năng chính:** Program Category
* **Module liên quan:** Course

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Tài khoản người dùng có quyền truy cập menu **Program Category**.
* Tài khoản người dùng có quyền xem danh sách Program Category.
* Đối với thao tác tạo mới, tài khoản cần có quyền tạo Program Category.
* Đối với thao tác chỉnh sửa, tài khoản cần có quyền chỉnh sửa Program Category.

## II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (59).png" alt=""><figcaption></figcaption></figure>

Màn hình **Program Category** cho phép Admin xem và quản lý danh sách các loại chương trình học đã được tạo trên hệ thống.

Tại màn hình này, Admin có thể:

* Xem danh sách Program Category.
* Tìm kiếm/lọc Program Category theo tên hoặc ngày tạo.
* Tạo mới Program Category.
* Chỉnh sửa thông tin Program Category đã tạo.

***

### Các thành phần chính trên màn hình

| Khu vực / Thành phần                | Mô tả                                                                               |
| ----------------------------------- | ----------------------------------------------------------------------------------- |
| **Vùng tìm kiếm/lọc**               | Cho phép Admin tìm kiếm hoặc lọc danh sách Program Category theo tên hoặc ngày tạo. |
| **Nút Search**                      | Thực hiện tìm kiếm danh sách Program Category theo điều kiện đã nhập.               |
| **Nút Reset**                       | Xóa điều kiện tìm kiếm/lọc và hiển thị lại danh sách mặc định.                      |
| **Nút Add Category**                | Mở form tạo mới Program Category ở phía bên phải màn hình.                          |
| **Bảng danh sách Program Category** | Hiển thị danh sách các Program Category đã được tạo trên hệ thống.                  |
| **Category name**                   | Tên loại chương trình học.                                                          |
| **Description**                     | Mô tả chương trình học.                                                             |
| **Update at**                       | Thời gian tạo chương trình học & Thời gian cập nhật gần nhất.                       |
| **Action**                          | Cho phép Admin thực hiện thao tác chỉnh sửa Program Category tương ứng.             |

## III. Các Bước Thực Hiện Chi Tiết

### 1. Xem danh sách Program Category <a href="#id-1.-xem-danh-sach-course-category" id="id-1.-xem-danh-sach-course-category"></a>

Màn hình hiển thị danh sách Program được hiển thị như sau:

<figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>

Tại màn hình Program Category, Admin có thể tìm kiếm/lọc danh sách Program theo tên hoặc ngày tạo tại khu vực tìm kiếm

<figure><img src="../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

Tại khu vực hiển thị danh sách Program, các thông tin được hiển thị bao gồm

| **Thông tin** | **Mô tả**                      |
| ------------- | ------------------------------ |
| Category name | Tên loại chương trình học      |
| Description   | Mô tả chương trình học         |
| Created       | Thời gian tạo chương trình học |
| Updated       | Thời gian cập nhật gần nhất    |

### 2. Tạo một Program <a href="#id-2.-tao-mot-course-category" id="id-2.-tao-mot-course-category"></a>

**Bước 1:** Admin thực hiện click button Add Category tại màn hình

<figure><img src="../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Admin nhập thông tin vào màn hình tạo mới Program hiển thị phía bên phải như ảnh dưới đây:

<figure><img src="../../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

Thông tin cần nhập bao gồm:

* Tên Program: đây là trường yêu cầu bắt buộc phải nhập để có thể tạo mới. Tên Programkhông được phép trùng với Program đã tồn tại
* Mô tả: Admin thực hiện nhập mô tả cho Program. Đây là trường không bắt buộc, vì vậy Admin có thể điền hoặc không

**Bước 3:** Admin thực hiện ckick button Save để lưu Program mới

Sau khi click button Save, màn hình sẽ hiển thị message thông báo tạo mới Proghram thành công

### 3. Chỉnh sửa một Program <a href="#id-3.-chinh-sua-mot-course-category" id="id-3.-chinh-sua-mot-course-category"></a>

Để chỉnh sửa Program đã tạo, Admin thực hiện click vào biểu tượng Action tại Program muốn chỉnh sửa rồi chọn Edit

<figure><img src="../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>

Sau khi chọn Edit, thông tin của Program được hiển thị phía bên phải như ảnh sau:

<figure><img src="../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

Admin thực hiện chỉnh sửa nội dung của Program gồm các thông tin sau:

* Tên của Program: đảm bảo tên của Program không trùng với Program đã tồn tại
* Mô tả Program: Admin có thể nhập/xóa nội dung mô tả Program

Sau khi chỉnh sửa nội dung của Program, Admin thực hiện click Save để lưu thông tin mới. Sau khi click Save, màn hình sẽ hiển thị message thông báo lưu thông tin thành công

> **Lưu ý:**\
> Program đã tạo thì không thể xóa khỏi danh sách

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Admin cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa Program Category.
* Tên Program Category không được phép trùng với Program Category đã tồn tại.
* Trường **Description** không bắt buộc, Admin có thể nhập hoặc để trống.
* Program Category đã tạo thì **không thể xóa khỏi danh sách**.

***

### 💡 Mẹo sử dụng

* Trước khi tạo mới Program Category, Admin nên tìm kiếm theo tên để kiểm tra Program Category đã tồn tại hay chưa.
* Nên đặt tên Program Category ngắn gọn, rõ nghĩa và thống nhất theo quy chuẩn đặt tên của hệ thống.
* Nên nhập mô tả để người dùng khác hiểu rõ Program Category đang dùng cho nhóm chương trình học nào.
* Với Program Category đã tạo sai hoặc không còn sử dụng, do hệ thống không hỗ trợ xóa, Admin nên cân nhắc chỉnh sửa tên/mô tả theo quy ước nội bộ, ví dụ thêm ghi chú “Không sử dụng” nếu được phép.
* Khi chỉnh sửa tên Program Category, cần kiểm tra kỹ để tránh ảnh hưởng đến việc nhận diện nhóm chương trình học ở các màn hình liên quan.
