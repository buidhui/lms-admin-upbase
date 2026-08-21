# Certificate Management

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Certificate** trên hệ thống vận hành **OPS**.

Chức năng **Certificate** cho phép người dùng tạo và quản lý các mẫu chứng chỉ sử dụng cho khóa học. Người dùng có thể xem danh sách chứng chỉ, xem hình ảnh chi tiết của chứng chỉ, tạo mới mẫu chứng chỉ, upload ảnh nền chứng chỉ, thiết lập khu vực hiển thị tên học viên và chỉnh sửa thông tin chứng chỉ khi cần.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                         | Quyền hạn                                                      |
| --------- | ------------------------------- | -------------------------------------------------------------- |
| Admin     | Người quản trị hệ thống OPS     | Có quyền xem, tạo mới và chỉnh sửa chứng chỉ theo phân quyền   |
| SX        | Người vận hành nội dung học tập | Có quyền quản lý danh sách chứng chỉ phục vụ cấu hình khóa học |

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

![](<.gitbook/assets/image (473)>)

Màn hình **Certificate List** cho phép người dùng xem, tìm kiếm và quản lý danh sách chứng chỉ đã được tạo trên hệ thống OPS.

Tại màn hình này, người dùng có thể:

* Xem danh sách chứng chỉ hiện có.
* Tìm kiếm chứng chỉ theo tên, loại chứng chỉ, trạng thái hoặc thời gian.
* Xem hình ảnh chi tiết của chứng chỉ.
* Tạo mới chứng chỉ.
* Chỉnh sửa trạng thái chứng chỉ.
* Truy cập màn hình chỉnh sửa chứng chỉ.

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

### 3.1. Xem danh sách/chi tiết Chứng chỉ

#### 3.1.1. Xem danh sách/chi tiết Chứng chỉ

{% stepper %}
{% step %}
## Truy cập Certificates

Sau khi đăng nhập thành công vào hệ thống, tại thanh Menu, click vào **Certificates**.

Các trường thông tin hiển thị bao gồm:

* Số thứ tự
* Tên Chứng chỉ
* Loại Chứng chỉ: theo từng loại Khóa học
* Trạng thái
  * Công khai (Published): có thể được thêm vào làm Certificate của Khóa học.
  * Chặn (Block): chứng chỉ này sẽ không xuất hiện trong danh sách những chứng chỉ có thể thêm vào Khóa học.
* Ngày tạo và ngày cập nhật Chứng chỉ.

![](https://sapp-academy.gitbook.io/sapp-academy/~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F44b62364-1e92-4251-b716-15b129756868%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D44b62364-1e92-4251-b716-15b129756868%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=6b06d4f3\&sv=2)
{% endstep %}

{% step %}
## Xem hình ảnh chi tiết chứng chỉ

User click vào tên Chứng Chỉ (Template name) để xem hình ảnh chi tiết của Chứng chỉ.

![](https://sapp-academy.gitbook.io/sapp-academy/~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F57ef19e8-9525-470a-9b8f-eae0c5ec5021%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aW9uOmNvbnRlbnRJZC0xOTYzMTM2MDciOlsicmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D57ef19e8-9525-470a-9b8f-eae0c5ec5021%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=888f396f\&sv=2)
{% endstep %}
{% endstepper %}

#### 3.1.2. Tìm kiếm Chứng chỉ

Tìm kiếm theo các trường Tên Chứng Chỉ, chương trình học (Program), Sort by, From Date - To Date.

* Chọn **Search** để hiển thị các Chứng chỉ theo điều kiện tìm kiếm trên màn hình.
* Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách Chửng chỉ theo thời gian tạo.

![](<.gitbook/assets/image (175)>)

### 3.2. Tạo mới Chứng chỉ

{% stepper %}
{% step %}
## Mở màn hình tạo mới

Tại màn hình danh sách Chứng chỉ, chọn **Create Template** để chuyển đến màn hình tạo mới Chứng chỉ.

![](<.gitbook/assets/image (176)>)

![](<.gitbook/assets/image (177)>)
{% endstep %}

{% step %}
## Nhập thông tin chứng chỉ

Nhập các thông tin cần thiết:

* Tên Chứng chỉ
* Program: chọn 1 giá trị trong các giá trị có sẵn.

![](<.gitbook/assets/image (178)>)
{% endstep %}

{% step %}
## Chọn ảnh chứng chỉ

Click vào **Upload File** để mở màn hình chọn ảnh làm Chứng chỉ, có thể chọn ảnh từ thiết bị hoặc chọn ảnh đã có sẵn trên hệ thống.

![](<.gitbook/assets/image (179)>)

* Tải ảnh lên hệ thống từ thiết bị: Tại thẻ Upload File, chọn **Browse** để chọn ảnh từ thiết bị. Các định dạng ảnh được phép tải lên bao gồm _.jpg, .jpeg, .png, .gif, .webp._
* Chỉ được chọn một ảnh để tải lên.

![](<.gitbook/assets/image (180)>)

* Chọn ảnh có sẵn trên hệ thống: Chuyển qua màn hình **Resources**, và chọn hình ảnh cho Chứng chỉ.

![](<.gitbook/assets/image (181)>)

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
{% endstep %}

{% step %}
## Lưu ảnh

Click **Upload** để lưu.

![](<.gitbook/assets/image (182)>)

_Tải file template chứng chỉ lên hệ thống_

![](<.gitbook/assets/image (183)>)

_Chọn ảnh chứng chỉ từ hệ thống_
{% endstep %}

{% step %}
## Thêm khu vực hiển thị tên học viên

Thêm Khu vực hiển thị tên học viên bằng cách click **Add Student Name**.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F084d675d-19a9-41c5-bae3-2544688d5a25%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D084d675d-19a9-41c5-bae3-2544688d5a25%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=9096b873\&sv=2)
{% endstep %}

{% step %}
## Chỉnh sửa đặc điểm của ô chứa tên học viên

* Click chuột phải 2 lần để thực hiện di chuyển hoặc chỉnh lại kích cỡ của ô văn bản.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F38ea4718-0d44-4686-bc67-203972107814%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D38ea4718-0d44-4686-bc67-203972107814%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=90901c7f\&sv=2)

* Thay đổi kích chữ, font chữ, căn trái/phải/giữa… tại khu vực chỉnh sửa văn bản.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2Fe3e871b5-4fad-48b9-8359-20571e466ac1%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3De3e871b5-4fad-48b9-8359-20571e466ac1%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=c67b06d3\&sv=2)
{% endstep %}

{% step %}
## Lưu chứng chỉ

Chọn **Save** để lưu Chứng chỉ.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F7fa62d80-34dd-4fe6-a0c2-ecddef809e85%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D7fa62d80-34dd-4fe6-a0c2-ecddef809e85%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=ff01a48f\&sv=2)
{% endstep %}
{% endstepper %}

### 3.3. Chỉnh sửa Chứng chỉ

{% stepper %}
{% step %}
## Chỉnh sửa trạng thái chứng chỉ

Tại màn hình danh sách chứng chỉ, chỉnh sửa Trạng thái của chứng chỉ. Có thể đổi từ **Published** sang **Block** và ngược lại.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F65d22a1d-fd33-41c8-882e-73c19a63957b%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D65d22a1d-fd33-41c8-882e-73c19a63957b%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=168f27ff\&sv=2)
{% endstep %}

{% step %}
## Mở màn hình chỉnh sửa

Click vào Tên Chứng chỉ (Template name) muốn chỉnh sửa để chuyển đến màn hình chỉnh sửa Chứng Chỉ.

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F57ef19e8-9525-470a-9b8f-eae0c5ec5021%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D57ef19e8-9525-470a-9b8f-eae0c5ec5021%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=888f396f\&sv=2)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin chứng chỉ

Chỉnh sửa thông tin của Chứng Chỉ:

* Đổi tên
* Đổi program tương ứng với chương trình học
* Đổi ảnh Chứng chỉ
* Chỉnh sửa kích cỡ, định dạng ô chứa tên học viên và tên học viên

{% hint style="warning" %}
Nếu chứng chỉ đã được thêm vào Khóa học thì sẽ không được thay đổi thông tin về loại Chứng chỉ.
{% endhint %}

!\[]\(https://sapp-academy.gitbook.io/sapp-academy/\~gitbook/image?url=https%3A%2F%2Fmedia-cdn.atlassian.com%2Ffile%2F0a3c97e1-26e7-4b9d-b647-73176e419613%2Fimage%2Fcdn%3FallowAnimated%3Dtrue%26client%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26collection%3DcontentId-196313607%26height%3D125%26max-age%3D2592000%26mode%3Dfull-fit%26source%3DmediaCard%26token%3DeyJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJiZjkyMjFlYy05N2FjLTRlZjUtYWZjZC04MzkwZTQ3MGQ3Y2IiLCJhY2Nlc3MiOnsidXJuOmZpbGVzdG9yZTpjb2xsZWN0aWQiOlsi cmVhZCJdfSwiZXhwIjoxNzc5MDkxMTUyLCJuYmYiOjE3NzkwODgyNzIsImFhSWQiOiI3MTIwMjA6ZDBmODQ0NjUtNGQwYS00YWJmLWIyN2EtNjEwZDE0YTE1NjdhIiwiaHR0cHM6Ly9pZC5hdGxhc3NpYW4uY29tL2FwcEFjY3JlZGl0ZWQiOmZhbHNlLCJhdXRoVHlwZSI6InNlc3Npb24ifQ.0nCAOl3p2SVoL276nZtOb0QOUxRs6H4crqn\_gx21c6o%26width%3D760%23media-blob-url%3Dtrue%26id%3D0a3c97e1-26e7-4b9d-b647-73176e419613%26clientId%3Dbf9221ec-97ac-4ef5-afcd-8390e470d7cb%26contextId%3DcontentId-196313607%26collection%3DcontentId-196313607\&width=768\&dpr=3\&quality=100\&sign=40060d2f\&sv=2)
{% endstep %}

{% step %}
## Lưu thay đổi

Chọn **Save** để lưu.
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

{% hint style="warning" %}
* Người dùng cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa chứng chỉ.
* Trạng thái **Published** cho phép chứng chỉ được thêm vào làm Certificate của Course.
* Trạng thái **Block** khiến chứng chỉ không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course.
* Hệ thống chỉ cho phép chọn **một ảnh** để làm ảnh chứng chỉ.
* Định dạng ảnh được hỗ trợ gồm: **.jpg, .jpeg, .png, .gif, .webp**.
* Người dùng cần thêm khu vực **Student Name** để hệ thống hiển thị tên học viên trên chứng chỉ.
* Có thể chỉnh vị trí, kích cỡ, font chữ và căn chỉnh của vùng tên học viên.
* Nếu chứng chỉ đã được thêm vào Course thì không được thay đổi **Program**.
{% endhint %}

### 💡 Mẹo sử dụng

{% hint style="info" %}
* Nên đặt tên chứng chỉ rõ ràng theo chương trình học, program hoặc mục đích sử dụng để dễ tìm kiếm.
* Nếu sử dụng ảnh từ Resources, nên dùng bộ lọc **Course → Part → Chapter → Unit → Activity** để tìm đúng tài nguyên cần dùng.
* Nên kiểm tra kỹ trạng thái chứng chỉ trước khi gắn vào Course.
* Nên để chứng chỉ ở trạng thái **Block** nếu mẫu chứng chỉ chưa hoàn thiện hoặc chưa muốn sử dụng.
* Trước khi lưu, nên kiểm tra lại vị trí hiển thị tên học viên trên ảnh chứng chỉ để tránh lệch bố cục.
* Với các chứng chỉ đã đưa vào Course, nên hạn chế chỉnh sửa để tránh ảnh hưởng đến cấu hình khóa học đang sử dụng.
{% endhint %}

## V. Câu Hỏi Thường Gặp

<details>

<summary>Q: Trạng thái Published có ý nghĩa gì?</summary>

A: Published là trạng thái công khai. Chứng chỉ ở trạng thái này có thể được thêm vào làm Certificate của Course.

</details>

<details>

<summary>Q: Trạng thái Block có ý nghĩa gì?</summary>

A: Block là trạng thái chặn. Chứng chỉ ở trạng thái này sẽ không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course.

</details>

<details>

<summary>Q: Tôi có thể chọn nhiều ảnh cho một chứng chỉ không?</summary>

A: Không. Hệ thống chỉ cho phép chọn một ảnh để làm ảnh chứng chỉ.

</details>

<details>

<summary>Q: Add Student Name dùng để làm gì?</summary>

A: Add Student Name dùng để thêm khu vực hiển thị tên học viên trên mẫu chứng chỉ.

</details>

<details>

<summary>Q: Tôi có thể chỉnh font chữ hoặc vị trí tên học viên không?</summary>

A: Có. Người dùng có thể chỉnh vị trí, kích cỡ, font chữ, căn trái/phải/giữa và các thuộc tính hiển thị khác của vùng tên học viên.

</details>

<details>

<summary>Q: Vì sao tôi không đổi được Loại Chứng chỉ?</summary>

A: Nếu chứng chỉ đã được thêm vào Course, hệ thống không cho phép thay đổi Loại Chứng chỉ để tránh ảnh hưởng đến cấu hình khóa học.

</details>
