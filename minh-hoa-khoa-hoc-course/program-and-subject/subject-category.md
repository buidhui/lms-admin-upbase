# Subject Category

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 18, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Subject Category** trên hệ thống vận hành.

Chức năng **Subject Category** cho phép Admin quản lý danh sách môn học thuộc từng **Program**. Thông qua chức năng này, Admin có thể xem danh sách Subject, tìm kiếm/lọc Subject, tạo mới Subject, chỉnh sửa thông tin Subject và xóa Subject nếu Subject chưa được sử dụng trong khóa học.

Subject là dữ liệu danh mục quan trọng, được sử dụng để phân loại và tổ chức các khóa học theo đúng chương trình học tương ứng.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                  | Quyền hạn                                                                           |
| --------- | ---------------------------------------- | ----------------------------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành chương trình học | Có quyền xem danh sách, tìm kiếm, tạo mới, chỉnh sửa và xóa Subject theo phân quyền |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Subject Category
* **Module liên quan:**
  * Program Category
  * Course
  * Course 4 Level
  * Class

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Tài khoản người dùng có quyền truy cập menu **Subject Category**.
* Tài khoản người dùng có quyền xem danh sách Subject.
* Đối với thao tác tạo mới, tài khoản cần có quyền tạo Subject.
* Đối với thao tác chỉnh sửa, tài khoản cần có quyền chỉnh sửa Subject.
* Đối với thao tác xóa, tài khoản cần có quyền xóa Subject.
* Program cần tồn tại trên hệ thống trước khi Admin gán Subject vào Program tương ứng.
* Subject chỉ có thể xóa khi chưa được gán với bất kỳ khóa học nào.

## II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (67).png" alt=""><figcaption></figcaption></figure>

Màn hình **Subject Category** hiển thị danh sách các môn học đã được tạo trên hệ thống. Mỗi Subject thuộc một Program cụ thể và được sử dụng để phân loại khóa học.

Người dùng truy cập chức năng theo đường dẫn:

**Academic Management → Course & Materials → Subject Category**

Tại màn hình này, Admin có thể:

* Xem danh sách Subject.
* Tìm kiếm Subject theo tên hoặc từ khóa.
* Lọc Subject theo Program.
* Lọc Subject theo khoảng thời gian.
* Tạo mới Subject.
* Chỉnh sửa Subject.
* Xóa Subject nếu Subject chưa được gán với khóa học.

***

### Các thành phần chính trên màn hình

| Khu vực / Thành phần       | Mô tả                                                                |
| -------------------------- | -------------------------------------------------------------------- |
| **Search**                 | Cho phép Admin nhập từ khóa để tìm kiếm Subject.                     |
| **Program**                | Cho phép lọc danh sách Subject theo Program.                         |
| **From date**              | Lọc danh sách Subject từ ngày bắt đầu.                               |
| **To date**                | Lọc danh sách Subject đến ngày kết thúc.                             |
| **Reset**                  | Xóa toàn bộ điều kiện tìm kiếm/lọc đã nhập.                          |
| **Search button**          | Thực hiện tìm kiếm/lọc danh sách Subject theo điều kiện đã nhập.     |
| **Add Subject**            | Mở form tạo mới Subject.                                             |
| **Bảng danh sách Subject** | Hiển thị danh sách Subject hiện có trên hệ thống.                    |
| **Action**                 | Cho phép Admin thực hiện thao tác Edit hoặc Delete với từng Subject. |

## III. Các Bước Thực Hiện Chi Tiết

### 1. Xem danh sách Subject Category <a href="#id-1.-xem-danh-sach-course-category" id="id-1.-xem-danh-sach-course-category"></a>

Màn hình hiển thị danh sách Program được hiển thị như sau:

<figure><img src="../../.gitbook/assets/image (68).png" alt=""><figcaption></figcaption></figure>

Tại màn hình Subject Category, Admin có thể tìm kiếm/lọc danh sách Subject theo tên, Program hoặc ngày tạo tại khu vực tìm kiếm

<figure><img src="../../.gitbook/assets/image (69).png" alt=""><figcaption></figcaption></figure>

Tại khu vực hiển thị danh sách Subject, các thông tin được hiển thị bao gồm

| **Thông tin** | **Mô tả**                        |
| ------------- | -------------------------------- |
| Subject name  | Tên môn học                      |
| Code          | Mã môn học                       |
| Program       | Chương trình học gán với môn học |
| Updated at    | Thời gian cập nhật gần nhất      |

### 2. Tạo một Program <a href="#id-2.-tao-mot-course-category" id="id-2.-tao-mot-course-category"></a>

**Bước 1:** Admin thực hiện click button Add Subject tại màn hình

<figure><img src="../../.gitbook/assets/image (70).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Admin nhập thông tin vào màn hình tạo mới Subject hiển thị phía bên phải như ảnh dưới đây:

<figure><img src="../../.gitbook/assets/image (71).png" alt=""><figcaption></figcaption></figure>

Thông tin cần nhập bao gồm:

* Tên Subject: đây là trường yêu cầu bắt buộc phải nhập để có thể tạo mới.
* Code: đây là trường không bắt buộc, người dùng nhập mã của môn học
* Program: Chương trình học gán với môn học

**Bước 3:** Admin thực hiện ckick button Save để lưu Subject mới

Sau khi click button Save, màn hình sẽ hiển thị message thông báo tạo mới Subject thành công

### 3. Chỉnh sửa một Subject <a href="#id-3.-chinh-sua-mot-course-category" id="id-3.-chinh-sua-mot-course-category"></a>

Để chỉnh sửa Subject đã tạo, Admin thực hiện click vào biểu tượng Action tại Subject muốn chỉnh sửa rồi chọn Edit

<figure><img src="../../.gitbook/assets/image (72).png" alt=""><figcaption></figcaption></figure>

Sau khi chọn Edit, thông tin của Program được hiển thị phía bên phải như ảnh sau:

<figure><img src="../../.gitbook/assets/image (73).png" alt=""><figcaption></figcaption></figure>

Admin thực hiện chỉnh sửa nội dung của Subject gồm các thông tin sau:

* Tên của Subject
* Code: Admin có thể nhập/xóa code của subject
* Program

Sau khi chỉnh sửa nội dung của Subject, Admin thực hiện click Save để lưu thông tin mới. Sau khi click Save, màn hình sẽ hiển thị message thông báo lưu thông tin thành công

> **Lưu ý:**\
> Subject đã gán với khóa học thì không thể xóa

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Subject là môn học thuộc một Program.
* Admin cần chọn đúng Program khi tạo mới hoặc chỉnh sửa Subject.
* Trường **Name** là trường bắt buộc.
* Trường **Code** dùng để định danh Subject, nên đặt ngắn gọn và dễ nhận diện.
* Một Subject có thể được sử dụng để cấu hình Course.
* Subject đã được gán với khóa học thì **không thể xóa**.
* Khi chọn **Delete**, hệ thống cần kiểm tra ràng buộc dữ liệu giữa Subject và Course.
* Nếu Subject đang được sử dụng, Admin nên chỉnh sửa thông tin thay vì xóa.

***

### 💡 Mẹo sử dụng

* Nên đặt tên Subject rõ ràng, đúng tên môn học và thống nhất theo quy chuẩn nội bộ.
* Nên nhập **Code** theo format dễ nhận diện, ví dụ dùng tên viết tắt hoặc slug không dấu.
* Khi danh sách Subject nhiều, nên sử dụng bộ lọc **Program** để thu hẹp phạm vi tìm kiếm.
* Nên kiểm tra kỹ Subject đã được gán vào Course hay chưa trước khi thực hiện xóa.
* Với Subject đã được sử dụng trong khóa học, nên hạn chế chỉnh sửa Program để tránh ảnh hưởng đến việc phân loại Course.
