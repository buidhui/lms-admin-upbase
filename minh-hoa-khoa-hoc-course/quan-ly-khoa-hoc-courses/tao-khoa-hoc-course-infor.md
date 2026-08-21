# Tạo khóa học (Course Infor)

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 20, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn Admin cách tạo mới khóa học tại bước **Course Info** trên hệ thống vận hành **OPS**.

Bước **Course Info** là bước đầu tiên trong quy trình tạo khóa học, dùng để khai báo các thông tin tổng quan của khóa học như tên khóa học, mã khóa học, chương trình, môn học, loại khóa học, điểm đạt chứng chỉ và tỷ trọng điểm của từng thành phần đánh giá.

***

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                     | Quyền hạn                                                           |
| --------- | ------------------------------------------- | ------------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành khóa học            | Có quyền tạo mới khóa học và khai báo thông tin Course Info         |
| SX        | Người phụ trách học thuật/nội dung khóa học | Có quyền nhập, kiểm tra và quản lý thông tin học thuật của khóa học |

***

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Create Course
* **Bước thực hiện:** Course Info
* **Module liên quan:**
  * Program Category
  * Subject Category
  * Course Content
  * Resources
  * Certificates
  * Class

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản người dùng có quyền truy cập menu **Course 4 Level**.
* Tài khoản người dùng có quyền tạo mới khóa học.
* Hệ thống đã có dữ liệu **Program** để Admin lựa chọn.
* Hệ thống đã có dữ liệu **Subject** tương ứng với Program.
* Trường hợp tạo **Normal Course** và muốn cấu hình khóa học nền tảng đi kèm, hệ thống cần có sẵn các **Foundation Course** tương ứng theo level.

***

## II. Tổng Quan Giao Diện

<figure><img src="../../.gitbook/assets/image (206).png" alt=""><figcaption></figcaption></figure>

Màn hình **Course Info** là bước đầu tiên trong quy trình tạo khóa học. Tại màn hình này, Admin nhập các thông tin tổng quan để hệ thống tạo mới bản ghi khóa học.

Người dùng truy cập chức năng theo đường dẫn:

**Academic Management → Course & Materials → Course 4 Level → Create Course**

Sau khi chọn **Create Course**, hệ thống hiển thị màn hình thông tin chung của khóa học (Course infor) bao gồm các thông tin sau:

| Khu vực / Thành phần   | Mô tả                                                           |
| ---------------------- | --------------------------------------------------------------- |
| **General**            | Khu vực nhập thông tin chung của khóa học.                      |
| **Course Name**        | Tên khóa học.                                                   |
| **Describe**           | Mô tả khóa học.                                                 |
| **Code**               | Mã khóa học. Mã này dùng để định danh khóa học trên hệ thống.   |
| **Tag**                | Tag dùng để phân loại, tìm kiếm hoặc gắn nhãn khóa học.         |
| **Program (Category)** | Chương trình học/nhóm chương trình mà khóa học thuộc về.        |
| **Subject**            | Môn học của khóa học.                                           |
| **Type**               | Loại khóa học.                                                  |
| **Pass Point**         | Điểm tối thiểu học viên cần đạt để đủ điều kiện nhận chứng chỉ. |
| **Score Components**   | Khu vực nhập tỷ trọng điểm của các thành phần đánh giá.         |
| **Save**               | Lưu thông tin Course Info và tạo khóa học mới.                  |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Truy cập màn hình tạo mới khóa học

_**Bước 1:**_ Admin truy cập **Academic Management → Course & Materials → Course 4 Level**

Hệ thống hiển thị màn hình danh sách khóa học.

<figure><img src="../../.gitbook/assets/image (207).png" alt=""><figcaption></figcaption></figure>

_**Bước 2:**_ Tại màn hình danh sách khóa học, Admin chọn **Create Course**.

Lúc này, hệ thống chuyển đến bước **Course Info.**

<figure><img src="../../.gitbook/assets/image (208).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (209).png" alt=""><figcaption></figcaption></figure>

***

### 3.2 Nhập thông tin chung của khóa học

_**Bước 3:**_ Admin cần nhập Tên khóa học (**Course** **Name)**. Đây là trường bắt buộc dùng để hiển thị tên khóa học trên hệ thống và hiển thị cho học viên tại LMS.

<figure><img src="../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>

_**Bước 4:**_ Admin nhập mô tả khóa học (**Describe)**. Trường này dùng để mô tả nội dung hoặc mục tiêu chính của khóa học.

<figure><img src="../../.gitbook/assets/image (29).png" alt=""><figcaption></figcaption></figure>

_**Bước 5:**_ Admin nhập mã khóa học (**Code)**. Đây là trường bắt buộc. Hệ thống không cho phép lưu nếu mã khóa học trùng với mã đã tồn tại.

<figure><img src="../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>

_**Bước 6:**_ Nhập hoặc chọn **Tag**. Admin có thể tạo tag mới bằng cách nhập nội dung tag.

<figure><img src="../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

_**Bước 7:**_ Admin chọn **Program (Category)** từ danh sách hiển thị. Đây là trường bắt buộc, nhờ vào trường này, hệ thống mới xác định được chương trình học và từ đó cho phép admin chọn môn học tương ứng.

<figure><img src="../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

_**Bước 8:**_ Admin chọn hoặc nhập **Subject** tương ứng với Program đã chọn.

<figure><img src="../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>

_**Bước 9:**_ Admin chọn **Type** của khóa học. Hệ thống hỗ trợ các loại khóa học: **Foundation Course**, **Trial Course**, **Practice Course** và **Normal Course**.

<figure><img src="../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

***

### 3.3 Cấu hình thông tin theo loại khóa học

#### Trường hợp 1: Type = Foundation Course

<figure><img src="../../.gitbook/assets/image (177).png" alt=""><figcaption></figcaption></figure>

_**Bước 10.1:**_ Khi Admin chọn **Foundation Course**, hệ thống hiển thị danh sách checkbox level của khóa học.

Admin cần chọn ít nhất **01 level**.

Ví dụ level có thể bao gồm các mức như IA, IB, IIA, IIB tùy theo cấu hình hệ thống.

#### Trường hợp 2: Type = Normal Course

<figure><img src="../../.gitbook/assets/image (178).png" alt=""><figcaption></figcaption></figure>

_**Bước 10.2:**_ Khi Admin chọn **Normal Course**, hệ thống hiển thị danh sách combobox các khóa học **Foundation Course** theo từng level.

Admin có thể:

* Nhập ký tự để tìm kiếm khóa học Foundation đã tạo với level tương ứng.
* Chọn hoặc không chọn khóa học Foundation cho từng level.

Theo tài liệu gốc, với Normal Course, Admin có thể không chọn bất kỳ khóa học Foundation nào cho cả 4 level.

#### Trường hợp 3: Type = Trial Course hoặc Practice Course

_**Bước 10.3:**_ Với **Trial Course** hoặc **Practice Course**, Admin chỉ cần chọn loại khóa học tương ứng và tiếp tục nhập các thông tin còn lại của Course Info.

***

### 3.4 Nhập Pass Point

<figure><img src="../../.gitbook/assets/image (179).png" alt=""><figcaption></figcaption></figure>

_**Bước 11:**_ Admin nhập **Pass Point**. Đây là trường bắt buộc. Pass Point là mức điểm yêu cầu mà học viên phải đạt để có thể nhận được chứng chỉ của khóa học.

***

### 3.5 Nhập điểm các thành phần

<figure><img src="../../.gitbook/assets/image (180).png" alt=""><figcaption></figcaption></figure>

_**Bước 12:**_ Admin nhập hệ số điểm cho từng thành phần:

| Thành phần       | Bắt buộc | Ghi chú                                   |
| ---------------- | -------- | ----------------------------------------- |
| **Tiến độ học**  | Y        | Nhập tỷ trọng điểm cho tiến độ học.       |
| **Graded Quiz**  | Y        | Nhập tỷ trọng điểm cho quiz có tính điểm. |
| **Chapter Test** | Y        | Nhập tỷ trọng điểm cho Chapter Test.      |
| **Topic Test**   | Y        | Nhập tỷ trọng điểm cho Topic Test.        |
| **Mid Test**     | Y        | Nhập tỷ trọng điểm cho Mid Test.          |
| **Final Test**   | Y        | Nhập tỷ trọng điểm cho Final Test.        |

Tổng hệ số điểm của tất cả thành phần phải bằng **100**.

***

### 3.6 Lưu Course Info

_**Bước 13:**_ Admin chọn **Save**. Lúc này, hệ thống lưu thông tin đã nhập và tạo khóa học mới.

Sau khi lưu thành công, Admin có thể tiếp tục chuyển sang bước tiếp theo trong quy trình tạo khóa học.

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Course Info là bước đầu tiên trong quy trình tạo khóa học.
* Các trường có dấu **(\*)** là trường bắt buộc.
* **Code** là mã định danh khóa học và không được trùng với mã khóa học đã tồn tại.
* **Program / Category** và **Subject** cần được chọn đúng để đảm bảo khóa học được phân loại chính xác.
* **Type** là trường bắt buộc và ảnh hưởng đến các thông tin cần cấu hình tiếp theo.
* Nếu chọn **Foundation Course**, Admin bắt buộc phải chọn ít nhất một level.
* Nếu chọn **Normal Course**, hệ thống hiển thị danh sách Foundation Course theo từng level để Admin có thể cấu hình khóa học nền tảng đi kèm.
* Với **Normal Course**, Admin có thể không chọn Foundation Course cho cả 4 level.
* **Pass Point** là trường bắt buộc, dùng để xác định điều kiện điểm để học viên được nhận chứng chỉ.
* Tổng điểm các thành phần bắt buộc phải bằng **100**.
* Sau khi nhập đầy đủ thông tin, Admin cần chọn **Save** để lưu Course Info và tạo khóa học mới.

***

### 💡 Mẹo sử dụng

* Nên chọn đúng **Program** trước khi chọn **Subject** để đảm bảo môn học thuộc đúng chương trình
* Với **Normal Course**, nếu cần thiết lập điều kiện học nền tảng, nên tạo sẵn các Foundation Course trước.
* Nên kiểm tra kỹ tổng tỷ trọng điểm trước khi bấm **Save**.
* Nếu khóa học chưa chắc chắn cấu hình điểm, nên thống nhất quy tắc tính điểm nội bộ trước khi tạo Course Info.
