# Certificate Management

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 18, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Certificate** trên hệ thống vận hành **OPS**.

Chức năng **Certificate** cho phép người dùng tạo và quản lý các mẫu chứng chỉ sử dụng cho khóa học. Người dùng có thể xem danh sách chứng chỉ, xem hình ảnh chi tiết của chứng chỉ, tạo mới mẫu chứng chỉ, upload ảnh nền chứng chỉ, thiết lập khu vực hiển thị tên học viên và chỉnh sửa thông tin chứng chỉ khi cần.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                         | Quyền hạn                                                      |
| --------- | ------------------------------- | -------------------------------------------------------------- |
| Admin     | Người quản trị hệ thống OPS     | Có quyền xem, tạo mới và chỉnh sửa chứng chỉ theo phân quyền   |
| SX        | Người vận hành nội dung học tập | Có quyền quản lý danh sách chứng chỉ phục vụ cấu hình khóa học |

***

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Course & Materials
* **Chức năng chính:** Certificate Management
* **Module liên quan:**
  * Course
  * Resources
  * Learning Progress / Certificate Logic
  * LMS học viên

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành OPS.
* Tài khoản người dùng đã được cấp quyền truy cập chức năng **Certificates**.
* Đối với thao tác xem danh sách, người dùng cần có quyền xem danh sách chứng chỉ đã tạo trên hệ thống.
* Đối với thao tác tạo mới, người dùng cần có quyền tạo mới chứng chỉ.
* Đối với thao tác chỉnh sửa, người dùng cần có quyền chỉnh sửa chứng chỉ.
* Đối với thao tác chọn ảnh từ Resources, hệ thống cần có sẵn hình ảnh trong kho tài nguyên.
* Đối với thao tác upload ảnh từ thiết bị, file ảnh cần thuộc định dạng hệ thống hỗ trợ.
* Nếu chứng chỉ đã được thêm vào Course, người dùng không được thay đổi thông tin **Loại Chứng chỉ**.

## II. Tổng Quan Giao Diện

<figure><img src="../.gitbook/assets/image (164).png" alt=""><figcaption></figcaption></figure>

Màn hình **Certificate List** cho phép người dùng xem, tìm kiếm và quản lý danh sách chứng chỉ đã được tạo trên hệ thống OPS.

Tại màn hình này, người dùng có thể:

* Xem danh sách chứng chỉ hiện có.
* Tìm kiếm chứng chỉ theo tên, loại chứng chỉ, trạng thái hoặc thời gian.
* Xem hình ảnh chi tiết của chứng chỉ.
* Tạo mới chứng chỉ.
* Chỉnh sửa trạng thái chứng chỉ.
* Truy cập màn hình chỉnh sửa chứng chỉ.

***

### Các thành phần chính trên màn hình danh sách Certificate

| Khu vực / Thành phần         | Mô tả                                                                               |
| ---------------------------- | ----------------------------------------------------------------------------------- |
| **Vùng bộ lọc tìm kiếm**     | Cho phép người dùng tìm kiếm chứng chỉ theo điều kiện lọc.                          |
| **Search**                   | Tìm kiếm theo tên chứng chỉ.                                                        |
| **Program**                  | Lọc theo chương trình học tương ứng.                                                |
| **Sort by**                  | Sắp xếp danh sách chứng chỉ theo tiêu chí được chọn.                                |
| **From Date**                | Lọc chứng chỉ từ ngày bắt đầu.                                                      |
| **To Date**                  | Lọc chứng chỉ đến ngày kết thúc.                                                    |
| **Nút Search**               | Áp dụng điều kiện lọc và hiển thị danh sách chứng chỉ tương ứng.                    |
| **Nút Reset**                | Xóa toàn bộ điều kiện tìm kiếm và hiển thị lại danh sách chứng chỉ mặc định.        |
| **Nút Create Template**      | Tạo mới một mẫu chứng chỉ.                                                          |
| **Bảng danh sách chứng chỉ** | Hiển thị các chứng chỉ đã được tạo trong hệ thống.                                  |
| **Template Name**            | Tên chứng chỉ. Người dùng có thể nhấp vào để xem hoặc chỉnh sửa chi tiết chứng chỉ. |
| **Category**                 | Loại chứng chỉ theo từng loại chương trình học.                                     |
| **Status**                   | Trạng thái hiện tại của chứng chỉ, gồm Published hoặc Block.                        |
| **Date**                     | Hiển thị ngày tạo và ngày cập nhật chứng chỉ.                                       |

### Ý nghĩa trạng thái chứng chỉ

| Trạng thái    | Ý nghĩa                                                                                |
| ------------- | -------------------------------------------------------------------------------------- |
| **Published** | Chứng chỉ đang được công khai và có thể được thêm vào làm Certificate của Course.      |
| **Block**     | Chứng chỉ bị chặn và không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course. |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1. Xem danh sách/chi tiết Chứng chỉ <a href="#id-1.-xem-danh-sach-chi-tiet-chung-chi" id="id-1.-xem-danh-sach-chi-tiet-chung-chi"></a>

**3.1.1. Xem danh sách/chi tiết Chứng chỉ**

_**Bước 1**_: Sau khi đăng nhập thành công vào hệ thống, tại thanh Menu, click vào **Certificates**.

Các trường thông tin hiển thị bao gồm:

* Số thứ tự
* Tên Chứng chỉ
* Loại Chứng chỉ: theo từng loại Khóa học
* Trạng thái
  * Công khai (Published): có thể được thêm vào làm Certificate của Khóa học.
  * Chặn (Block): chứng chỉ này sẽ không xuất hiện trong danh sách những chứng chỉ có thể thêm vào Khóa học.
* Ngày tạo và ngày cập nhật Chứng chỉ.

<figure><img src="https://media-cdn.atlassian.com/file/44b62364-1e92-4251-b716-15b129756868/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=44b62364-1e92-4251-b716-15b129756868&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: User click vào tên Chứng Chỉ (Template name) để xem hình ảnh chi tiết của Chứng chỉ.

<figure><img src="https://media-cdn.atlassian.com/file/57ef19e8-9525-470a-9b8f-eae0c5ec5021/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=57ef19e8-9525-470a-9b8f-eae0c5ec5021&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

**3.1.2. Tìm kiếm Chứng chỉ**

Tìm kiếm theo các trường Tên Chứng Chỉ, chương trình học (Program), Sort by, From Date - To Date.

* Chọn **Search** để hiển thị các Chứng chỉ theo điều kiện tìm kiếm trên màn hình.
* Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách Chửng chỉ theo thời gian tạo.

<figure><img src="../.gitbook/assets/image (165).png" alt=""><figcaption></figcaption></figure>

### 3.2. Tạo mới Chứng chỉ <a href="#id-2.-tao-moi-chung-chi" id="id-2.-tao-moi-chung-chi"></a>

_**Bước 1**_: Tại màn hình danh sách Chứng chỉ, chọn **Create Template** để chuyển đến màn hình tạo mới Chứng chỉ.

<figure><img src="../.gitbook/assets/image (166).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: Nhập các thông tin cần thiết:

* Tên Chứng chỉ
* Program: chọn 1 giá trị trong các giá trị có sẵn.

<figure><img src="../.gitbook/assets/image (168).png" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Click vào **Upload File** để mở màn hình chọn ảnh làm Chứng chỉ, có thể chọn ảnh từ thiết bị hoặc chọn ảnh đã có sẵn trên hệ thống.

<figure><img src="../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

* Tải ảnh lên hệ thống từ thiết bị: Tại thẻ Upload File, chọn **Browse** để chọn ảnh từ thiết bị. Các định dạng ảnh được phép tải lên bao gồm _.jpg, .jpeg, .png, .gif, .webp._
* Chỉ được chọn một ảnh để tải lên.

<figure><img src="../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>

* Chọn ảnh có sẵn trên hệ thống: Chuyển qua màn hình **Resources**, và chọn hình ảnh cho Chứng chỉ.

<figure><img src="../.gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>

Có thể tìm kiếm hình ảnh thông qua các điều kiện:

* Tên hình ảnh
* Vị trí của tài liệu theo Khóa học, chọn các giá trị lần lượt theo thứ tự:
  * Course.
  * Part: các học phần lớn thuộc khóa học vừa chọn.
  * Chapter: các chương thuộc học phần lớn vừa chọn.
  * Unit: các bài học thuộc chương vừa chọn.
  * Activity: các hoạt động thuộc bài học vừa chọn.
* Loại tài liệu: Image
* From date - To date: khoảng thời gian tải hình ảnh lên hệ thống.

Click **Search** để tìm kiếm hình ảnh theo các điều kiện đã nhập.

Click **Reset** để xóa các điều kiện đã nhập, đồng thời hiển thị danh sách hình ảnh ban đầu.

_**Bước 4:**_ Click **Upload** để lưu.

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption><p>Tải file template chứng chỉ lên hệ thống</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (173).png" alt=""><figcaption><p>Chọn ảnh chứng chỉ từ hệ thống</p></figcaption></figure>

_**Bước 5:**_ Thêm Khu vực hiển thị tên học viên bằng cách click **Add Student Name**

<figure><img src="https://media-cdn.atlassian.com/file/084d675d-19a9-41c5-bae3-2544688d5a25/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=084d675d-19a9-41c5-bae3-2544688d5a25&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 6:**_ Chỉnh sửa đặc điểm của ô chứa tên học viên.

* Click chuột phải 2 lần để thực hiện di chuyển hoặc chỉnh lại kích cỡ của ô văn bản.

<figure><img src="https://media-cdn.atlassian.com/file/38ea4718-0d44-4686-bc67-203972107814/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=38ea4718-0d44-4686-bc67-203972107814&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

* Thay đổi kích chữ, font chữ, căn trái/phải/giữa… tại khu vực chỉnh sửa văn bản.

<figure><img src="https://media-cdn.atlassian.com/file/e3e871b5-4fad-48b9-8359-20571e466ac1/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=e3e871b5-4fad-48b9-8359-20571e466ac1&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 7:**_ Chọn **Save** để lưu Chứng chỉ.

<figure><img src="https://media-cdn.atlassian.com/file/7fa62d80-34dd-4fe6-a0c2-ecddef809e85/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=7fa62d80-34dd-4fe6-a0c2-ecddef809e85&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

### 3.3. Chỉnh sửa Chứng chỉ <a href="#id-3.-chinh-sua-chung-chi" id="id-3.-chinh-sua-chung-chi"></a>

_**Bước 1**_: Tại màn hình danh sách chứng chỉ, chỉnh sửa Trạng thái của chứng chỉ. Có thể đổi từ **Published** sang **Block** và ngược lại.

<figure><img src="https://media-cdn.atlassian.com/file/65d22a1d-fd33-41c8-882e-73c19a63957b/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=65d22a1d-fd33-41c8-882e-73c19a63957b&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: Click vào Tên Chứng chỉ (Template name) muốn chỉnh sửa để chuyển đến màn hình chỉnh sửa Chứng Chỉ.

<figure><img src="https://media-cdn.atlassian.com/file/57ef19e8-9525-470a-9b8f-eae0c5ec5021/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=57ef19e8-9525-470a-9b8f-eae0c5ec5021&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Chỉnh sửa thông tin của Chứng Chỉ:

* Đổi tên
* Đổi program tương ứng với chương trình học
* Đổi ảnh Chứng chỉ
* Chỉnh sửa kích cỡ, định dạng ô chứa tên học viên và tên học viên

Nếu chứng chỉ đã được thêm vào Khóa học thì sẽ không được thay đổi thông tin về loại Chứng chỉ.

<figure><img src="https://media-cdn.atlassian.com/file/0a3c97e1-26e7-4b9d-b647-73176e419613/image/cdn?allowAnimated=true&#x26;client=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;collection=contentId-196313607&#x26;height=125&#x26;max-age=2592000&#x26;mode=full-fit&#x26;source=mediaCard&#x26;token=eyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o&#x26;width=760#media-blob-url=true&#x26;id=0a3c97e1-26e7-4b9d-b647-73176e419613&#x26;clientId=bf9221ec-97ac-4ef5-afcd-8390e470d7cb&#x26;contextId=contentId-196313607&#x26;collection=contentId-196313607" alt=""><figcaption></figcaption></figure>

_**Bước 4**_: Chọn **Save** để lưu.

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Người dùng cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa chứng chỉ.
* Trạng thái **Published** cho phép chứng chỉ được thêm vào làm Certificate của Course.
* Trạng thái **Block** khiến chứng chỉ không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course.
* Hệ thống chỉ cho phép chọn **một ảnh** để làm ảnh chứng chỉ.
* Định dạng ảnh được hỗ trợ gồm: **.jpg, .jpeg, .png, .gif, .webp**.
* Người dùng cần thêm khu vực **Student Name** để hệ thống hiển thị tên học viên trên chứng chỉ.
* Có thể chỉnh vị trí, kích cỡ, font chữ và căn chỉnh của vùng tên học viên.
* Nếu chứng chỉ đã được thêm vào Course thì không được thay đổi **Program**.

***

### 💡 Mẹo sử dụng

* Nên đặt tên chứng chỉ rõ ràng theo chương trình học, program hoặc mục đích sử dụng để dễ tìm kiếm.
* Nếu sử dụng ảnh từ Resources, nên dùng bộ lọc **Course → Part → Chapter → Unit → Activity** để tìm đúng tài nguyên cần dùng.
* Nên kiểm tra kỹ trạng thái chứng chỉ trước khi gắn vào Course.
* Nên để chứng chỉ ở trạng thái **Block** nếu mẫu chứng chỉ chưa hoàn thiện hoặc chưa muốn sử dụng.
* Trước khi lưu, nên kiểm tra lại vị trí hiển thị tên học viên trên ảnh chứng chỉ để tránh lệch bố cục.
* Với các chứng chỉ đã đưa vào Course, nên hạn chế chỉnh sửa để tránh ảnh hưởng đến cấu hình khóa học đang sử dụng.

## V. Câu Hỏi Thường Gặp

**Q: Trạng thái Published có ý nghĩa gì?**\
A: Published là trạng thái công khai. Chứng chỉ ở trạng thái này có thể được thêm vào làm Certificate của Course.

**Q: Trạng thái Block có ý nghĩa gì?**\
A: Block là trạng thái chặn. Chứng chỉ ở trạng thái này sẽ không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course.

**Q: Tôi có thể chọn nhiều ảnh cho một chứng chỉ không?**\
A: Không. Hệ thống chỉ cho phép chọn một ảnh để làm ảnh chứng chỉ.

**Q: Add Student Name dùng để làm gì?**\
A: Add Student Name dùng để thêm khu vực hiển thị tên học viên trên mẫu chứng chỉ.

**Q: Tôi có thể chỉnh font chữ hoặc vị trí tên học viên không?**\
A: Có. Người dùng có thể chỉnh vị trí, kích cỡ, font chữ, căn trái/phải/giữa và các thuộc tính hiển thị khác của vùng tên học viên.

**Q: Vì sao tôi không đổi được Loại Chứng chỉ?**\
A: Nếu chứng chỉ đã được thêm vào Course, hệ thống không cho phép thay đổi Loại Chứng chỉ để tránh ảnh hưởng đến cấu hình khóa học.
