---
description: >-
  Kết quả đạt được: Các mã khuyến mại được tạo ra để gắn cho sản phẩm/combo sản
  phẩm xác định và các đơn hàng
---

# Promotion Code

## Record of changes

\*A - Add M - Modify D - Delete

<table><thead><tr><th width="147.99993896484375">Effective Date</th><th width="146.66668701171875">Update Person</th><th width="92.6666259765625">A,M,D</th><th width="296.0001220703125">Change Description</th><th>Version</th></tr></thead><tbody><tr><td>August 15, 2025</td><td>Nhungdh</td><td>A</td><td>Create New</td><td>3.0.0</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="info" icon="1" %}
### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/promotion-codes?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/promotion-codes?page_index=1\&page_size=10)
{% endhint %}

{% hint style="warning" icon="2" %}
#### Phạm vi & Module liên quan <a href="#id-1.3-pham-vi-and-module-lien-quan" id="id-1.3-pham-vi-and-module-lien-quan"></a>

* **Module chính**: Promotion code
* **Module liên quan**: [Product](../product/), [Combo Product](../combo/), [List of Orders](../order-list/)
* **Hệ thống tích hợp**: Không có
{% endhint %}

{% hint style="success" icon="3" %}
### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Promotion Code.
{% endhint %}

## II. Hướng dẫn chi tiết

> Promotion Code là danh sách các mã khuyến mại được áp dụng cho:
>
> 1. Sản phẩm đơn lẻ
> 2. Nhóm sản phẩm
> 3. Đơn hàng

<details>

<summary>Xem danh sách mã khuyến mại</summary>

{% stepper %}
{% step %}
**Truy cập màn hình danh sách mã khuyến mại**

Tại thanh Menu, chọn vào mục <mark style="color:$primary;">Order & Payment</mark> <mark style="color:$primary;">**> Promotion Codes**</mark>

→ Hệ thống chuyển đến màn hình danh sách các mã khuyến mại

<figure><img src="../../.gitbook/assets/image (1063).png" alt=""><figcaption></figcaption></figure>

Danh sách mã khuyến mại hiển thị các thông tin dưới đây:

| Thông tin          | Ý nghĩa                                                                                                                                                                                    |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Code               | Mã khuyến mại                                                                                                                                                                              |
| Total              | Tổng số lượng mã khuyến mại                                                                                                                                                                |
| Reserved           | Số lượng mã khuyến mãi được sử dụng trong các Order chưa được thanh toán                                                                                                                   |
| Start - End        | Hiệu lực của mã khuyến mại                                                                                                                                                                 |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                                                                                                                                    |
| Apply for Combos   | Các combo được áp dụng mã khuyến mại                                                                                                                                                       |
| Status             | <ul><li><mark style="color:$primary;">Active</mark>: mã khuyến mại còn thời gian sử dụng</li><li><mark style="color:$primary;">Inactive</mark>: mã khuyến mại đã hết hạn sử dụng</li></ul> |
{% endstep %}

{% step %}
**User có thể tìm kiếm promotion code theo điều kiện**

Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* Tên mã khuyến mại (Code name)
* Chương trình học (Category): chọn 1 giá trị trong danh sách cho trước.
* Trạng thái (Status): chọn 1 giá trị trong danh sách cho trước.
* Cách sắp xếp của danh sách (Sort by): chọn 1 giá trị trong danh sách cho trước.
* Thời gian hiệu lực (Start - End)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

<figure><img src="../../.gitbook/assets/image (1062).png" alt=""><figcaption></figcaption></figure>

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết mã khuyến mại</summary>

{% stepper %}
{% step %}
**Chọn mã khuyến mãi cần xem chi tiết**

Tại màn hình danh sách mã khuyến mại, click vào giá trị tại cột <mark style="color:$primary;">**Code**</mark>

<figure><img src="../../.gitbook/assets/image (1065).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin chung của mã khuyến mại**

Tại khu vực **Overview**, người dùng xem các thông tin sau:

| Thông tin          | Mô tả                                                                                                                 |
| ------------------ | --------------------------------------------------------------------------------------------------------------------- |
| Code               | Mã khuyến mại                                                                                                         |
| Quantity           | Tổng số lượng mã khuyến mại                                                                                           |
| Start - End        | Thời gian hiệu lực của mã khuyến mại                                                                                  |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                                                               |
| Apply for Combos   | Các nhóm sản phẩm được áp dụng mã khuyến mại                                                                          |
| Discount           | <p>Lượng giảm giá của mã khuyến mại, bao gồm:<br>1. Theo % giá trị đơn hàng<br>2. Theo số tiền cụ thể</p>             |
| Combined With      | Các mã giảm giá được kết hợp cùng mã này → cho phép sử dụng nhiều mã khuyến mãi cho cùng 1 Product hoặc Combo product |

<figure><img src="../../.gitbook/assets/image (340).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chuyển tab&#x20;**<mark style="color:$primary;">**List Orders**</mark>**&#x20;→ Xem danh sách đơn hàng sử dụng mã khuyến mại**

Người dùng xem danh sách các đơn hàng đã sử dụng mã khuyến mại, với các thông tin hiển thị như sau:

| Thông tin | Mô tả                                                                                                                                                                                |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Product   | Tên sản phẩm sử dụng mã khuyến mại                                                                                                                                                   |
| Combo     | Tên nhóm sản phẩm sử dụng mã khuyến mại                                                                                                                                              |
| Customer  | Khách hàng                                                                                                                                                                           |
| Deal ID   | Mã Deal trên Hubspot của khách hàng                                                                                                                                                  |
| Price     | Giá trị sản phẩm sau khi áp dụng mã khuyến mại                                                                                                                                       |
| Status    | <p>Trạng thái của đơn hàng, bao gồm:</p><ul><li>Chờ thanh toán</li><li>Đang thanh toán</li><li>Đã thanh toán một phần</li><li>Đã thanh toán</li><li>Hết hạn</li><li>Đã hủy</li></ul> |

<figure><img src="../../.gitbook/assets/image (341).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hoàn tất**

User đã xem chi tiết toàn bộ thông tin về mã khuyến mại
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới mã khuyến mại</summary>

User có thể thực hiện tạo mã khuyến mãi áp dụng cho:

* Sản phẩm hoặc nhóm sản phẩm
* Đơn hàng

<mark style="color:blue;">**A.**</mark> <mark style="color:blue;">**Tạo mới mã khuyến mại áp dụng cho sản phẩm hoặc nhóm sản phẩm**</mark>

{% stepper %}
{% step %}
**Tại màn hình danh sách mã khuyến mại > Chọn&#x20;**<mark style="color:$primary;">**New Promotion Code**</mark>

<figure><img src="../../.gitbook/assets/image (1068).png" alt=""><figcaption></figcaption></figure>

Sau đó, hệ thống hiển thị màn hình tạo mới mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (1069).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tại trường&#x20;**<mark style="color:$primary;">**Apply Option**</mark>**, chọn&#x20;**<mark style="color:$primary;">**Apply for Product + Combo**</mark>

Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng theo sản phẩm hoặc nhóm sản phẩm.

<figure><img src="../../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin chung của mã khuyến mại**

User nhập các thông tin sau:

<table><thead><tr><th width="191.33331298828125">Trường thông tin</th><th width="220.33331298828125">Hướng dẫn nhập</th><th>Lưu ý</th></tr></thead><tbody><tr><td>Code<mark style="color:$danger;">*</mark></td><td>Nhập tên mã khuyến mại</td><td></td></tr><tr><td>Quantity<mark style="color:$danger;">*</mark></td><td>Nhập số lượng mã khuyến mại</td><td>Không cập nhật trong trường hợp chọn checkbox <mark style="color:$danger;">No quantity required</mark></td></tr><tr><td>No quantity required</td><td>Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng</td><td></td></tr><tr><td>Start - End</td><td>Chọn thời gian hiệu lực của mã khuyến mại</td><td></td></tr><tr><td>Discount<mark style="color:$danger;">*</mark></td><td>Nhập lượng giảm giá của mã khuyến mại</td><td></td></tr><tr><td>Combined with</td><td>Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo</td><td></td></tr></tbody></table>

<figure><img src="../../.gitbook/assets/image (367).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn sản phẩm được áp dụng mã khuyến mại**

Tại trường <mark style="color:$primary;">Apply for Product</mark>, chọn để mở danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, user thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách sản phẩm đã chọn.

<figure><img src="../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn nhóm sản phẩm được áp dụng mã khuyến mại**

Tại trường <mark style="color:$primary;">Apply for Combo</mark>, chọn để mở danh sách nhóm sản phẩm.

Trên màn hình danh sách nhóm sản phẩm, người dùng thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các nhóm sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách nhóm sản phẩm đã chọn.

<div><figure><img src="../../.gitbook/assets/image (370).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1006).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Chọn loại&#x20;**<mark style="color:$primary;">**Discount**</mark>**&#x20;và nhập lượng giảm giá**

Tại trường <mark style="color:$primary;">Discount</mark>, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |

<figure><img src="../../.gitbook/assets/image (372).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Save**</mark>**&#x20;để lưu mã khuyến mại**

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

<figure><img src="../../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

<mark style="color:blue;">**B. Tạo mới mã khuyến mại áp dụng cho đơn hàng**</mark>

{% stepper %}
{% step %}
**Tại màn hình danh sách mã khuyến mại > Chọn&#x20;**<mark style="color:$primary;">**New Promotion Code**</mark>

<figure><img src="../../.gitbook/assets/image (1009).png" alt=""><figcaption></figcaption></figure>

Sau đó, hệ thống hiển thị màn hình tạo mới mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (1010).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tại trường&#x20;**<mark style="color:$primary;">**Apply Option,**</mark>**&#x20;chọn&#x20;**<mark style="color:$primary;">**Apply for Order**</mark>

Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng cho đơn hàng.

<figure><img src="../../.gitbook/assets/image (375).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin chung của mã khuyến mại**

User nhập các thông tin sau:

<table><thead><tr><th width="191.33331298828125">Trường thông tin</th><th width="220.33331298828125">Hướng dẫn nhập</th><th>Lưu ý</th></tr></thead><tbody><tr><td>Code<mark style="color:$danger;">*</mark></td><td>Nhập tên mã khuyến mại</td><td></td></tr><tr><td>Quantity<mark style="color:$danger;">*</mark></td><td>Nhập số lượng mã khuyến mại</td><td>Không cập nhật trong trường hợp chọn checkbox <mark style="color:$danger;">No quantity required</mark></td></tr><tr><td>No quantity required</td><td>Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng</td><td></td></tr><tr><td>Start - End</td><td>Chọn thời gian hiệu lực của mã khuyến mại</td><td></td></tr><tr><td>Discount<mark style="color:$danger;">*</mark></td><td>Nhập lượng giảm giá của mã khuyến mại</td><td></td></tr><tr><td>Combined with</td><td>Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo</td><td></td></tr></tbody></table>

<figure><img src="../../.gitbook/assets/image (376).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn loại&#x20;**<mark style="color:$primary;">**Discount**</mark>**&#x20;và nhập lượng giảm giá**

Tại trường <mark style="color:$primary;">Discount</mark>, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Save**</mark>**&#x20;để lưu mã khuyến mại**

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

<figure><img src="../../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa mã khuyến mại</summary>

{% stepper %}
{% step %}
### Truy cập màn hình chỉnh sửa mã khuyến mại

Tại màn hình danh sách Promotion Codes, user có thể truy cập màn hình chỉnh sửa mã khuyến mại bằng 1 trong 2 cách dưới đây:

* **Cách 1:** Chọn <mark style="color:$primary;">**Code > Edit Promotion Code**</mark> của mã khuyến mại cần chỉnh sửa

<figure><img src="../../.gitbook/assets/image (1014).png" alt=""><figcaption></figcaption></figure>

* **Cách 2**: Chọn <mark style="color:$primary;">**Action > Edit**</mark> tại nhóm sản phẩm cần chỉnh sửa

<figure><img src="../../.gitbook/assets/image (1015).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật các thông tin muốn thay đổi cho mã khuyến mại**

User nhập hoặc chỉnh sửa các thông tin cần cập nhật dưới đây:

<table><thead><tr><th width="204">Trường thông tin</th><th>Hướng dẫn chỉnh sửa</th></tr></thead><tbody><tr><td>Code<mark style="color:$danger;">*</mark></td><td>Tên mã</td></tr><tr><td>Quantity<mark style="color:$danger;">*</mark></td><td>Số lượng mã khuyến mại</td></tr><tr><td>No quantity required</td><td>Chọn checkbox này để không giới hạn số lượng mã giảm giá được dùng, và lúc này cũng không cần điền thông tin về Quantity</td></tr><tr><td>Start - End<mark style="color:$danger;">*</mark></td><td>Hiệu lực của mã khuyến mại</td></tr><tr><td>Apply for Product<mark style="color:$danger;">*</mark></td><td>Các sản phẩm được áp dụng mã khuyến mại<br><br>Click để chuyển đến màn hình danh sách các sản phầm, thực hiện chọn các sản phẩm bằng cách <strong>chọn/bỏ chọn checkbox > Select</strong> để lưu</td></tr><tr><td>Apply for Combo<mark style="color:$danger;">*</mark></td><td>Các combo được áp dụng mã khuyến mại<br><br>Click để chuyển đến màn hình danh sách các combo, thực hiện chọn các nhóm sản phẩm bằng cách <strong>chọn/bỏ chọn checkbox > Select</strong> để lưu</td></tr><tr><td>Discount<mark style="color:$danger;">*</mark></td><td><p>Lượng giảm giá, bao gồm:<br></p><ul><li>Theo số tiền cụ thể, đơn vị VND (Fixed)</li><li>Theo phần trăm giá trị đơn hàng (Percentage)</li></ul></td></tr><tr><td>Combine with</td><td>Các mã giảm giá có thể dùng kết hợp với mã giảm giá đang tạo</td></tr></tbody></table>

{% hint style="info" %}
Đối với Apply for Product và Apply for Combo, người dùng chỉ cần điền 1 trong 2, không bắt buộc phải điền cả 2 thông tin.

Việc chỉnh sửa mã giảm giá sẽ không ảnh hưởng đến giá trị các đơn hàng đã được tạo trước đó mà có gắn với mã giảm giá.
{% endhint %}
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Save**</mark>**&#x20;để lưu thông tin cập nhật**

Sau khi cập nhật thông tin cần chỉnh sửa, chọn <mark style="color:$primary;">**Save**</mark> để lưu thông tin.

→ Hệ thống lưu thông tin đã chỉnh sửa của mã và quay lại màn Danh sách khuyến mại.

<figure><img src="../../.gitbook/assets/image (1016).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa mã khuyến mại</summary>

{% stepper %}
{% step %}
**Tại màn hình Danh sách, chọn mã muốn xóa → nút&#x20;**<mark style="color:$primary;">**Action > Delete**</mark>

Hệ thống hiển thị hộp thoại xác nhận xóa mã khuyến mại → User có thể chọn tiếp tục xóa hoặc hủy thao tác.

<div><figure><img src="../../.gitbook/assets/image (1017).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1019).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Xác nhận thao tác xóa trên hộp thoại**

Tại hộp thoại xác nhận, user chọn <mark style="color:$primary;">**Yes**</mark> để đồng ý xóa sản phẩm.

<figure><img src="../../.gitbook/assets/image (1020).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Lưu ý: Không thể xóa các mã khuyến mại đã được áp dụng trong đơn hàng
{% endhint %}
{% endstep %}

{% step %}
**Kiểm tra kết quả sau xóa**

Sau khi xác nhận xóa, user kiểm tra lại danh sách mã khuyến mại.

→ Kết quả mong đợi: Mã khuyến mại vừa xóa không còn xuất hiện trên danh sách Promotion Code.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" icon="1" %}
### Lưu ý quan trọng

1. Khi thêm mới hoặc chỉnh sửa mã khuyến mại:

* Đối với Apply for Product và Apply for Combo, user chỉ cần điền 1 trong 2, không bắt buộc điền cả hai thông tin.
* Việc chỉnh sửa mã khuyến mại không ảnh hưởng đến giá trị của các đơn hàng đã được tạo trước đó được gắn với mã khuyến mại

2. Khi xóa mã khuyến mại, nếu mã đang được gắn với đơn hàng → User không thể xóa mã khuyến mại này
{% endhint %}
