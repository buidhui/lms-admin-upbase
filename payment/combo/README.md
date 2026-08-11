---
description: >-
  Kết quả đạt được: Các nhóm sản phẩm được tạo ra từ các Products sẵn sàng để
  gắn vào các Orders
---

# Combo

## Record of changes

\*A - Add M - Modify D - Delete

<table><thead><tr><th width="147.99993896484375">Effective Date</th><th width="146.66668701171875">Update Person</th><th width="92.6666259765625">A,M,D</th><th width="296.0001220703125">Change Description</th><th>Version</th></tr></thead><tbody><tr><td>August 15, 2025</td><td>Nhungdh</td><td>A</td><td>Create New</td><td>3.0.0</td></tr><tr><td>June 8, 2026</td><td>Nhungnth</td><td>M</td><td>Cập nhật tính năng Combo</td><td>3.1.0</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" icon="1" %}
### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/combo-products?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/combo-products?page_index=1\&page_size=10)
{% endhint %}

{% hint style="warning" icon="2" %}
#### Phạm vi & Module liên quan <a href="#id-1.3-pham-vi-and-module-lien-quan" id="id-1.3-pham-vi-and-module-lien-quan"></a>

* **Module chính**: Combo Product
* **Module liên quan**: [Program & Subject](../../khoa-hoc-course/program-and-subject/), [Product](../product/), [Promotion Codes](../promotion-code/), [List of Orders](../order-list/)
* **Hệ thống tích hợp**: Không có
{% endhint %}

{% hint style="success" icon="3" %}
### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Combo.
{% endhint %}

## II. Hướng dẫn chi tiết

> Combo Product là danh sách các nhóm sản phẩm, được sử dụng để gắn vào các Orders. Combo Product được tạo bằng các khóa học đơn lẻ thuộc cùng chương trình kết hợp với nhau.

<details>

<summary>Xem danh sách nhóm sản phẩm</summary>

{% stepper %}
{% step %}
**Truy cập màn hình danh sách nhóm sản phẩm**

Tại thanh Menu, chọn <mark style="color:$primary;">Order & Payment > Product & Combo ></mark> <mark style="color:$primary;">**Combo Products**</mark>.

→ Hệ thống chuyển đến màn hình danh sách Combo Products.

<figure><img src="../../.gitbook/assets/image (965).png" alt=""><figcaption></figcaption></figure>

Danh sách nhóm sản phẩm hiển thị các thông tin dưới đây:

| Thông tin  | Ý nghĩa                                  |
| ---------- | ---------------------------------------- |
| Combo name | Tên nhóm sản phẩm                        |
| Products   | Danh sách sản phẩm thuộc nhóm sản phẩm   |
| Category   | Chương trình học của nhóm sản phẩm       |
| Price      | Tổng giá trị của các sản phẩm trong nhóm |
| Status     | Trạng thái của nhóm sản phẩm             |
{% endstep %}

{% step %}
**User có thể tìm kiếm nhóm sản phẩm theo điều kiện**

Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* <mark style="color:$primary;">Search Combo</mark>: Theo tên nhóm sản phẩm
* <mark style="color:$primary;">Product</mark>: Theo một sản phẩm trong danh sách
* <mark style="color:$primary;">Category</mark>: Theo chương trình học
* <mark style="color:$primary;">Status</mark>: Theo trạng thái sản phẩm
* <mark style="color:$primary;">Sort by</mark>: Chọn cách sắp xếp sản phẩm (A-Z, Z-A, Lastest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

<figure><img src="../../.gitbook/assets/image (966).png" alt=""><figcaption></figcaption></figure>

Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết nhóm sản phẩm</summary>

{% stepper %}
{% step %}
**Chọn nhóm sản phẩm cần xem chi tiết**

Tại màn hình danh sách nhóm sản phẩm <mark style="color:$primary;">Combo Products</mark>, chọn <mark style="color:$primary;">**Combo Name**</mark> của nhóm sản phẩm cần xem.

<figure><img src="../../.gitbook/assets/image (967).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hoàn tất**

Hệ thống hiển thị màn hình chi tiết của nhóm sản phẩm tương ứng.

<figure><img src="../../.gitbook/assets/image (968).png" alt=""><figcaption></figcaption></figure>

Màn hình chi tiết nhóm sản phẩm hiển thị các thông tin sau:

| Thông tin  | Mô tả                                                                                                  |
| ---------- | ------------------------------------------------------------------------------------------------------ |
| Combo name | Tên nhóm sản phẩm                                                                                      |
| Products   | Danh sách sản phẩm trong nhóm                                                                          |
| Category   | Chương trình học của nhóm sản phẩm. Hệ thống tổng hợp từ chương trình học của từng sản phẩm trong nhóm |
| Price      | Giá của nhóm sản phẩm. Giá trị này là tổng giá trị của các sản phẩm trong nhóm                         |
| Status     | Trạng thái của nhóm sản phẩm                                                                           |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới nhóm sản phẩm</summary>

{% stepper %}
{% step %}
**Tại màn hình&#x20;**<mark style="color:$primary;">**Combo Products**</mark>**, chọn&#x20;**<mark style="color:$primary;">**New Combo**</mark>**.**

Hệ thống chuyển đến màn hình tạo mới nhóm sản phẩm.

<div><figure><img src="../../.gitbook/assets/image (969).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (970).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Nhập tên nhóm sản phẩm**

Tại trường <mark style="color:$primary;">**Combo name**</mark>, nhập tên nhóm sản phẩm cần tạo <mark style="color:$danger;">(bắt buộc)</mark>.

<figure><img src="../../.gitbook/assets/image (973).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn sản phẩm vào nhóm**

Tại trường <mark style="color:$primary;">**Products**</mark>, chọn vào vùng trống của trường để mở màn hình danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, user thực hiện:

* Chọn checkbox tại một hoặc nhiều sản phẩm cần thêm vào nhóm.
* Chọn <mark style="color:$primary;">**Add**</mark> để thêm các sản phẩm đã chọn vào nhóm.

<div><figure><img src="../../.gitbook/assets/image (974).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1040).png" alt=""><figcaption></figcaption></figure></div>

> <mark style="color:$danger;">Lưu ý:</mark> Chỉ được chọn các sản phẩm thuộc <mark style="color:$primary;">cùng 1 chương trình</mark> (Category)
{% endstep %}

{% step %}
**Kiểm tra thông tin&#x20;**<mark style="color:$primary;">**Category, Price**</mark>**&#x20;và&#x20;**<mark style="color:$primary;">**Product - Main course**</mark>

Sau khi chọn sản phẩm vào nhóm, user kiểm tra các thông tin hệ thống tự hiển thị.

<table><thead><tr><th width="155">Trường thông tin</th><th>Cách xử lý</th></tr></thead><tbody><tr><td>Category</td><td>Hệ thống cập nhật tự động Category của các sản phẩm được thêm vào Combo.</td></tr><tr><td>Product - Main course</td><td>Hệ thống cập nhật tự động theo Subject và Construction Mode của các sản phẩm trong Combo</td></tr><tr><td>Price</td><td>Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm.</td></tr></tbody></table>

<figure><img src="../../.gitbook/assets/image (947).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Status**</mark>**&#x20;của nhóm sản phẩm**

Tại trường <mark style="color:$primary;">**Status**</mark>, chọn trạng thái của nhóm sản phẩm <mark style="color:$danger;">(bắt buộc)</mark>.

<table><thead><tr><th width="93.66668701171875">Giá trị</th><th>Ý nghĩa</th></tr></thead><tbody><tr><td>Active</td><td>Nhóm sản phẩm vẫn đang được kinh doanh</td></tr><tr><td>Inactive</td><td>Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới</td></tr></tbody></table>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Save**</mark>**&#x20;để lưu thông tin nhóm sản phẩm**

Sau khi nhập đầy đủ thông tin bắt buộc, chọn <mark style="color:$primary;">**Save**</mark> để lưu thông tin.

→ Kết quả mong đợi:

* Hệ thống lưu thông tin nhóm sản phẩm mới.
* Nhóm sản phẩm vừa tạo hiển thị ở đầu danh sách nhóm sản phẩm.

<figure><img src="../../.gitbook/assets/image (948).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa thông tin nhóm sản phẩm</summary>

{% stepper %}
{% step %}
### Truy cập màn hình chỉnh sửa

Tại màn hình danh sách Combo Products, user có thể truy cập màn hình chỉnh sửa nhóm sản phẩm bằng 1 trong 2 cách dưới đây:

* **Cách 1:** Chọn <mark style="color:$primary;">**Combo Name**</mark> của nhóm sản phẩm cần chỉnh sửa
* **Cách 2**: Chọn <mark style="color:$primary;">**Action > Edit**</mark> tại nhóm sản phẩm cần chỉnh sửa

→ Hệ thống chuyển đến màn hình chỉnh sửa thông tin nhóm sản phẩm.

<figure><img src="../../.gitbook/assets/image (975).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Cập nhật Combo Name (nếu cần)

Tại trường **Combo name**, cập nhật tên nhóm sản phẩm nếu cần.

| Trường thông tin | Bắt buộc | Hướng dẫn chỉnh sửa        |
| ---------------- | -------- | -------------------------- |
| Combo name       | Có       | Cập nhật tên nhóm sản phẩm |

→ Tên nhóm sản phẩm mới được ghi nhận trên form chỉnh sửa
{% endstep %}

{% step %}
### Cập nhật danh sách Product trên Combo

User có thể <mark style="color:$primary;">Xóa, Thêm</mark> hoặc <mark style="color:$primary;">Chọn lại</mark> danh sách sản phẩm trong nhóm tương ứng như sau:

<table><thead><tr><th width="144.00006103515625">Nhu cầu</th><th>Thao tác</th></tr></thead><tbody><tr><td>Xóa sản phẩm khỏi nhóm</td><td>Chọn dấu <strong>x</strong> tại sản phẩm cần xóa</td></tr><tr><td>Thêm hoặc chọn lại sản phẩm trong nhóm</td><td><ol><li>Chọn vào vùng trống của trường <strong>Products</strong> để mở màn hình danh sách sản phẩm.</li><li>Sau đó chọn hoặc bỏ chọn checkbox tại các sản phẩm cần thay đổi và chọn <strong>Add</strong> để lưu</li></ol></td></tr></tbody></table>

<div><figure><img src="../../.gitbook/assets/image (950).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (951).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Kiểm tra thông tin&#x20;**<mark style="color:$primary;">**Category, Product - Main course**</mark>**&#x20;và&#x20;**<mark style="color:$primary;">**Price**</mark>

Sau khi cập nhật danh sách sản phẩm trong nhóm, người dùng kiểm tra các thông tin hệ thống tự hiển thị dưới đây:

<table><thead><tr><th width="226">Trường thông tin</th><th>Cách xử lý</th></tr></thead><tbody><tr><td>Category</td><td>Hệ thống tự động cập nhật tổng hợp các chương trình học của sản phẩm trong nhóm</td></tr><tr><td>Product - Main course</td><td>Hệ thống tự động cập nhật dựa trên các sản phẩm user đã thêm vào Combo</td></tr><tr><td>Price</td><td>Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm</td></tr></tbody></table>
{% endstep %}

{% step %}
**Cập nhật&#x20;**<mark style="color:$primary;">**Status**</mark>**&#x20;của nhóm sản phẩm (nếu cần)**

Tại trường **Status**, chọn trạng thái của nhóm sản phẩm.

<table><thead><tr><th width="93.66668701171875">Giá trị</th><th>Ý nghĩa</th></tr></thead><tbody><tr><td>Active</td><td>Nhóm sản phẩm vẫn đang được kinh doanh</td></tr><tr><td>Inactive</td><td>Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới</td></tr></tbody></table>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Save**</mark>**&#x20;để lưu thông tin chỉnh sửa**

Sau khi cập nhật đầy đủ thông tin cần thay đổi, chọn <mark style="color:$primary;">**Save**</mark> để lưu thông tin.

→ Kết quả mong đợi:

* Hệ thống lưu thông tin đã chỉnh sửa của nhóm sản phẩm.
* Thông tin mới của nhóm sản phẩm được cập nhật trên hệ thống.

<figure><img src="../../.gitbook/assets/image (952).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa nhóm sản phẩm</summary>

{% stepper %}
{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Combo**</mark>**&#x20;cần xóa, chọn&#x20;**<mark style="color:$primary;">**Action > Delete**</mark>**.**

Tại màn hình danh sách nhóm sản phẩm **Combo Products**, tìm nhóm sản phẩm cần xóa. Sau đó, chọn **Action > Delete**.

<figure><img src="../../.gitbook/assets/image (953).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận thao tác xóa**

<figure><img src="../../.gitbook/assets/image (954).png" alt=""><figcaption></figcaption></figure>

Tại hộp thoại xác nhận, user chọn <mark style="color:$primary;">**Yes**</mark> để đồng ý xóa Combo.

→ Kết quả mong đợi:

* Hệ thống xóa Combo khỏi danh sách;
* Combo đã xóa không còn hiển thị trên màn hình danh sách ;
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.
{% endstep %}

{% step %}
**Kiểm tra kết quả sau khi xóa**

Sau khi xác nhận xóa, người dùng kiểm tra lại danh sách nhóm sản phẩm.

→ Kết quả mong đợi:

* Nhóm sản phẩm vừa xóa không còn xuất hiện trên danh sách nhóm sản phẩm.
* Các đơn hàng đã tạo trước đó có chứa nhóm sản phẩm này vẫn được giữ nguyên thông tin.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" icon="1" %}
### Lưu ý quan trọng

1. Khi thêm <mark style="color:$primary;">**Product**</mark> vào Combo: chỉ có thể thêm các sản phẩm có cùng Category
2. Khi đổi trạng thái combo sản phẩm từ <mark style="color:$primary;">**Active**</mark> sang <mark style="color:$primary;">**Inactive**</mark>:

* User không thêm được nhóm sản phẩm vào đơn hàng mới,
* Các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái không bị ảnh hưởng.

3. Khi tạo mới hoặc chỉnh sửa nhóm sản phẩm: <mark style="color:$primary;">Category, Main course</mark> và <mark style="color:$primary;">Price</mark> được hệ thống tự động cập nhật
4. Khi xóa sản phẩm, sản phẩm sẽ bị xóa khỏi:

* <mark style="color:$primary;">Combo Products</mark> có chứa sản phẩm đó
* Mã khuyến mại <mark style="color:$primary;">Promotion Codes</mark> đã gắn với sản phẩm trước đó
{% endhint %}

{% hint style="info" icon="2" %}
### Mẹo sử dụng

1. Khi tìm kiếm, có thể kết hợp nhiều điều kiện tìm kiếm để thu hẹp kết quả nhanh hơn
{% endhint %}

## IV. Các lỗi thường gặp & Cách xử lý

| Lỗi hoặc tình huống                     | Nguyên nhân                                     | Cách xử lý                                                         |
| --------------------------------------- | ----------------------------------------------- | ------------------------------------------------------------------ |
| Không tìm thấy dữ liệu                  | Sai điều kiện tìm kiếm                          | Kiểm tra lại bộ lọc tìm kiếm                                       |
| Không truy cập được menu Combo Products | Chưa được cấp quyền                             | Liên hệ quản trị hệ thống                                          |
| This field is required                  | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ **Combo name**, **Products** và **Status** |

## V. Câu hỏi thường gặp

<table><thead><tr><th width="143.66668701171875">Bối cảnh</th><th>Câu hỏi</th><th>Câu trả lời</th></tr></thead><tbody><tr><td></td><td>Price của nhóm sản phẩm được hiểu như thế nào?</td><td><mark style="color:$primary;"><strong>Price</strong></mark> là tổng giá trị của các sản phẩm trong nhóm.</td></tr><tr><td></td><td>Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Nhóm sản phẩm ở trạng thái <strong>Inactive</strong> sẽ không được thêm vào đơn hàng mới.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Có cần nhập Category khi tạo nhóm sản phẩm không?</td><td><mark style="color:$danger;"><strong>Không.</strong></mark> Hệ thống tự tổng hợp <strong>Category</strong> từ chương trình học của từng sản phẩm trong nhóm.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Có cần nhập Price khi tạo nhóm sản phẩm không?</td><td><mark style="color:$danger;"><strong>Không.</strong></mark> Hệ thống tự tính <strong>Price</strong> bằng tổng giá trị của các sản phẩm trong nhóm.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Làm thế nào để thêm sản phẩm vào nhóm?</td><td>Tại trường <strong>Products</strong>, chọn vào vùng trống để mở danh sách sản phẩm. Sau đó chọn checkbox tại một hoặc nhiều sản phẩm và chọn <strong>Add</strong>.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Có thể thêm các sản phẩm Inactive vào nhóm sản phẩm không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Danh sách Products chỉ gồm các sản phẩm đang ở trạng thái Active.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Nhóm sản phẩm ở trạng thái <strong>Inactive</strong> sẽ không được thêm vào đơn hàng mới.</td></tr><tr><td>Tạo mới nhóm sản phẩm</td><td>Sau khi tạo mới, nhóm sản phẩm hiển thị ở đâu?</td><td>Nhóm sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách nhóm sản phẩm.</td></tr><tr><td>Chỉnh sửa nhóm sản phẩm</td><td>Khi thay đổi sản phẩm trong nhóm làm Price thay đổi thì đơn hàng cũ có bị ảnh hưởng không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ. Các đơn hàng trong tương lai có chứa nhóm sản phẩm sẽ áp dụng giá mới.</td></tr><tr><td>Chỉnh sửa nhóm sản phẩm</td><td>Việc đổi trạng thái nhóm sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Việc đổi trạng thái nhóm sản phẩm từ <strong>Active</strong> sang <strong>Inactive</strong> không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.</td></tr><tr><td>Xóa nhóm sản phẩm</td><td>Xóa nhóm sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.</td></tr><tr><td>Xóa nhóm sản phẩm</td><td>Có thể khôi phục nhóm sản phẩm đã xóa không?</td><td><mark style="color:$danger;"><strong>Không</strong></mark>. Combo đã bị xóa không thể được khôi phục.</td></tr></tbody></table>
