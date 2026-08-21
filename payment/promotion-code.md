# Promotion Code

Kết quả đạt được: Các mã khuyến mại được tạo ra để gắn cho sản phẩm/combo sản phẩm xác định và các đơn hàng.

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date  | Update Person | A,M,D | Change Description | Version |
| --------------- | ------------- | ----- | ------------------ | ------- |
| August 15, 2025 | Nhungdh       | A     | Create New         | 3.0.0   |

## I. Thông tin chung

### Đối tượng sử dụng

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/promotion-codes?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/promotion-codes?page_index=1\&page_size=10)

#### Phạm vi & Module liên quan

* **Module chính**: Promotion code
* **Module liên quan**: [Product](product.md), [Combo Product](combo.md), [List of Orders](order-list.md)
* **Hệ thống tích hợp**: Không có

### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Promotion Code.

## II. Hướng dẫn chi tiết

{% hint style="info" %}
Promotion Code là danh sách các mã khuyến mại được áp dụng cho:

1. Sản phẩm đơn lẻ
2. Nhóm sản phẩm
3. Đơn hàng
{% endhint %}

### Xem danh sách mã khuyến mại

{% stepper %}
{% step %}
## Truy cập màn hình danh sách mã khuyến mại

Tại thanh Menu, chọn vào mục Order & Payment **> Promotion Codes**.

→ Hệ thống chuyển đến màn hình danh sách các mã khuyến mại.

![](<../.gitbook/assets/image (422)>)

Danh sách mã khuyến mại hiển thị các thông tin dưới đây:

| Thông tin          | Ý nghĩa                                                                                              |
| ------------------ | ---------------------------------------------------------------------------------------------------- |
| Code               | Mã khuyến mại                                                                                        |
| Total              | Tổng số lượng mã khuyến mại                                                                          |
| Reserved           | Số lượng mã khuyến mãi được sử dụng trong các Order chưa được thanh toán                             |
| Start - End        | Hiệu lực của mã khuyến mại                                                                           |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                                              |
| Apply for Combos   | Các combo được áp dụng mã khuyến mại                                                                 |
| Status             | <p>- Active: mã khuyến mại còn thời gian sử dụng<br>- Inactive: mã khuyến mại đã hết hạn sử dụng</p> |
{% endstep %}

{% step %}
## Tìm kiếm promotion code theo điều kiện

Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* Tên mã khuyến mại (Code name)
* Chương trình học (Category): chọn 1 giá trị trong danh sách cho trước.
* Trạng thái (Status): chọn 1 giá trị trong danh sách cho trước.
* Cách sắp xếp của danh sách (Sort by): chọn 1 giá trị trong danh sách cho trước.
* Thời gian hiệu lực (Start - End)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

![](<../.gitbook/assets/image (423)>)

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo.
{% endstep %}
{% endstepper %}

### Xem chi tiết mã khuyến mại

{% stepper %}
{% step %}
## Chọn mã khuyến mãi cần xem chi tiết

Tại màn hình danh sách mã khuyến mại, click vào giá trị tại cột **Code**.

![](<../.gitbook/assets/image (424)>)
{% endstep %}

{% step %}
## Xem thông tin chung của mã khuyến mại

Tại khu vực **Overview**, người dùng xem các thông tin sau:

| Thông tin          | Mô tả                                                                                                                 |
| ------------------ | --------------------------------------------------------------------------------------------------------------------- |
| Code               | Mã khuyến mại                                                                                                         |
| Quantity           | Tổng số lượng mã khuyến mại                                                                                           |
| Start - End        | Thời gian hiệu lực của mã khuyến mại                                                                                  |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                                                               |
| Apply for Combos   | Các nhóm sản phẩm được áp dụng mã khuyến mại                                                                          |
| Discount           | Lượng giảm giá của mã khuyến mại, bao gồm: 1. Theo % giá trị đơn hàng 2. Theo số tiền cụ thể                          |
| Combined With      | Các mã giảm giá được kết hợp cùng mã này → cho phép sử dụng nhiều mã khuyến mãi cho cùng 1 Product hoặc Combo product |

![](<../.gitbook/assets/image (425)>)
{% endstep %}

{% step %}
## Chuyển tab **List Orders** → Xem danh sách đơn hàng sử dụng mã khuyến mại

Người dùng xem danh sách các đơn hàng đã sử dụng mã khuyến mại, với các thông tin hiển thị như sau:

| Thông tin | Mô tả                                                                                                                                                         |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Product   | Tên sản phẩm sử dụng mã khuyến mại                                                                                                                            |
| Combo     | Tên nhóm sản phẩm sử dụng mã khuyến mại                                                                                                                       |
| Customer  | Khách hàng                                                                                                                                                    |
| Deal ID   | Mã Deal trên Hubspot của khách hàng                                                                                                                           |
| Price     | Giá trị sản phẩm sau khi áp dụng mã khuyến mại                                                                                                                |
| Status    | <p>Trạng thái của đơn hàng, bao gồm:<br><br>- Chờ thanh toán<br>- Đang thanh toán<br>- Đã thanh toán một phần<br>- Đã thanh toán<br>- Hết hạn<br>- Đã hủy</p> |

![](<../.gitbook/assets/image (426)>)
{% endstep %}

{% step %}
## Hoàn tất

User đã xem chi tiết toàn bộ thông tin về mã khuyến mại.
{% endstep %}
{% endstepper %}

### Tạo mới mã khuyến mại

User có thể thực hiện tạo mã khuyến mãi áp dụng cho:

* Sản phẩm hoặc nhóm sản phẩm
* Đơn hàng

#### A. Tạo mới mã khuyến mại áp dụng cho sản phẩm hoặc nhóm sản phẩm

{% stepper %}
{% step %}
## Tại màn hình danh sách mã khuyến mại > Chọn **New Promotion Code**

![](<../.gitbook/assets/image (427)>)

Sau đó, hệ thống hiển thị màn hình tạo mới mã khuyến mại.

![](<../.gitbook/assets/image (428)>)
{% endstep %}

{% step %}
## Tại trường **Apply Option**, chọn **Apply for Product + Combo**

Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng theo sản phẩm hoặc nhóm sản phẩm.

![](<../.gitbook/assets/image (429)>)
{% endstep %}

{% step %}
## Nhập thông tin chung của mã khuyến mại

User nhập các thông tin sau:

| Trường thông tin     | Hướng dẫn nhập                                                                | Lưu ý                                                              |
| -------------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Code\*               | Nhập tên mã khuyến mại                                                        |                                                                    |
| Quantity\*           | Nhập số lượng mã khuyến mại                                                   | Không cập nhật trong trường hợp chọn checkbox No quantity required |
| No quantity required | Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng |                                                                    |
| Start - End          | Chọn thời gian hiệu lực của mã khuyến mại                                     |                                                                    |
| Discount\*           | Nhập lượng giảm giá của mã khuyến mại                                         |                                                                    |
| Combined with        | Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo           |                                                                    |

![](<../.gitbook/assets/image (430)>)
{% endstep %}

{% step %}
## Chọn sản phẩm được áp dụng mã khuyến mại

Tại trường Apply for Product, chọn để mở danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, user thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách sản phẩm đã chọn.

![](<../.gitbook/assets/image (431)>)
{% endstep %}

{% step %}
## Chọn nhóm sản phẩm được áp dụng mã khuyến mại

Tại trường Apply for Combo, chọn để mở danh sách nhóm sản phẩm.

Trên màn hình danh sách nhóm sản phẩm, người dùng thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các nhóm sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách nhóm sản phẩm đã chọn.

![](<../.gitbook/assets/image (432)>)

![](<../.gitbook/assets/image (433)>)
{% endstep %}

{% step %}
## Chọn loại **Discount** và nhập lượng giảm giá

Tại trường Discount, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |

![](<../.gitbook/assets/image (434)>)
{% endstep %}

{% step %}
## Chọn **Save** để lưu mã khuyến mại

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

![](<../.gitbook/assets/image (435)>)
{% endstep %}
{% endstepper %}

#### B. Tạo mới mã khuyến mại áp dụng cho đơn hàng

{% stepper %}
{% step %}
## Tại màn hình danh sách mã khuyến mại > Chọn **New Promotion Code**

![](<../.gitbook/assets/image (436)>)

Sau đó, hệ thống hiển thị màn hình tạo mới mã khuyến mại.

![](<../.gitbook/assets/image (437)>)
{% endstep %}

{% step %}
## Tại trường **Apply Option**, chọn **Apply for Order**

Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng cho đơn hàng.

![](<../.gitbook/assets/image (438)>)
{% endstep %}

{% step %}
## Nhập thông tin chung của mã khuyến mại

User nhập các thông tin sau:

| Trường thông tin     | Hướng dẫn nhập                                                                | Lưu ý                                                              |
| -------------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Code\*               | Nhập tên mã khuyến mại                                                        |                                                                    |
| Quantity\*           | Nhập số lượng mã khuyến mại                                                   | Không cập nhật trong trường hợp chọn checkbox No quantity required |
| No quantity required | Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng |                                                                    |
| Start - End          | Chọn thời gian hiệu lực của mã khuyến mại                                     |                                                                    |
| Discount\*           | Nhập lượng giảm giá của mã khuyến mại                                         |                                                                    |
| Combined with        | Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo           |                                                                    |

![](<../.gitbook/assets/image (439)>)
{% endstep %}

{% step %}
## Chọn loại **Discount** và nhập lượng giảm giá

Tại trường Discount, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |
{% endstep %}

{% step %}
## Chọn **Save** để lưu mã khuyến mại

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

![](<../.gitbook/assets/image (440)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa mã khuyến mại

{% stepper %}
{% step %}
## Truy cập màn hình chỉnh sửa mã khuyến mại

Tại màn hình danh sách Promotion Codes, user có thể truy cập màn hình chỉnh sửa mã khuyến mại bằng 1 trong 2 cách dưới đây:

* **Cách 1:** Chọn **Code > Edit Promotion Code** của mã khuyến mại cần chỉnh sửa.

![](<../.gitbook/assets/image (441)>)

* **Cách 2**: Chọn **Action > Edit** tại nhóm sản phẩm cần chỉnh sửa.

![](<../.gitbook/assets/image (442)>)
{% endstep %}

{% step %}
## Cập nhật các thông tin muốn thay đổi cho mã khuyến mại

User nhập hoặc chỉnh sửa các thông tin cần cập nhật dưới đây:

| Trường thông tin     | Hướng dẫn chỉnh sửa                                                                                                                                                           |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Code\*               | Tên mã                                                                                                                                                                        |
| Quantity\*           | Số lượng mã khuyến mại                                                                                                                                                        |
| No quantity required | Chọn checkbox này để không giới hạn số lượng mã giảm giá được dùng, và lúc này cũng không cần điền thông tin về Quantity                                                      |
| Start - End\*        | Hiệu lực của mã khuyến mại                                                                                                                                                    |
| Apply for Product\*  | Các sản phẩm được áp dụng mã khuyến mại. Click để chuyển đến màn hình danh sách các sản phầm, thực hiện chọn các sản phẩm bằng cách **chọn/bỏ chọn checkbox > Select** để lưu |
| Apply for Combo\*    | Các combo được áp dụng mã khuyến mại. Click để chuyển đến màn hình danh sách các combo, thực hiện chọn các nhóm sản phẩm bằng cách **chọn/bỏ chọn checkbox > Select** để lưu  |
| Discount\*           | <p>Lượng giảm giá, bao gồm:<br><br>- Theo số tiền cụ thể, đơn vị VND (Fixed)<br>- Theo phần trăm giá trị đơn hàng (Percentage)</p>                                            |
| Combine with         | Các mã giảm giá có thể dùng kết hợp với mã giảm giá đang tạo                                                                                                                  |

{% hint style="info" %}
Đối với Apply for Product và Apply for Combo, người dùng chỉ cần điền 1 trong 2, không bắt buộc phải điền cả 2 thông tin.

Việc chỉnh sửa mã giảm giá sẽ không ảnh hưởng đến giá trị các đơn hàng đã được tạo trước đó mà có gắn với mã giảm giá.
{% endhint %}
{% endstep %}

{% step %}
## Chọn **Save** để lưu thông tin cập nhật

Sau khi cập nhật thông tin cần chỉnh sửa, chọn **Save** để lưu thông tin.

→ Hệ thống lưu thông tin đã chỉnh sửa của mã và quay lại màn Danh sách khuyến mại.

![](<../.gitbook/assets/image (443)>)
{% endstep %}
{% endstepper %}

### Xóa mã khuyến mại

{% stepper %}
{% step %}
## Tại màn hình Danh sách, chọn mã muốn xóa → nút **Action > Delete**

Hệ thống hiển thị hộp thoại xác nhận xóa mã khuyến mại → User có thể chọn tiếp tục xóa hoặc hủy thao tác.

![](<../.gitbook/assets/image (444)>)

![](<../.gitbook/assets/image (445)>)
{% endstep %}

{% step %}
## Xác nhận thao tác xóa trên hộp thoại

Tại hộp thoại xác nhận, user chọn **Yes** để đồng ý xóa sản phẩm.

![](<../.gitbook/assets/image (446)>)

{% hint style="warning" %}
Không thể xóa các mã khuyến mại đã được áp dụng trong đơn hàng.
{% endhint %}
{% endstep %}

{% step %}
## Kiểm tra kết quả sau xóa

Sau khi xác nhận xóa, user kiểm tra lại danh sách mã khuyến mại.

→ Kết quả mong đợi: Mã khuyến mại vừa xóa không còn xuất hiện trên danh sách Promotion Code.
{% endstep %}
{% endstepper %}

## III. Lưu ý & Quy tắc nghiệp vụ

### Lưu ý quan trọng

1. Khi thêm mới hoặc chỉnh sửa mã khuyến mại:
   * Đối với Apply for Product và Apply for Combo, user chỉ cần điền 1 trong 2, không bắt buộc điền cả hai thông tin.
   * Việc chỉnh sửa mã khuyến mại không ảnh hưởng đến giá trị của các đơn hàng đã được tạo trước đó được gắn với mã khuyến mại.
2. Khi xóa mã khuyến mại, nếu mã đang được gắn với đơn hàng → User không thể xóa mã khuyến mại này.
