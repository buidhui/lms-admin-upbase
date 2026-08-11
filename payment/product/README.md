---
description: >-
  Kết quả đạt được: Các sản phẩm đơn lẻ được tạo sẵn sàng để gắn vào các Combo
  Products hoặc Orders.
---

# Product

## Record of changes

\*A - Add M - Modify D - Delete

<table><thead><tr><th width="147.99993896484375">Effective Date</th><th width="146.66668701171875">Update Person</th><th width="92.6666259765625">A,M,D</th><th width="296.0001220703125">Change Description</th><th>Version</th></tr></thead><tbody><tr><td>August 15, 2025</td><td>Nhungdh</td><td>A</td><td>Create New</td><td>3.0.0</td></tr><tr><td>June 8, 2026</td><td>Nhungnth</td><td>M</td><td>Cập nhật tính năng Product</td><td>3.1.0</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" icon="1" %}
### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/products?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/products?page_index=1\&page_size=10)
{% endhint %}

{% hint style="warning" icon="2" %}
#### Phạm vi & Module liên quan <a href="#id-1.3-pham-vi-and-module-lien-quan" id="id-1.3-pham-vi-and-module-lien-quan"></a>

* **Module chính**: Product
* **Module liên quan**: [Program & Subject](../../khoa-hoc-course/program-and-subject/), [Combo Product](../combo/), [Promotion Codes](../promotion-code/), [List of Orders](../order-list/)
* **Hệ thống tích hợp**: Không có
{% endhint %}

{% hint style="success" icon="3" %}
### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Product.
{% endhint %}

## II. Hướng dẫn chi tiết

> Products là danh sách các sản phẩm đơn lẻ, được gắn độc lập vào Orders hoặc được thêm vào các nhóm sản phẩm (Combo Products).

<details>

<summary>Xem danh sách sản phẩm đơn lẻ</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Products**

Tại thanh menu hệ thống: chọn <mark style="color:$primary;">Order & Payment → Product & Combo →</mark> <mark style="color:$primary;">**chọn tab Products**</mark>

<figure><img src="../../.gitbook/assets/image (1021).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**User có thể tìm kiếm sản phẩm theo điều kiện**

a. Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* <mark style="color:$primary;">Search Product</mark>: Theo tên sản phẩm
* <mark style="color:$primary;">Category</mark>: Theo chương trình học
* <mark style="color:$primary;">Status</mark>: Theo trạng thái sản phẩm
* <mark style="color:$primary;">Sort by</mark>: Chọn cách sắp xếp sản phẩm (A-Z, Z-A, Latest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

<figure><img src="../../.gitbook/assets/image (1023).png" alt=""><figcaption></figcaption></figure>

b. Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết sản phẩm đơn lẻ</summary>

{% stepper %}
{% step %}
**Chọn sản phẩm cần xem chi tiết**

Tại màn hình danh sách sản phẩm, click vào giá trị tại cột **Product Name**.

<figure><img src="../../.gitbook/assets/image (1024).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hoàn tất**

Hệ thống hiển thị màn hình chi tiết sản phẩm tương ứng.

<figure><img src="../../.gitbook/assets/image (1025).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới sản phẩm đơn lẻ</summary>

{% stepper %}
{% step %}
**Tại màn hình&#x20;**<mark style="color:$primary;">**Products**</mark>**, chọn&#x20;**<mark style="color:$primary;">**New Product**</mark>**.**

Hệ thống chuyển tới màn hình tạo mới sản phẩm đơn lẻ.

<div><figure><img src="../../.gitbook/assets/image (1026).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1027).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Nhập thông tin sản phẩm**

<figure><img src="../../.gitbook/assets/image (1028).png" alt=""><figcaption></figcaption></figure>

Chi tiết các trường thông tin dưới đây:

<table><thead><tr><th width="199" valign="middle">Trường thông tin</th><th>Input</th></tr></thead><tbody><tr><td valign="middle">Product name<mark style="color:$danger;">*</mark></td><td>Nhập tên sản phẩm cần tạo mới</td></tr><tr><td valign="middle">Category<mark style="color:$danger;">*</mark></td><td>Chọn chương trình học của sản phẩm từ danh sách cho trước</td></tr><tr><td valign="middle">Subject<mark style="color:$danger;">*</mark></td><td>Chọn môn học của sản phẩm từ danh sách cho trước (chỉ hiển thị tương ứng với Category)</td></tr><tr><td valign="middle">Construction mode<mark style="color:$danger;">*</mark></td><td>Chọn hình thức học của sản phẩm từ danh sách cho trước</td></tr><tr><td valign="middle">Product - Main Course</td><td>Hệ thống cập nhật tự động dựa trên Subject và Construction mode của sản phẩm</td></tr><tr><td valign="middle">Price<mark style="color:$danger;">*</mark></td><td>Nhập giá của sản phẩm theo đơn vị VND</td></tr><tr><td valign="middle">Status<mark style="color:$danger;">*</mark></td><td>Chọn trạng thái của sản phẩm, bao gồm:<br>- <mark style="color:$success;">Active:</mark> Sản phẩm vẫn đang được kinh doanh<br>- <mark style="color:$danger;">Inactive</mark>: Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới</td></tr></tbody></table>

> Lưu ý:
>
> * User cần kiểm tra lại thông tin trước khi Save, đặc biệt là <mark style="color:$primary;">**Category, Subject, Construction Mode và Price**</mark>**.**
{% endstep %}

{% step %}
**Lưu thông tin sản phẩm**

Sau khi nhập đủ thông tin bắt buộc, chọn <mark style="color:$primary;">**Save**</mark> để lưu thông tin sản phẩm.

→ Hệ thống lưu thông tin sản phẩm mới, hiển thị ở đầu danh sách sản phẩm đơn lẻ.

<figure><img src="../../.gitbook/assets/image (1029).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa thông tin sản phẩm đơn lẻ</summary>

{% stepper %}
{% step %}
**Truy cập màn hình chỉnh sửa**

Tại màn hình danh sách Products, user có thể truy cập màn hình chỉnh sửa sản phẩm bằng 1 trong 2 cách sau:

* Cách 1: Chọn <mark style="color:$primary;">**Product Name**</mark> của sản phẩm cần chỉnh sửa
* Cách 2: Chọn <mark style="color:$primary;">**Action > Edit**</mark> tại sản phẩm cần chỉnh sửa

→ Hệ thống chuyển đến màn hình chỉnh sửa thông tin sản phẩm.

<figure><img src="../../.gitbook/assets/image (1030).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật thông tin sản phẩm**

<figure><img src="../../.gitbook/assets/image (1031).png" alt=""><figcaption></figcaption></figure>

Người dùng nhập hoặc chỉnh sửa các thông tin cần cập nhật.

<table><thead><tr><th width="220.66668701171875">Trường thông tin</th><th>Hướng dẫn chỉnh sửa</th></tr></thead><tbody><tr><td>Product name<mark style="color:$danger;">*</mark></td><td>Cập nhật tên sản phẩm</td></tr><tr><td>Category<mark style="color:$danger;">*</mark></td><td>Chọn chương trình học của sản phẩm từ danh sách cho trước</td></tr><tr><td>Subject<mark style="color:$danger;">*</mark></td><td>Chọn môn học của sản phẩm từ danh sách cho trước</td></tr><tr><td>Construction mode<mark style="color:$danger;">*</mark></td><td>Chọn hình thức học của sản phẩm từ danh sách cho trước</td></tr><tr><td>Product - Main course</td><td>Hệ thống cập nhật tự động theo Subject và Construction Mode user đã chọn</td></tr><tr><td>Price<mark style="color:$danger;">*</mark></td><td>Cập nhật giá của sản phẩm theo đơn vị VND</td></tr><tr><td>Status<mark style="color:$danger;">*</mark></td><td>Chọn trạng thái của sản phẩm<br>- <mark style="color:$success;">Active:</mark> Sản phẩm vẫn đang được kinh doanh<br>- <mark style="color:$danger;">Inactive</mark>: Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới</td></tr></tbody></table>

> Lưu ý:
>
> * User cần kiểm tra lại thông tin trước khi Save, đặc biệt là <mark style="color:$primary;">**Category, Subject, Construction Mode và Price**</mark>**.**
{% endstep %}

{% step %}
**Chọn Save để lưu thông tin**

Sau khi cập nhật thông tin cần chỉnh sửa, chọn <mark style="color:$primary;">**Save**</mark> để lưu thông tin.

→ Hệ thống lưu thông tin đã chỉnh sửa của sản phẩm và quay lại màn Danh sách sản phẩm.

<figure><img src="../../.gitbook/assets/image (1032).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa sản phẩm đơn lẻ</summary>

{% stepper %}
{% step %}
**Chọn sản phẩm cần xóa, chọn Action > Delete**

Hệ thống hiển thị hộp thoại xác nhận xóa sản phẩm → User có thể chọn tiếp tục xóa hoặc hủy thao tác.

<figure><img src="../../.gitbook/assets/image (1033).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận thao tác xóa trên hộp thoại**

<figure><img src="../../.gitbook/assets/image (1035).png" alt=""><figcaption></figcaption></figure>

Tại hộp thoại xác nhận, user chọn <mark style="color:$primary;">**Yes**</mark> để đồng ý xóa sản phẩm.

→ Kết quả mong đợi:

* Hệ thống xóa sản phẩm khỏi danh sách;
* Sản phẩm đã xóa không còn hiển thị trên màn hình danh sách sản phẩm;
* Sản phẩm bị xóa sẽ biến mất khỏi các nhóm sản phẩm **Combo Products** hoặc mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó.
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.
{% endstep %}

{% step %}
**Kiểm tra kết quả sau khi xóa**

Sau khi xác nhận xóa, user kiểm tra lại danh sách sản phẩm.

→ Kết quả mong đợi:

* Sản phẩm vừa xóa không còn xuất hiện trên danh sách sản phẩm đơn lẻ.
* Các đơn hàng đã tạo trước đó có chứa sản phẩm này vẫn được giữ nguyên thông tin.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" icon="1" %}
### Lưu ý quan trọng

1. Khi thay đổi <mark style="color:$primary;">**Price**</mark> của sản phẩm:

* Các đơn hàng trong tương lai sẽ áp dụng giá mới của sản phẩm.
* Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.

2. Khi đổi trạng thái sản phẩm từ <mark style="color:$primary;">**Active**</mark> sang <mark style="color:$primary;">**Inactive**</mark>:

* Sản phẩm sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.
* Các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái không bị ảnh hưởng.

3. Khi xóa sản phẩm, sản phẩm sẽ bị xóa khỏi:

* <mark style="color:$primary;">**Combo Products**</mark> có chứa sản phẩm đó
* Mã khuyến mại <mark style="color:$primary;">**Promotion Codes**</mark> đã gắn với sản phẩm trước đó
{% endhint %}

{% hint style="info" icon="2" %}
### Mẹo sử dụng

1. Khi tìm kiếm, có thể kết hợp nhiều điều kiện tìm kiếm để thu hẹp kết quả nhanh hơn
{% endhint %}

## IV. Các lỗi thường gặp & Cách xử lý

| Lỗi hoặc tình huống               | Nguyên nhân                                     | Cách xử lý                                                                                    |
| --------------------------------- | ----------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Không tìm thấy dữ liệu            | Sai điều kiện tìm kiếm                          | Kiểm tra lại bộ lọc tìm kiếm                                                                  |
| Không truy cập được menu Products | Chưa được cấp quyền                             | Liên hệ quản trị hệ thống                                                                     |
| This field is required            | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ các trường Product name, Category, Construction mode, Price và Status |
| Only numbers > 5000 are allowed.  | Giá sản phẩm tại trường Price nhỏ hơn 5000      | Điền lại giá sản phẩm sao cho lớn hơn 5000.                                                   |

## V. Câu hỏi thường gặp

<table><thead><tr><th width="193">Bối cảnh</th><th>Câu hỏi</th><th>Câu trả lời</th></tr></thead><tbody><tr><td>Tìm kiếm sản phẩm</td><td>Vì sao sản phẩm không hiển thị trong danh sách?</td><td>Có thể sản phẩm không thỏa điều kiện tìm kiếm hoặc người dùng chưa có quyền truy cập.</td></tr><tr><td>Xem chi tiết sản phẩm</td><td>Sản phẩm Inactive có sử dụng được không?</td><td>Không. Sản phẩm Inactive không thể thêm vào nhóm sản phẩm hoặc đơn hàng mới.</td></tr><tr><td>Tạo mới sản phẩm</td><td>Sau khi tạo mới, sản phẩm hiển thị ở đâu?</td><td>Sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách sản phẩm đơn lẻ.</td></tr><tr><td>Tạo mới sản phẩm</td><td>Có thể tạo sản phẩm ở trạng thái Inactive không?</td><td><mark style="color:$success;"><strong>Có</strong>.</mark> Tuy nhiên, sản phẩm ở trạng thái Inactive là sản phẩm đã ngừng kinh doanh và sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.</td></tr><tr><td>Chỉnh sửa sản phẩm</td><td>Có thể chỉnh sửa giá của sản phẩm không?</td><td><mark style="color:$success;"><strong>Có</strong>.</mark> Khi thay đổi giá sản phẩm, các đơn hàng trong tương lai sẽ áp dụng giá mới. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.</td></tr><tr><td>Chỉnh sửa sản phẩm</td><td>Việc đổi trạng thái sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Việc đổi trạng thái sản phẩm từ Active sang Inactive không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.</td></tr><tr><td>Chỉnh sửa sản phẩm</td><td>Sản phẩm Inactive có được thêm vào nhóm sản phẩm hoặc đơn hàng mới không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Sản phẩm ở trạng thái Inactive sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.</td></tr><tr><td>Chỉnh sửa sản phẩm</td><td>Các trường nào bắt buộc khi chỉnh sửa sản phẩm đơn lẻ?</td><td>Các trường bắt buộc gồm <mark style="color:$primary;">Product name, Category, Construction mode, Price</mark> và <mark style="color:$primary;">Status</mark>.</td></tr><tr><td>Xóa sản phẩm</td><td>Sau khi xóa, sản phẩm có còn hiển thị trên danh sách Products không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Sản phẩm xóa thành công sẽ biến mất khỏi màn hình danh sách sản phẩm</td></tr><tr><td>Xóa sản phẩm</td><td>Xóa sản phẩm có ảnh hưởng đến nhóm sản phẩm hoặc mã khuyến mại đã gắn sản phẩm đó không?</td><td><mark style="color:$success;"><strong>Có</strong></mark>. Sản phẩm đã xóa sẽ biến mất khỏi các nhóm sản phẩm <mark style="color:$primary;">Combo Products</mark> hoặc mã khuyến mại <mark style="color:$primary;">Promotion Codes</mark> đã gắn với sản phẩm trước đó.</td></tr><tr><td>Xóa sản phẩm</td><td>Xóa sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng chứa sản phẩm đã được tạo trước đó.</td></tr><tr><td>Xóa sản phẩm</td><td>Nếu không muốn tiếp tục xóa sản phẩm thì thao tác như thế nào?</td><td>Tại hộp thoại xác nhận, chọn <mark style="color:$primary;"><strong>No</strong></mark> để hủy thao tác xóa.</td></tr></tbody></table>
