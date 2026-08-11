# Storyline

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 18, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Storyline** trên hệ thống vận hành **OPS**.

Chức năng **Storyline** cho phép người dùng tạo mới, cấu hình, chỉnh sửa và quản lý nội dung học tập theo định dạng Storyline. Sau khi được tạo, Storyline có thể được gán vào Course để học viên truy cập và học trên hệ thống LMS.

Thông qua chức năng này, Admin có thể xây dựng nội dung học tập gồm nhiều **Storyline Item**, trong đó mỗi Storyline Item có thể chứa các loại Document như **Text**, **Question** hoặc **Video**.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                 | Quyền hạn                                                                            |
| --------- | --------------------------------------- | ------------------------------------------------------------------------------------ |
| SX        | Người tạo và quản lý nội dung Storyline | Có quyền xem, tạo mới, chỉnh sửa, xóa và cấu hình Storyline theo phân quyền được cấp |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Storyline
* **Module liên quan:**
  * Course
  * Question Bank / Question List
  * Resources / Video Library nếu hệ thống sử dụng nguồn video có sẵn
  * LMS học viên

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành OPS.
* Tài khoản người dùng đã được cấp quyền truy cập menu **Storyline**.
* Đối với thao tác xem danh sách, tài khoản cần có quyền xem danh sách Storyline.
* Đối với thao tác tạo mới, tài khoản cần có quyền tạo Storyline.
* Đối với thao tác chỉnh sửa hoặc xóa, tài khoản cần có quyền chỉnh sửa Storyline.
* Đối với thao tác gán Storyline vào Course, tài khoản cần có quyền tạo hoặc chỉnh sửa Course.

## II. Tổng Quan Giao Diện

<figure><img src="../.gitbook/assets/image (143).png" alt=""><figcaption></figcaption></figure>

Màn hình **Storyline** cho phép người dùng xem, tìm kiếm và quản lý danh sách các Storyline đã được tạo trên hệ thống OPS.

Người dùng truy cập chức năng theo đường dẫn:

**Academic Management → Course & Materials → Storyline**

### Các thành phần chính trên màn hình danh sách Storyline

| Khu vực / Thành phần         | Mô tả                                                                                      |
| ---------------------------- | ------------------------------------------------------------------------------------------ |
| **Vùng Filter**              | Cho phép người dùng tìm kiếm và lọc danh sách Storyline.                                   |
| **Search**                   | Tìm kiếm Storyline theo tên.                                                               |
| **Sort by**                  | Sắp xếp danh sách Storyline theo tiêu chí được chọn.                                       |
| **From Date**                | Chọn thời gian bắt đầu để lọc danh sách Storyline.                                         |
| **To Date**                  | Chọn thời gian kết thúc để lọc danh sách Storyline.                                        |
| **Nút Search**               | Áp dụng điều kiện lọc và hiển thị danh sách Storyline tương ứng.                           |
| **Nút Reset**                | Xóa toàn bộ điều kiện tìm kiếm và đưa danh sách về trạng thái mặc định.                    |
| **Nút Create**               | Tạo mới Storyline.                                                                         |
| **Bảng danh sách Storyline** | Hiển thị danh sách Storyline đã được tạo trên hệ thống.                                    |
| **Storyline Name**           | Tên Storyline. Người dùng có thể chọn Storyline để xem hoặc chỉnh sửa thông tin.           |
| **Description**              | Mô tả ngắn nội dung Storyline.                                                             |
| **Date**                     | Hiển thị thời gian tạo mới và chỉnh sửa Storyline theo định dạng dd/mm/yyyy hh:mm.         |
| **Action**                   | Cho phép người dùng thực hiện các thao tác như chỉnh sửa hoặc xóa tùy theo quyền được cấp. |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1. Xem danh sách Storyline <a href="#id-2.1.1.-xem-danh-sach-storyline" id="id-2.1.1.-xem-danh-sach-storyline"></a>

_**Bước 1**_: Truy cập màn hình quản lý Storyline

Đường dẫn: Academic Management/ Course & Materials/ Storyline

<figure><img src="../.gitbook/assets/image (144).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (145).png" alt=""><figcaption></figcaption></figure>

Màn hình danh sách Storyline được hiển thị với các thông tin như sau:

| **Name**                                                                        | **Description**                                                                  |
| ------------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| _Filter_                                                                        |                                                                                  |
| Search                                                                          | Tìm kiếm theo tên                                                                |
| Sort by                                                                         | <p>Lọc theo:</p><ul><li>A-Z</li><li>Z-A</li><li>Oldest</li><li>Lastest</li></ul> |
| From Date                                                                       | Khoảng thời gian lọc: Thời gian bắt đầu lọc                                      |
| To date                                                                         | Khoảng thời gian lọc: Thời gian kết thúc lọc                                     |
| _Thông tin hiển thị (thứ tự hiển thị được sắp xếp theo thời gian tạo giảm dần)_ |                                                                                  |
| StoryLine name                                                                  | Tên tài liệu                                                                     |
| Description                                                                     | Mô tả Storyline                                                                  |
| Date                                                                            | <p>Thời gian tạo mới và chỉnh sửa Storyline</p><p>Format: dd/mm/yyyy hh:mm</p>   |

_**Bước 2**_: Tìm kiếm Storyline

Người dùng nhập Filter

Chọn **Search** để hiển thị các danh sách Storyline theo điều kiện Filter.

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách tài liệu theo thời gian tạo.

### 3.2. Tạo mới Storyline <a href="#id-2.1.2.-tao-moi-storyline" id="id-2.1.2.-tao-moi-storyline"></a>

_**Bước 1**_: Tại màn hình danh sách Storyline, ấn nút **Create** để tạo mới Storyline

<figure><img src="../.gitbook/assets/image (146).png" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: Màn hình tạo mới Storyline hiện lên với các thông tin sau, người dùng nhập đầy đủ các thông tin để tạo Storyline

Step 1: Storyline Info bao gồm các thông tin cơ bản của Storyline

<figure><img src="../.gitbook/assets/image (147).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin:

| **Name**                                                  | **Mandatory** | **Description**                                                                    |
| --------------------------------------------------------- | ------------- | ---------------------------------------------------------------------------------- |
| **Step 1: Storyline Info: Thông tin chung của Storyline** |               |                                                                                    |
| Story Line Name                                           | Yes           | Tên Storyline                                                                      |
| Duration - Hour                                           | No            | <p>Thời gian dự kiến hoàn thành Storyline</p><p>Hiển thị trên màn LMS học viên</p> |
| Duration - Minutes                                        | No            | <p>Thời gian dự kiến hoàn thành Storyline</p><p>Hiển thị trên màn LMS học viên</p> |
| Description                                               | Yes           | Mô tả Storyline                                                                    |

_**Bước 3**_: Ấn nút **Save** để chuyển tới **Step 2: Storyline Content**

Step 2: Storyline Content bao gồm danh sách các Storyline Item - đơn vị nội dung có trong Storyline

Màn hình tạo mới Step 2 hiện lên gồm các thông tin sau

<figure><img src="../.gitbook/assets/image (148).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin:

| **Name**                | **Description**                                                                                                                        |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| **Filter**              |                                                                                                                                        |
| Search StoryLine Item   | Tìm kiếm theo tên                                                                                                                      |
| **List Storyline Item** |                                                                                                                                        |
| Order                   | Thứ tự hiển thị của Storyline Item                                                                                                     |
| Storyline Item Name     | Tên Storyline Item                                                                                                                     |
| Documents               | Số lượng Document có trong Storyline Item                                                                                              |
| Action                  | <p>Nút Action bao gồm:</p><ul><li>Edit: Chỉnh sửa thông tin Storyline Item</li><li>Delete: Xóa Storyline Item khỏi Storyline</li></ul> |

_**Bước 4**_: Tạo mới **Storyline Item**

Tại màn hình Storyline Content, ấn nút “Create Storyline Item” để tạo mới

<figure><img src="../.gitbook/assets/image (149).png" alt=""><figcaption></figcaption></figure>

1. _**Nhập tên Storyline Item**_

<figure><img src="../.gitbook/assets/image (150).png" alt=""><figcaption></figcaption></figure>

2. _**Click Save**_
3. _**Tạo Document**_

<figure><img src="../.gitbook/assets/image (858).png" alt=""><figcaption></figcaption></figure>

Người dùng chọn Add Document để tạo Document cho Storyline Item, Document gồm 4 loại:

* Text
* Question
* Video
* Interaction

_**3.2.1. Tạo mới Document Text**_

Sau khi chọn Text, màn hình tạo mới Document Text hiển thị như sau:

<figure><img src="../.gitbook/assets/image (152).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin:

| **Name**    | **Description**                                                                                                                                              |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Text Name   | <p>Tên của Đoạn văn bản</p><p>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p> |
| Description | Nội dung Content của Text                                                                                                                                    |

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document

_**3.2.2. Tạo mới Document Question**_

Sau khi chọn Question, màn hình tạo mới Document Question hiển thị như sau:

<figure><img src="../.gitbook/assets/image (153).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin:

| **Name**      | **Description**                                                                                                                                                                                                                                                             |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Question Name | <p>Tên của Câu hỏi</p><p>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p>                                                                                                                     |
| Add Question  | <p>Chọn câu hỏi từ Question List (danh sách tất cả các câu hỏi, bao gồm cả trắc nghiệm và tự luận)</p><p>Sau khi ấn Add Question, hệ thống hiển thị màn hình chọn Question từ Question list</p><p>Người dùng có thể chọn <strong>1 câu hỏi</strong> trong Question List</p> |

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document

_**3.2.3. Tạo mới Document Video**_

Sau khi chọn Video, màn hình tạo mới Document Video hiển thị như sau:

<figure><img src="../.gitbook/assets/image (154).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin:

| **Name**   | **Description**                                                                                                                                       |
| ---------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Video Name | <p>Tên của Video</p><p>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p> |
| Upload     | Button Upload Video, người dùng có thể chọn Upload Video từ thiết bị của mình hoặc chọn Video có sẵn trên hệ thống                                    |

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document

_**3.2.4. Tạo mới Document Interaction**_

Sau khi chọn **Interaction** từ danh sách Add Documents, trường **Interaction Type** hiển thị với giá trị mặc định là **"Labeled Graphic"**. Màn hình **New Interaction Document** hiển thị như sau:

<figure><img src="../.gitbook/assets/image (860).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (861).png" alt=""><figcaption></figcaption></figure>

Mô tả thông tin cấu hình:

| **Name**         | **Mandatory**                | **Description**                                                                                                        |
| ---------------- | ---------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Document Name    | Yes                          | <p>Tên Document.</p><p>*Lưu ý: Tên Document chỉ hiển thị trên OPS, không hiển thị trên giao diện học của học viên.</p> |
| Interaction Type | Yes                          | Loại Interaction. Trong giai đoạn này mặc định là **Labeled Graphic**.                                                 |
| Background Image | Yes                          | Ảnh nền để đặt Marker lên. Hỗ trợ định dạng: JPG, JPEG, PNG, GIF, WEBP.                                                |
| Marker List      | Yes (tối thiểu 1, tối đa 10) | Danh sách Marker đã thêm vào ảnh. Mỗi Marker gồm: Marker Title, Marker Content, Marker Style.                          |

_**Cách tạo Marker:**_

1. Upload ảnh nền thành công.
2. Click vào vị trí bất kỳ trên ảnh — hệ thống hiển thị icon dấu "+" tại vị trí đó và mở form nhập thông tin Marker trong panel bên trái.

<figure><img src="../.gitbook/assets/image (862).png" alt=""><figcaption></figcaption></figure>

3. Nhập thông tin Marker:

| **Name**       | **Mandatory** | **Description**                                                                     |
| -------------- | ------------- | ----------------------------------------------------------------------------------- |
| Marker Title   | Yes           | Tiêu đề hiển thị trên popup khi học viên click vào Marker.                          |
| Marker Content | Yes           | Nội dung chi tiết bên trong popup (hỗ trợ text, ảnh). Scroll được nếu nội dung dài. |
| Marker Style   | No            | Chọn icon cho Marker (dấu "+", dấu "?", ...). Nếu không chọn, mặc định là dấu "+".  |

4. Ấn **Save** để lưu Marker, hoặc **Cancel** để hủy.

_**Thao tác với Marker đã tạo:**_

* **Di chuyển Marker:** Kéo thả trực tiếp icon dấu "+" trên ảnh đến vị trí mới. Vị trí mới được cập nhật ngay lập tức.
* **Chỉnh sửa Marker:** Click icon **Edit (bút chì)** tại Marker tương ứng trong panel danh sách, hoặc click trực tiếp vào icon Marker trên ảnh → form thông tin mở ra → chỉnh sửa Title, Content, Marker Style → ấn **Save** để lưu hoặc **Cancel** để hủy.
* **Xóa Marker:** Click icon **Delete (thùng rác)** tại Marker tương ứng → xác nhận trong dialog _"Bạn có chắc muốn xóa Marker này không?"_ → ấn **Confirm** để xóa. Sau khi xóa, số thứ tự các Marker còn lại được cập nhật lại liên tiếp.

{% hint style="info" %}
**Lưu ý – Validate khi Save Document:**

* Document Name: bắt buộc, không để trống.
* Background Image: bắt buộc upload trước khi Save.
* Marker List: bắt buộc ít nhất 1 Marker; mỗi Marker phải có đầy đủ Title và Content.
* Nếu vi phạm, hệ thống hiển thị thông báo lỗi ngay dưới field tương ứng và không cho phép Save.

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document.
{% endhint %}

4. _**Lưu Storyline Item**_

Ấn nút **Save** bên phải góc màn hình để lưu Storyline Item

<figure><img src="../.gitbook/assets/image (155).png" alt=""><figcaption></figcaption></figure>

_**Bước 5:**_ Lưu **Storyline Item**

Sau khi hoàn thành tạo nội dung Storyline, người dùng ấn nút **Finish** để lưu Storyline

<figure><img src="../.gitbook/assets/image (156).png" alt=""><figcaption></figcaption></figure>

### 3.3. Chỉnh sửa thông tin Storyline <a href="#id-2.1.3.-chinh-sua-thong-tin-storyline" id="id-2.1.3.-chinh-sua-thong-tin-storyline"></a>

**3.3.1. Chỉnh sửa thông tin Storyline**

Tại màn hình danh sách Storyline, chọn Storyline hoặc chọn nút Action: **Edit** tại Storyline cần chỉnh sửa

<figure><img src="../.gitbook/assets/image (157).png" alt=""><figcaption></figcaption></figure>

**3.3.2. Xóa/Chỉnh sửa thông tin Storyline Item**

Tại màn hình List Storyline Item, người dùng có thể thực hiện xóa/chỉnh sửa thông tin bằng cách click vào nút Action tại Storyline Item tương ứng

<figure><img src="../.gitbook/assets/image (158).png" alt=""><figcaption></figcaption></figure>

**3.3.3. Xóa/Chỉnh sửa thông tin Document**

Tại màn hình Edit Storyline Item, người dùng có thể thực hiện xóa/chỉnh sửa thông tin bằng cách click vào nút Action tại Storyline Item/ Document tương ứng

<figure><img src="../.gitbook/assets/image (159).png" alt=""><figcaption></figcaption></figure>

\*Lưu ý:

* Xóa Storyline Item sẽ xóa tất cả các Document có trong Item đó
* Chỉ có thể xóa/chỉnh sửa thông tin khi Storyline chưa được học. Nếu Storyline đã được học, hệ thống sẽ chặn việc Update thông tin

_**3.3.4. Sắp xếp thứ tự Storyline Item/Document**_

_**3.3.4.1. Sắp xếp thứ tự Storyline Item**_

Tại màn hình Storyline Content, bấm nút: **Reoder** để thực hiện chỉnh sửa thứ tự Storyline Item

<figure><img src="../.gitbook/assets/image (160).png" alt=""><figcaption></figcaption></figure>

Người dùng nhập số thứ tự mới của từng Storyline Item, ấn Save để Lưu thông tin

<figure><img src="../.gitbook/assets/image (161).png" alt=""><figcaption></figcaption></figure>

_**3.3.4.2. Sắp xếp thứ tự Document**_

Tại màn hình Edit Storyline Item, ấn nút **Enable Drag** để thực hiện Reoder danh sách Document

<figure><img src="../.gitbook/assets/image (162).png" alt=""><figcaption></figcaption></figure>

Người dùng thực hiện kéo thả Document tới vị trí mới

Sau khi hoàn thành, ấn **Upload** để lưu thông tin thay đổi

<figure><img src="../.gitbook/assets/image (163).png" alt=""><figcaption></figcaption></figure>

### _**3.4. Gán Storyline vào Course**_ <a href="#id-2.2.-gan-storyline-vao-course" id="id-2.2.-gan-storyline-vao-course"></a>

_**Bước 1**_: Truy cập Course cần add Storyline

Đường dẫn: Academic Management/ Course & Materials/ Storyline

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Người dùng cần đăng nhập thành công và có quyền phù hợp để xem, tạo mới, chỉnh sửa hoặc xóa Storyline.
* Storyline được cấu trúc theo 2 cấp chính: **Storyline Item** và **Document**.
* Một Storyline có thể gồm nhiều Storyline Item.
* Một Storyline Item có thể gồm nhiều Document.
* Document trong Storyline Item gồm 4 loại: **Text**, **Question**, **Video** và **Interaction**.
* Document dạng Question được chọn từ **Question List**.
* Document dạng Video có thể được upload từ thiết bị của người dùng hoặc chọn từ video có sẵn trên hệ thống.

### 💡 Mẹo sử dụng

* Nên đặt tên Storyline rõ ràng theo khóa học, môn học, level hoặc mục đích sử dụng để dễ tìm kiếm.
* Nên nhập mô tả Storyline ngắn gọn nhưng đủ ý để người quản lý nội dung khác hiểu nội dung chính của Storyline.
* Nếu Storyline đã có học viên học, cần cân nhắc kỹ trước khi chỉnh sửa vì hệ thống có thể chặn cập nhật để bảo toàn dữ liệu học tập.
* Khi cần thay đổi thứ tự nội dung, nên dùng chức năng **Reorder** hoặc **Enable Drag** thay vì xóa và tạo lại nội dung.
