# Storyline

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

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

![](<../.gitbook/assets/image (455)>)

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

### 3.1. Xem danh sách Storyline

{% stepper %}
{% step %}
## Truy cập màn hình quản lý Storyline

Đường dẫn: Academic Management/ Course & Materials/ Storyline

![](<../.gitbook/assets/image (136)>)

![](<../.gitbook/assets/image (138)>)

Màn hình danh sách Storyline được hiển thị với các thông tin như sau:

| Name                                                                            | Description                                                                 |
| ------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| _Filter_                                                                        |                                                                             |
| Search                                                                          | Tìm kiếm theo tên                                                           |
| Sort by                                                                         | Lọc theo: A-Z, Z-A, Oldest, Lastest                                         |
| From Date                                                                       | Khoảng thời gian lọc: Thời gian bắt đầu lọc                                 |
| To date                                                                         | Khoảng thời gian lọc: Thời gian kết thúc lọc                                |
| _Thông tin hiển thị (thứ tự hiển thị được sắp xếp theo thời gian tạo giảm dần)_ |                                                                             |
| StoryLine name                                                                  | Tên tài liệu                                                                |
| Description                                                                     | Mô tả Storyline                                                             |
| Date                                                                            | <p>Thời gian tạo mới và chỉnh sửa Storyline<br>Format: dd/mm/yyyy hh:mm</p> |
{% endstep %}

{% step %}
## Tìm kiếm Storyline

Người dùng nhập Filter.

Chọn **Search** để hiển thị các danh sách Storyline theo điều kiện Filter.

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách tài liệu theo thời gian tạo.
{% endstep %}
{% endstepper %}

### 3.2. Tạo mới Storyline

{% stepper %}
{% step %}
## Tạo mới Storyline

Tại màn hình danh sách Storyline, ấn nút **Create** để tạo mới Storyline.

![](<../.gitbook/assets/image (140)>)
{% endstep %}

{% step %}
## Nhập thông tin Storyline

Màn hình tạo mới Storyline hiện lên với các thông tin sau, người dùng nhập đầy đủ các thông tin để tạo Storyline.

Step 1: Storyline Info bao gồm các thông tin cơ bản của Storyline.

![](<../.gitbook/assets/image (456)>)

| Name                                                      | Mandatory | Description                                                                     |
| --------------------------------------------------------- | --------- | ------------------------------------------------------------------------------- |
| **Step 1: Storyline Info: Thông tin chung của Storyline** |           |                                                                                 |
| Story Line Name                                           | Yes       | Tên Storyline                                                                   |
| Duration - Hour                                           | No        | <p>Thời gian dự kiến hoàn thành Storyline<br>Hiển thị trên màn LMS học viên</p> |
| Duration - Minutes                                        | No        | <p>Thời gian dự kiến hoàn thành Storyline<br>Hiển thị trên màn LMS học viên</p> |
| Description                                               | Yes       | Mô tả Storyline                                                                 |
{% endstep %}

{% step %}
## Chuyển tới Storyline Content

Ấn nút **Save** để chuyển tới **Step 2: Storyline Content**.

Step 2: Storyline Content bao gồm danh sách các Storyline Item - đơn vị nội dung có trong Storyline.

Màn hình tạo mới Step 2 hiện lên gồm các thông tin sau.

![](<../.gitbook/assets/image (142)>)

| Name                    | Description                                                                                                             |
| ----------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| **Filter**              |                                                                                                                         |
| Search StoryLine Item   | Tìm kiếm theo tên                                                                                                       |
| **List Storyline Item** |                                                                                                                         |
| Order                   | Thứ tự hiển thị của Storyline Item                                                                                      |
| Storyline Item Name     | Tên Storyline Item                                                                                                      |
| Documents               | Số lượng Document có trong Storyline Item                                                                               |
| Action                  | <p>Nút Action bao gồm:<br>- Edit: Chỉnh sửa thông tin Storyline Item<br>- Delete: Xóa Storyline Item khỏi Storyline</p> |
{% endstep %}

{% step %}
## Tạo mới Storyline Item

Tại màn hình Storyline Content, ấn nút “Create Storyline Item” để tạo mới.

![](<../.gitbook/assets/image (145)>)

1.  _**Nhập tên Storyline Item**_

    ![](<../.gitbook/assets/image (146)>)
2. _**Click Save**_
3.  _**Tạo Document**_

    ![](<../.gitbook/assets/image (148)>)

Người dùng chọn Add Document để tạo Document cho Storyline Item, Document gồm 4 loại:

* Text
* Question
* Video
* Interaction
{% endstep %}
{% endstepper %}

#### 3.2.1. Tạo mới Document Text

Sau khi chọn Text, màn hình tạo mới Document Text hiển thị như sau:

![](<../.gitbook/assets/image (150)>)

| Name        | Description                                                                                                                                                   |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Text Name   | <p>Tên của Đoạn văn bản<br><br>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p> |
| Description | Nội dung Content của Text                                                                                                                                     |

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document.

#### 3.2.2. Tạo mới Document Question

Sau khi chọn Question, màn hình tạo mới Document Question hiển thị như sau:

![](<../.gitbook/assets/image (152)>)

| Name          | Description                                                                                                                                              |
| ------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Question Name | <p>Tên của Câu hỏi<br><br>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p> |
| Add Question  | Chọn câu hỏi từ Question List (danh sách tất cả các câu hỏi, bao gồm cả trắc nghiệm và tự luận)                                                          |

Sau khi ấn Add Question, hệ thống hiển thị màn hình chọn Question từ Question list.

Người dùng có thể chọn **1 câu hỏi** trong Question List.

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document.

#### 3.2.3. Tạo mới Document Video

Sau khi chọn Video, màn hình tạo mới Document Video hiển thị như sau:

![](<../.gitbook/assets/image (154)>)

| Name       | Description                                                                                                                                            |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Video Name | <p>Tên của Video<br><br>*Lưu ý: Tên của Document chỉ hiển thị trên hệ thống vận hành Ops, không hiển thị trên giao diện học Storyline của học viên</p> |
| Upload     | Button Upload Video, người dùng có thể chọn Upload Video từ thiết bị của mình hoặc chọn Video có sẵn trên hệ thống                                     |

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document.

#### 3.2.4. Tạo mới Document Interaction

Sau khi chọn **Interaction** từ danh sách Add Documents, trường **Interaction Type** hiển thị với giá trị mặc định là **"Labeled Graphic"**. Màn hình **New Interaction Document** hiển thị như sau:

![](<../.gitbook/assets/image (155)>)

![](<../.gitbook/assets/image (156)>)

| Name             | Mandatory                    | Description                                                                                                             |
| ---------------- | ---------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| Document Name    | Yes                          | <p>Tên Document.<br><br>*Lưu ý: Tên Document chỉ hiển thị trên OPS, không hiển thị trên giao diện học của học viên.</p> |
| Interaction Type | Yes                          | Loại Interaction. Trong giai đoạn này mặc định là **Labeled Graphic**.                                                  |
| Background Image | Yes                          | Ảnh nền để đặt Marker lên. Hỗ trợ định dạng: JPG, JPEG, PNG, GIF, WEBP.                                                 |
| Marker List      | Yes (tối thiểu 1, tối đa 10) | Danh sách Marker đã thêm vào ảnh. Mỗi Marker gồm: Marker Title, Marker Content, Marker Style.                           |

**Cách tạo Marker:**

{% stepper %}
{% step %}
## Upload ảnh nền

Upload ảnh nền thành công.
{% endstep %}

{% step %}
## Chọn vị trí Marker

Click vào vị trí bất kỳ trên ảnh — hệ thống hiển thị icon dấu "+" tại vị trí đó và mở form nhập thông tin Marker trong panel bên trái.

![](<../.gitbook/assets/image (157)>)
{% endstep %}

{% step %}
## Nhập thông tin Marker

| Name           | Mandatory | Description                                                                         |
| -------------- | --------- | ----------------------------------------------------------------------------------- |
| Marker Title   | Yes       | Tiêu đề hiển thị trên popup khi học viên click vào Marker.                          |
| Marker Content | Yes       | Nội dung chi tiết bên trong popup (hỗ trợ text, ảnh). Scroll được nếu nội dung dài. |
| Marker Style   | No        | Chọn icon cho Marker (dấu "+", dấu "?", ...). Nếu không chọn, mặc định là dấu "+".  |
{% endstep %}

{% step %}
## Lưu hoặc hủy Marker

Ấn **Save** để lưu Marker, hoặc **Cancel** để hủy.
{% endstep %}
{% endstepper %}

**Thao tác với Marker đã tạo:**

* **Di chuyển Marker:** Kéo thả trực tiếp icon dấu "+" trên ảnh đến vị trí mới. Vị trí mới được cập nhật ngay lập tức.
* **Chỉnh sửa Marker:** Click icon **Edit (bút chì)** tại Marker tương ứng trong panel danh sách, hoặc click trực tiếp vào icon Marker trên ảnh → form thông tin mở ra → chỉnh sửa Title, Content, Marker Style → ấn **Save** để lưu hoặc **Cancel** để hủy.
* **Xóa Marker:** Click icon **Delete (thùng rác)** tại Marker tương ứng → xác nhận trong dialog _"Bạn có chắc muốn xóa Marker này không?"_ → ấn **Confirm** để xóa. Sau khi xóa, số thứ tự các Marker còn lại được cập nhật lại liên tiếp.

{% hint style="warning" %}
**Lưu ý – Validate khi Save Document:**

* Document Name: bắt buộc, không để trống.
* Background Image: bắt buộc upload trước khi Save.
* Marker List: bắt buộc ít nhất 1 Marker; mỗi Marker phải có đầy đủ Title và Content.
* Nếu vi phạm, hệ thống hiển thị thông báo lỗi ngay dưới field tương ứng và không cho phép Save.
{% endhint %}

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu thông tin Document.

### Lưu Storyline Item

Ấn nút **Save** bên phải góc màn hình để lưu Storyline Item.

![](<../.gitbook/assets/image (158)>)

### Hoàn thành tạo Storyline

Sau khi hoàn thành tạo nội dung Storyline, người dùng ấn nút **Finish** để lưu Storyline.

![](<../.gitbook/assets/image (159)>)

### 3.3. Chỉnh sửa thông tin Storyline

#### 3.3.1. Chỉnh sửa thông tin Storyline

Tại màn hình danh sách Storyline, chọn Storyline hoặc chọn nút Action: **Edit** tại Storyline cần chỉnh sửa.

![](<../.gitbook/assets/image (160)>)

#### 3.3.2. Xóa/Chỉnh sửa thông tin Storyline Item

Tại màn hình List Storyline Item, người dùng có thể thực hiện xóa/chỉnh sửa thông tin bằng cách click vào nút Action tại Storyline Item tương ứng.

![](<../.gitbook/assets/image (161)>)

#### 3.3.3. Xóa/Chỉnh sửa thông tin Document

Tại màn hình Edit Storyline Item, người dùng có thể thực hiện xóa/chỉnh sửa thông tin bằng cách click vào nút Action tại Storyline Item/ Document tương ứng.

![](<../.gitbook/assets/image (162)>)

{% hint style="warning" %}
* Xóa Storyline Item sẽ xóa tất cả các Document có trong Item đó.
* Chỉ có thể xóa/chỉnh sửa thông tin khi Storyline chưa được học. Nếu Storyline đã được học, hệ thống sẽ chặn việc Update thông tin.
{% endhint %}

#### 3.3.4. Sắp xếp thứ tự Storyline Item/Document

**3.3.4.1. Sắp xếp thứ tự Storyline Item**

Tại màn hình Storyline Content, bấm nút: **Reoder** để thực hiện chỉnh sửa thứ tự Storyline Item.

![](<../.gitbook/assets/image (163)>)

Người dùng nhập số thứ tự mới của từng Storyline Item, ấn Save để Lưu thông tin.

![](<../.gitbook/assets/image (164)>)

**3.3.4.2. Sắp xếp thứ tự Document**

Tại màn hình Edit Storyline Item, ấn nút **Enable Drag** để thực hiện Reoder danh sách Document.

![](<../.gitbook/assets/image (165)>)

Người dùng thực hiện kéo thả Document tới vị trí mới.

Sau khi hoàn thành, ấn **Upload** để lưu thông tin thay đổi.

![](<../.gitbook/assets/image (166)>)

### 3.4. Gán Storyline vào Course

{% stepper %}
{% step %}
## Truy cập Course cần add Storyline

Đường dẫn: Academic Management/ Course & Materials/ Storyline
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

{% hint style="warning" %}
* Người dùng cần đăng nhập thành công và có quyền phù hợp để xem, tạo mới, chỉnh sửa hoặc xóa Storyline.
* Storyline được cấu trúc theo 2 cấp chính: **Storyline Item** và **Document**.
* Một Storyline có thể gồm nhiều Storyline Item.
* Một Storyline Item có thể gồm nhiều Document.
* Document trong Storyline Item gồm 4 loại: **Text**, **Question**, **Video** và\*\* Interaction\*\*.
* Document dạng Question được chọn từ **Question List**.
* Document dạng Video có thể được upload từ thiết bị của người dùng hoặc chọn từ video có sẵn trên hệ thống.
{% endhint %}

### 💡 Mẹo sử dụng

{% hint style="info" %}
* Nên đặt tên Storyline rõ ràng theo khóa học, môn học, level hoặc mục đích sử dụng để dễ tìm kiếm.
* Nên nhập mô tả Storyline ngắn gọn nhưng đủ ý để người quản lý nội dung khác hiểu nội dung chính của Storyline.
* Nếu Storyline đã có học viên học, cần cân nhắc kỹ trước khi chỉnh sửa vì hệ thống có thể chặn cập nhật để bảo toàn dữ liệu học tập.
* Khi cần thay đổi thứ tự nội dung, nên dùng chức năng **Reorder** hoặc **Enable Drag** thay vì xóa và tạo lại nội dung.
{% endhint %}
