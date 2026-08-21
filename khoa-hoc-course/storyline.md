# Storyline

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** SX

**Đường dẫn:** Academic Management → Course & Materials → Storyline

#### Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Storyline
* **Module liên quan:** Course, Question Bank / Question List, Resources / LMS học viên

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống vận hành **OPS**.
* Tài khoản đã được cấp quyền truy cập menu **Storyline**.
* Xem danh sách: cần quyền xem danh sách Storyline.
* Tạo mới: cần quyền tạo Storyline.
* Chỉnh sửa/xóa: cần quyền chỉnh sửa Storyline.
* Gán Storyline vào Course: cần quyền tạo hoặc chỉnh sửa Course.

## II. Hướng dẫn chi tiết

### Xem danh sách Storyline

{% stepper %}
{% step %}
## Truy cập màn hình quản lý Storyline

Đường dẫn: Academic Management / Course & Materials / Storyline.

![](<../.gitbook/assets/image (136)>)

Danh sách Storyline hiển thị theo thời gian tạo giảm dần.

![](<../.gitbook/assets/image (138)>)

Các thông tin hiển thị trên màn hình danh sách:

| Name                                                       | Description                                                        |
| ---------------------------------------------------------- | ------------------------------------------------------------------ |
| _Filter_                                                   |                                                                    |
| Search                                                     | Tìm kiếm theo tên                                                  |
| Sort by                                                    | Lọc theo: A-Z, Z-A, Oldest, Lastest                                |
| From Date                                                  | Khoảng thời gian lọc: Thời gian bắt đầu lọc                        |
| To Date                                                    | Khoảng thời gian lọc: Thời gian kết thúc lọc                       |
| _Thông tin hiển thị (sắp xếp theo thời gian tạo giảm dần)_ |                                                                    |
| StoryLine Name                                             | Tên tài liệu                                                       |
| Description                                                | Mô tả Storyline                                                    |
| Date                                                       | Thời gian tạo mới và chỉnh sửa Storyline. Format: dd/mm/yyyy hh:mm |
{% endstep %}

{% step %}
## Tìm kiếm Storyline

Người dùng nhập Filter.

* Chọn **Search** để hiển thị danh sách Storyline theo điều kiện Filter.
* Chọn **Reset** để xóa tất cả giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo.
{% endstep %}
{% endstepper %}

### Tạo mới Storyline

{% stepper %}
{% step %}
## Chọn Create để tạo mới Storyline

Tại màn hình danh sách Storyline, ấn nút **Create**.

![](<../.gitbook/assets/image (140)>)
{% endstep %}

{% step %}
## Storyline Info — nhập thông tin cơ bản

| Name               | Mandatory | Description                                                            |
| ------------------ | --------- | ---------------------------------------------------------------------- |
| Story Line Name    | Yes       | Tên Storyline                                                          |
| Duration - Hour    | No        | Thời gian dự kiến hoàn thành Storyline. Hiển thị trên màn LMS học viên |
| Duration - Minutes | No        | Thời gian dự kiến hoàn thành Storyline. Hiển thị trên màn LMS học viên |
| Description        | Yes       | Mô tả Storyline                                                        |
{% endstep %}

{% step %}
## Storyline Content — danh sách Storyline Item

Ấn nút **Save** để chuyển tới màn hình Storyline Content, hiển thị danh sách các Storyline Item.

![](<../.gitbook/assets/image (142)>)

| Name                    | Description                                                                                             |
| ----------------------- | ------------------------------------------------------------------------------------------------------- |
| **Filter**              |                                                                                                         |
| Search StoryLine Item   | Tìm kiếm theo tên                                                                                       |
| **List Storyline Item** |                                                                                                         |
| Order                   | Thứ tự hiển thị của Storyline Item                                                                      |
| Storyline Item Name     | Tên Storyline Item                                                                                      |
| Documents               | Số lượng Document có trong Storyline Item                                                               |
| Action                  | Nút Action bao gồm: Edit: Chỉnh sửa thông tin Storyline Item; Delete: Xóa Storyline Item khỏi Storyline |
{% endstep %}

{% step %}
## Tạo mới Storyline Item và Document

Tại màn hình Storyline Content, ấn **Create Storyline Item**.

![](<../.gitbook/assets/image (145)>)

Nhập tên Storyline Item → **Save**.

![](<../.gitbook/assets/image (146)>)

Chọn **Add Document** để tạo Document cho Storyline Item. Document gồm 4 loại: **Text**, **Question**, **Video**, **Interaction**.

![](<../.gitbook/assets/image (148)>)

#### Text

| Name        | Description                                                                                                                 |
| ----------- | --------------------------------------------------------------------------------------------------------------------------- |
| Text Name   | Tên của Đoạn văn bản. _Lưu ý: Tên Document chỉ hiển thị trên Ops, không hiển thị trên giao diện học Storyline của học viên_ |
| Description | Nội dung Content của Text                                                                                                   |

![](<../.gitbook/assets/image (150)>)

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu.

#### Question

| Name        | Description                                                                                                                 |
| ----------- | --------------------------------------------------------------------------------------------------------------------------- |
| Text Name   | Tên của Đoạn văn bản. _Lưu ý: Tên Document chỉ hiển thị trên Ops, không hiển thị trên giao diện học Storyline của học viên_ |
| Description | Nội dung Content của Text                                                                                                   |

![](<../.gitbook/assets/image (152)>)

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu.

#### Video

| Name       | Description                                                                                                |
| ---------- | ---------------------------------------------------------------------------------------------------------- |
| Video Name | Tên của Video. _Lưu ý: Tên Document chỉ hiển thị trên Ops, không hiển thị trên giao diện học của học viên_ |
| Upload     | Button Upload Video: chọn Upload từ thiết bị hoặc chọn Video có sẵn trên hệ thống                          |

![](<../.gitbook/assets/image (154)>)

Sau khi nhập đủ thông tin, ấn **Save Document** để lưu.

#### Interaction

Sau khi chọn **Interaction**, trường **Interaction Type** mặc định là **"Labeled Graphic"**. Màn hình **New Interaction Document** hiển thị như sau:

![](<../.gitbook/assets/image (155)>)

![](<../.gitbook/assets/image (156)>)

| Name             | Mandatory                    | Description                                                                                                |
| ---------------- | ---------------------------- | ---------------------------------------------------------------------------------------------------------- |
| Document Name    | Yes                          | Tên Document. _Lưu ý: Tên Document chỉ hiển thị trên OPS, không hiển thị trên giao diện học của học viên._ |
| Interaction Type | Yes                          | Loại Interaction. Giai đoạn này mặc định là **Labeled Graphic**.                                           |
| Background Image | Yes                          | Ảnh nền để đặt Marker. Hỗ trợ: JPG, JPEG, PNG, GIF, WEBP.                                                  |
| Marker List      | Yes (tối thiểu 1, tối đa 10) | Danh sách Marker đã thêm vào ảnh. Mỗi Marker gồm: Marker Title, Marker Content, Marker Style.              |

**Cách tạo Marker:** Upload ảnh nền thành công → click vào vị trí bất kỳ trên ảnh, hệ thống hiển thị icon dấu "+" và mở form nhập thông tin Marker ở panel bên trái.

![](<../.gitbook/assets/image (157)>)

| Name           | Mandatory | Description                                                                         |
| -------------- | --------- | ----------------------------------------------------------------------------------- |
| Marker Title   | Yes       | Tiêu đề hiển thị trên popup khi học viên click vào Marker.                          |
| Marker Content | Yes       | Nội dung chi tiết bên trong popup (hỗ trợ text, ảnh). Scroll được nếu nội dung dài. |
| Marker Style   | No        | Chọn icon cho Marker (dấu "+", dấu "?", ...). Mặc định là dấu "+".                  |

Ấn **Save** để lưu Marker, hoặc **Cancel** để hủy.

**Thao tác với Marker đã tạo:**

* **Di chuyển:** Kéo thả icon dấu "+" trên ảnh đến vị trí mới, cập nhật ngay lập tức.
* **Chỉnh sửa:** Click icon **Edit (bút chì)** trong panel danh sách hoặc click trực tiếp icon Marker trên ảnh → chỉnh sửa Title, Content, Marker Style → **Save**/**Cancel**.
* **Xóa:** Click icon **Delete (thùng rác)** → xác nhận _"Bạn có chắc muốn xóa Marker này không?"_ → **Confirm**. Sau khi xóa, số thứ tự các Marker còn lại được cập nhật lại liên tiếp.

{% hint style="warning" %}
**Lưu ý – Validate khi Save Document:**

* Document Name: bắt buộc, không để trống.
* Background Image: bắt buộc upload trước khi Save.
* Marker List: bắt buộc ít nhất 1 Marker; mỗi Marker phải có đầy đủ Title và Content.
* Nếu vi phạm, hệ thống hiển thị lỗi ngay dưới field tương ứng và không cho phép Save.
{% endhint %}

Lưu Storyline Item: ấn nút **Save** ở góc phải màn hình.

![](<../.gitbook/assets/image (158)>)
{% endstep %}

{% step %}
## Hoàn tất Storyline

Sau khi hoàn thành tạo nội dung, ấn nút **Finish** để lưu Storyline.

![](<../.gitbook/assets/image (159)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin Storyline

{% stepper %}
{% step %}
## Chỉnh sửa thông tin Storyline

Tại màn hình danh sách Storyline, chọn Storyline hoặc chọn Action: **Edit** tại Storyline cần chỉnh sửa.

![](<../.gitbook/assets/image (160)>)
{% endstep %}

{% step %}
## Xóa/Chỉnh sửa Storyline Item

Tại màn hình List Storyline Item, click nút Action tại Storyline Item tương ứng để xóa/chỉnh sửa.

![](<../.gitbook/assets/image (161)>)
{% endstep %}

{% step %}
## Xóa/Chỉnh sửa Document

Tại màn hình Edit Storyline Item, click nút Action tại Storyline Item / Document tương ứng để xóa/chỉnh sửa.

![](<../.gitbook/assets/image (162)>)

{% hint style="warning" %}
* Xóa Storyline Item sẽ xóa tất cả các Document trong Item đó.
* Chỉ có thể xóa/chỉnh sửa khi Storyline chưa được học. Nếu Storyline đã được học, hệ thống sẽ chặn việc Update.
{% endhint %}
{% endstep %}

{% step %}
## Sắp xếp thứ tự Storyline Item

Tại màn hình Storyline Content, bấm nút **Reorder** để chỉnh sửa thứ tự Storyline Item.

![](<../.gitbook/assets/image (163)>)

Nhập số thứ tự mới của từng Storyline Item, ấn **Save** để lưu.

![](<../.gitbook/assets/image (164)>)
{% endstep %}

{% step %}
## Sắp xếp thứ tự Document

Tại màn hình Edit Storyline Item, ấn nút **Enable Drag** để Reorder danh sách Document.

![](<../.gitbook/assets/image (165)>)

Kéo thả Document tới vị trí mới, sau đó ấn **Upload** để lưu thay đổi.

![](<../.gitbook/assets/image (166)>)
{% endstep %}
{% endstepper %}

### Gán Storyline vào Course

{% stepper %}
{% step %}
## Truy cập Course cần add Storyline

Đường dẫn: Academic Management / Course & Materials / Course 4 Level / Truy cập vào course cần add Storyline.

![](<../.gitbook/assets/image (167)>)
{% endstep %}

{% step %}
## Truy cập vào Course Contect, tại UNIT cần add Storyline, chọn "Storyline"

![](<../.gitbook/assets/image (168)>)

Hệ thống hiển thị giao diện add storyline cho khóa học.

![](<../.gitbook/assets/image (169)>)
{% endstep %}

{% step %}
## Nhập thông tin và chọn Storyline mong muốn

![](<../.gitbook/assets/image (170)>)
{% endstep %}

{% step %}
## Ấn Save để lưu thông tin Storyline

![](<../.gitbook/assets/image (171)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần đăng nhập thành công và có quyền phù hợp để xem, tạo mới, chỉnh sửa hoặc xóa Storyline.
2. Storyline được cấu trúc theo 2 cấp chính: **Storyline Item** và **Document**.
3. Một Storyline có thể gồm nhiều Storyline Item; một Storyline Item có thể gồm nhiều Document.
4. Document trong Storyline Item gồm 4 loại: **Text**, **Question**, **Video** và **Interaction**.
5. Document dạng Question được chọn từ **Question List**.
6. Document dạng Video có thể upload từ thiết bị hoặc chọn từ video có sẵn trên hệ thống.
7. Xóa Storyline Item sẽ xóa toàn bộ Document trong Item đó.
8. Chỉ chỉnh sửa/xóa được khi Storyline chưa được học; nếu đã được học, hệ thống chặn cập nhật.

#### Mẹo sử dụng

1. Nên đặt tên Storyline rõ ràng theo khóa học, môn học, level hoặc mục đích sử dụng để dễ tìm kiếm.
2. Nên nhập mô tả ngắn gọn nhưng đủ ý để người quản lý nội dung khác hiểu nội dung chính.
3. Nếu Storyline đã có học viên học, cần cân nhắc kỹ trước khi chỉnh sửa vì hệ thống có thể chặn cập nhật để bảo toàn dữ liệu học tập.
4. Khi cần thay đổi thứ tự nội dung, nên dùng **Reorder** hoặc **Enable Drag** thay vì xóa và tạo lại.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                          | Nguyên nhân                                                              | Cách xử lý                                                           |
| ----------------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------- |
| Không thể lưu Storyline / Storyline Item  | Chưa nhập đủ các trường bắt buộc (Story Line Name, Description...)       | Kiểm tra và nhập đầy đủ các trường bắt buộc rồi bấm Save/Finish      |
| Không tìm thấy Storyline                  | Sai điều kiện lọc tìm kiếm                                               | Kiểm tra lại Filter, bấm Reset để về danh sách mặc định              |
| Không lưu được Document Interaction       | Thiếu Background Image hoặc chưa có Marker / Marker thiếu Title, Content | Upload ảnh nền, thêm tối thiểu 1 Marker đủ Title và Content rồi Save |
| Không chỉnh sửa/xóa được Storyline        | Storyline đã được học viên học, hệ thống chặn cập nhật                   | Chỉ chỉnh sửa khi Storyline chưa được học; tạo Storyline mới nếu cần |
| Không upload được Video                   | Định dạng/file video không hợp lệ                                        | Kiểm tra lại file hoặc chọn Video có sẵn trên hệ thống               |
| Không thực hiện được thao tác tạo/sửa/xóa | Tài khoản chưa được cấp quyền tương ứng                                  | Liên hệ Admin để được cấp quyền tạo/chỉnh sửa Storyline              |
