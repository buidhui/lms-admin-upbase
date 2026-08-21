# Combo

Kết quả đạt được: Các nhóm sản phẩm được tạo ra từ các Products sẵn sàng để gắn vào các Orders

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date  | Update Person | A,M,D | Change Description       | Version |
| --------------- | ------------- | ----- | ------------------------ | ------- |
| August 15, 2025 | Nhungdh       | A     | Create New               | 3.0.0   |
| June 8, 2026    | Nhungnth      | M     | Cập nhật tính năng Combo | 3.1.0   |

## I. Thông tin chung

### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/combo-products?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/combo-products?page_index=1\&page_size=10)

#### Phạm vi & Module liên quan

* **Module chính**: Combo Product
* **Module liên quan**: [Program & Subject](/broken/pages/60d8ad886d1deb674dc83f513d97c407496f5c4d), [Product](product.md), [Promotion Codes](promotion-code.md), [List of Orders](order-list.md)
* **Hệ thống tích hợp**: Không có

### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Combo.

## II. Hướng dẫn chi tiết

{% hint style="info" %}
Combo Product là danh sách các nhóm sản phẩm, được sử dụng để gắn vào các Orders. Combo Product được tạo bằng các khóa học đơn lẻ thuộc cùng chương trình kết hợp với nhau.
{% endhint %}

### Xem danh sách nhóm sản phẩm

{% stepper %}
{% step %}
## Truy cập màn hình danh sách nhóm sản phẩm

Tại thanh Menu, chọn Order & Payment > Product & Combo > **Combo Products**.

→ Hệ thống chuyển đến màn hình danh sách Combo Products.

![](<../.gitbook/assets/image (398)>)

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
## Tìm kiếm nhóm sản phẩm theo điều kiện

Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* Search Combo: Theo tên nhóm sản phẩm
* Product: Theo một sản phẩm trong danh sách
* Category: Theo chương trình học
* Status: Theo trạng thái sản phẩm
* Sort by: Chọn cách sắp xếp sản phẩm (A-Z, Z-A, Lastest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

![](<../.gitbook/assets/image (400)>)

Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết nhóm sản phẩm

{% stepper %}
{% step %}
## Chọn nhóm sản phẩm cần xem chi tiết

Tại màn hình danh sách nhóm sản phẩm Combo Products, chọn **Combo Name** của nhóm sản phẩm cần xem.

![](<../.gitbook/assets/image (401)>)
{% endstep %}

{% step %}
## Hoàn tất

Hệ thống hiển thị màn hình chi tiết của nhóm sản phẩm tương ứng.

![](<../.gitbook/assets/image (404)>)

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

### Tạo mới nhóm sản phẩm

{% stepper %}
{% step %}
## Tại màn hình Combo Products, chọn New Combo

Hệ thống chuyển đến màn hình tạo mới nhóm sản phẩm.

![](<../.gitbook/assets/image (406)>)

![](<../.gitbook/assets/image (407)>)
{% endstep %}

{% step %}
## Nhập tên nhóm sản phẩm

Tại trường **Combo name**, nhập tên nhóm sản phẩm cần tạo (bắt buộc).

![](<../.gitbook/assets/image (409)>)
{% endstep %}

{% step %}
## Chọn sản phẩm vào nhóm

Tại trường **Products**, chọn vào vùng trống của trường để mở màn hình danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, user thực hiện:

* Chọn checkbox tại một hoặc nhiều sản phẩm cần thêm vào nhóm.
* Chọn **Add** để thêm các sản phẩm đã chọn vào nhóm.

![](<../.gitbook/assets/image (411)>)

![](<../.gitbook/assets/image (412)>)

{% hint style="info" %}
Lưu ý: Chỉ được chọn các sản phẩm thuộc cùng 1 chương trình (Category)
{% endhint %}
{% endstep %}

{% step %}
## Kiểm tra thông tin Category, Price và Product - Main course

Sau khi chọn sản phẩm vào nhóm, user kiểm tra các thông tin hệ thống tự hiển thị.

| Trường thông tin      | Cách xử lý                                                                               |
| --------------------- | ---------------------------------------------------------------------------------------- |
| Category              | Hệ thống cập nhật tự động Category của các sản phẩm được thêm vào Combo.                 |
| Product - Main course | Hệ thống cập nhật tự động theo Subject và Construction Mode của các sản phẩm trong Combo |
| Price                 | Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm.                          |

![](<../.gitbook/assets/image (413)>)
{% endstep %}

{% step %}
## Chọn Status của nhóm sản phẩm

Tại trường **Status**, chọn trạng thái của nhóm sản phẩm (bắt buộc).

| Giá trị  | Ý nghĩa                                                                                               |
| -------- | ----------------------------------------------------------------------------------------------------- |
| Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |
{% endstep %}

{% step %}
## Chọn Save để lưu thông tin nhóm sản phẩm

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

→ Kết quả mong đợi:

* Hệ thống lưu thông tin nhóm sản phẩm mới.
* Nhóm sản phẩm vừa tạo hiển thị ở đầu danh sách nhóm sản phẩm.

![](<../.gitbook/assets/image (415)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin nhóm sản phẩm

{% stepper %}
{% step %}
## Truy cập màn hình chỉnh sửa

Tại màn hình danh sách Combo Products, user có thể truy cập màn hình chỉnh sửa nhóm sản phẩm bằng 1 trong 2 cách dưới đây:

* **Cách 1:** Chọn **Combo Name** của nhóm sản phẩm cần chỉnh sửa
* **Cách 2**: Chọn **Action > Edit** tại nhóm sản phẩm cần chỉnh sửa

→ Hệ thống chuyển đến màn hình chỉnh sửa thông tin nhóm sản phẩm.

![](<../.gitbook/assets/image (416)>)
{% endstep %}

{% step %}
## Cập nhật Combo Name (nếu cần)

Tại trường **Combo name**, cập nhật tên nhóm sản phẩm nếu cần.

| Trường thông tin | Bắt buộc | Hướng dẫn chỉnh sửa        |
| ---------------- | -------- | -------------------------- |
| Combo name       | Có       | Cập nhật tên nhóm sản phẩm |

→ Tên nhóm sản phẩm mới được ghi nhận trên form chỉnh sửa
{% endstep %}

{% step %}
## Cập nhật danh sách Product trên Combo

User có thể Xóa, Thêm hoặc Chọn lại danh sách sản phẩm trong nhóm tương ứng như sau:

| Nhu cầu                                | Thao tác                                                                                                                                                                                                        |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Xóa sản phẩm khỏi nhóm                 | Chọn dấu **x** tại sản phẩm cần xóa                                                                                                                                                                             |
| Thêm hoặc chọn lại sản phẩm trong nhóm | <p>1. Chọn vào vùng trống của trường <strong>Products</strong> để mở màn hình danh sách sản phẩm.<br>2. Sau đó chọn hoặc bỏ chọn checkbox tại các sản phẩm cần thay đổi và chọn <strong>Add</strong> để lưu</p> |

![](<../.gitbook/assets/image (417)>)

![](<../.gitbook/assets/image (418)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin Category, Product - Main course và Price

Sau khi cập nhật danh sách sản phẩm trong nhóm, người dùng kiểm tra các thông tin hệ thống tự hiển thị dưới đây:

| Trường thông tin      | Cách xử lý                                                                      |
| --------------------- | ------------------------------------------------------------------------------- |
| Category              | Hệ thống tự động cập nhật tổng hợp các chương trình học của sản phẩm trong nhóm |
| Product - Main course | Hệ thống tự động cập nhật dựa trên các sản phẩm user đã thêm vào Combo          |
| Price                 | Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm                  |
{% endstep %}

{% step %}
## Cập nhật Status của nhóm sản phẩm (nếu cần)

Tại trường **Status**, chọn trạng thái của nhóm sản phẩm.

| Giá trị  | Ý nghĩa                                                                                               |
| -------- | ----------------------------------------------------------------------------------------------------- |
| Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |
{% endstep %}

{% step %}
## Chọn Save để lưu thông tin chỉnh sửa

Sau khi cập nhật đầy đủ thông tin cần thay đổi, chọn **Save** để lưu thông tin.

→ Kết quả mong đợi:

* Hệ thống lưu thông tin đã chỉnh sửa của nhóm sản phẩm.
* Thông tin mới của nhóm sản phẩm được cập nhật trên hệ thống.

![](<../.gitbook/assets/image (419)>)
{% endstep %}
{% endstepper %}

### Xóa nhóm sản phẩm

{% stepper %}
{% step %}
## Chọn Combo cần xóa, chọn Action > Delete

Tại màn hình danh sách nhóm sản phẩm **Combo Products**, tìm nhóm sản phẩm cần xóa. Sau đó, chọn **Action > Delete**.

![](<../.gitbook/assets/image (420)>)
{% endstep %}

{% step %}
## Xác nhận thao tác xóa

![](<../.gitbook/assets/image (421)>)

Tại hộp thoại xác nhận, user chọn **Yes** để đồng ý xóa Combo.

→ Kết quả mong đợi:

* Hệ thống xóa Combo khỏi danh sách;
* Combo đã xóa không còn hiển thị trên màn hình danh sách;
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.
{% endstep %}

{% step %}
## Kiểm tra kết quả sau khi xóa

Sau khi xác nhận xóa, người dùng kiểm tra lại danh sách nhóm sản phẩm.

→ Kết quả mong đợi:

* Nhóm sản phẩm vừa xóa không còn xuất hiện trên danh sách nhóm sản phẩm.
* Các đơn hàng đã tạo trước đó có chứa nhóm sản phẩm này vẫn được giữ nguyên thông tin.
{% endstep %}
{% endstepper %}

## III. Lưu ý & Quy tắc nghiệp vụ

### Lưu ý quan trọng

1. Khi thêm **Product** vào Combo: chỉ có thể thêm các sản phẩm có cùng Category.
2. Khi đổi trạng thái combo sản phẩm từ **Active** sang **Inactive**:
   * User không thêm được nhóm sản phẩm vào đơn hàng mới.
   * Các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái không bị ảnh hưởng.
3. Khi tạo mới hoặc chỉnh sửa nhóm sản phẩm: Category, Main course và Price được hệ thống tự động cập nhật.
4. Khi xóa sản phẩm, sản phẩm sẽ bị xóa khỏi:
   * Combo Products có chứa sản phẩm đó.
   * Mã khuyến mại Promotion Codes đã gắn với sản phẩm trước đó.

### Mẹo sử dụng

1. Khi tìm kiếm, có thể kết hợp nhiều điều kiện tìm kiếm để thu hẹp kết quả nhanh hơn.

## IV. Các lỗi thường gặp & Cách xử lý

| Lỗi hoặc tình huống                     | Nguyên nhân                                     | Cách xử lý                                                         |
| --------------------------------------- | ----------------------------------------------- | ------------------------------------------------------------------ |
| Không tìm thấy dữ liệu                  | Sai điều kiện tìm kiếm                          | Kiểm tra lại bộ lọc tìm kiếm                                       |
| Không truy cập được menu Combo Products | Chưa được cấp quyền                             | Liên hệ quản trị hệ thống                                          |
| This field is required                  | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ **Combo name**, **Products** và **Status** |

## V. Câu hỏi thường gặp

<details>

<summary>Price của nhóm sản phẩm được hiểu như thế nào?</summary>

**Price** là tổng giá trị của các sản phẩm trong nhóm.

</details>

<details>

<summary>Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?</summary>

**Không**. Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.

</details>

<details>

<summary>Có cần nhập Category khi tạo nhóm sản phẩm không?</summary>

**Không.** Hệ thống tự tổng hợp **Category** từ chương trình học của từng sản phẩm trong nhóm.

</details>

<details>

<summary>Có cần nhập Price khi tạo nhóm sản phẩm không?</summary>

**Không.** Hệ thống tự tính **Price** bằng tổng giá trị của các sản phẩm trong nhóm.

</details>

<details>

<summary>Làm thế nào để thêm sản phẩm vào nhóm?</summary>

Tại trường **Products**, chọn vào vùng trống để mở danh sách sản phẩm. Sau đó chọn checkbox tại một hoặc nhiều sản phẩm và chọn **Add**.

</details>

<details>

<summary>Có thể thêm các sản phẩm Inactive vào nhóm sản phẩm không?</summary>

**Không**. Danh sách Products chỉ gồm các sản phẩm đang ở trạng thái Active.

</details>

<details>

<summary>Sau khi tạo mới, nhóm sản phẩm hiển thị ở đâu?</summary>

Nhóm sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách nhóm sản phẩm.

</details>

<details>

<summary>Khi thay đổi sản phẩm trong nhóm làm Price thay đổi thì đơn hàng cũ có bị ảnh hưởng không?</summary>

**Không**. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ. Các đơn hàng trong tương lai có chứa nhóm sản phẩm sẽ áp dụng giá mới.

</details>

<details>

<summary>Việc đổi trạng thái nhóm sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?</summary>

**Không**. Việc đổi trạng thái nhóm sản phẩm từ **Active** sang **Inactive** không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.

</details>

<details>

<summary>Xóa nhóm sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?</summary>

**Không**. Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.

</details>

<details>

<summary>Có thể khôi phục nhóm sản phẩm đã xóa không?</summary>

**Không**. Combo đã bị xóa không thể được khôi phục.

</details>
