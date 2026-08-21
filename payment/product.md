# Product

Kết quả đạt được: Các sản phẩm đơn lẻ được tạo sẵn sàng để gắn vào các Combo Products hoặc Orders.

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date  | Update Person | A,M,D | Change Description         | Version |
| --------------- | ------------- | ----- | -------------------------- | ------- |
| August 15, 2025 | Nhungdh       | A     | Create New                 | 3.0.0   |
| June 8, 2026    | Nhungnth      | M     | Cập nhật tính năng Product | 3.1.0   |

## I. Thông tin chung

### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/products?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/products?page_index=1\&page_size=10)

#### Phạm vi & Module liên quan

* **Module chính**: Product
* **Module liên quan**: [Program & Subject](../khoa-hoc-course/program-and-subject.md), [Combo Product](combo.md), [Promotion Codes](promotion-code.md), [List of Orders](order-list.md)
* **Hệ thống tích hợp**: Không có

### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Product.

## II. Hướng dẫn chi tiết

> Products là danh sách các sản phẩm đơn lẻ, được gắn độc lập vào Orders hoặc được thêm vào các nhóm sản phẩm (Combo Products).

### Xem danh sách sản phẩm đơn lẻ

{% stepper %}
{% step %}
## Truy cập màn hình Products

Tại thanh menu hệ thống: chọn Order & Payment → Product & Combo → **chọn tab Products**

![](<../.gitbook/assets/image (392)>)
{% endstep %}

{% step %}
## User có thể tìm kiếm sản phẩm theo điều kiện

a. Người dùng có thể tìm kiếm theo các điều kiện dưới đây:

* Search Product: Theo tên sản phẩm
* Category: Theo chương trình học
* Status: Theo trạng thái sản phẩm
* Sort by: Chọn cách sắp xếp sản phẩm (A-Z, Z-A, Latest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

![](<../.gitbook/assets/image (393)>)

b. Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết sản phẩm đơn lẻ

{% stepper %}
{% step %}
## Chọn sản phẩm cần xem chi tiết

Tại màn hình danh sách sản phẩm, click vào giá trị tại cột **Product Name**.

![](<../.gitbook/assets/image (394)>)
{% endstep %}

{% step %}
## Hoàn tất

Hệ thống hiển thị màn hình chi tiết sản phẩm tương ứng.

![](<../.gitbook/assets/image (395)>)
{% endstep %}
{% endstepper %}

### Tạo mới sản phẩm đơn lẻ

{% stepper %}
{% step %}
## Tại màn hình Products, chọn New Product

Hệ thống chuyển tới màn hình tạo mới sản phẩm đơn lẻ.

![](<../.gitbook/assets/image (396)>)

![](<../.gitbook/assets/image (397)>)
{% endstep %}

{% step %}
## Nhập thông tin sản phẩm

![](<../.gitbook/assets/image (399)>)

Chi tiết các trường thông tin dưới đây:

| Trường thông tin      | Input                                                                                                                                                                                                                      |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Product name\*        | Nhập tên sản phẩm cần tạo mới                                                                                                                                                                                              |
| Category\*            | Chọn chương trình học của sản phẩm từ danh sách cho trước                                                                                                                                                                  |
| Subject\*             | Chọn môn học của sản phẩm từ danh sách cho trước (chỉ hiển thị tương ứng với Category)                                                                                                                                     |
| Construction mode\*   | Chọn hình thức học của sản phẩm từ danh sách cho trước                                                                                                                                                                     |
| Product - Main Course | Hệ thống cập nhật tự động dựa trên Subject và Construction mode của sản phẩm                                                                                                                                               |
| Price\*               | Nhập giá của sản phẩm theo đơn vị VND                                                                                                                                                                                      |
| Status\*              | <p>Chọn trạng thái của sản phẩm, bao gồm:<br>- Active: Sản phẩm vẫn đang được kinh doanh<br>- Inactive: Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới</p> |

{% hint style="info" %}
User cần kiểm tra lại thông tin trước khi Save, đặc biệt là **Category, Subject, Construction Mode và Price**.
{% endhint %}
{% endstep %}

{% step %}
## Lưu thông tin sản phẩm

Sau khi nhập đủ thông tin bắt buộc, chọn **Save** để lưu thông tin sản phẩm.

→ Hệ thống lưu thông tin sản phẩm mới, hiển thị ở đầu danh sách sản phẩm đơn lẻ.

![](<../.gitbook/assets/image (402)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin sản phẩm đơn lẻ

{% stepper %}
{% step %}
## Truy cập màn hình chỉnh sửa

Tại màn hình danh sách Products, user có thể truy cập màn hình chỉnh sửa sản phẩm bằng 1 trong 2 cách sau:

* Cách 1: Chọn **Product Name** của sản phẩm cần chỉnh sửa
* Cách 2: Chọn **Action > Edit** tại sản phẩm cần chỉnh sửa

→ Hệ thống chuyển đến màn hình chỉnh sửa thông tin sản phẩm.

![](<../.gitbook/assets/image (403)>)
{% endstep %}

{% step %}
## Cập nhật thông tin sản phẩm

![](<../.gitbook/assets/image (405)>)

Người dùng nhập hoặc chỉnh sửa các thông tin cần cập nhật.

| Trường thông tin      | Hướng dẫn chỉnh sửa                                                                                                                                                                                              |
| --------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Product name\*        | Cập nhật tên sản phẩm                                                                                                                                                                                            |
| Category\*            | Chọn chương trình học của sản phẩm từ danh sách cho trước                                                                                                                                                        |
| Subject\*             | Chọn môn học của sản phẩm từ danh sách cho trước                                                                                                                                                                 |
| Construction mode\*   | Chọn hình thức học của sản phẩm từ danh sách cho trước                                                                                                                                                           |
| Product - Main course | Hệ thống cập nhật tự động theo Subject và Construction Mode user đã chọn                                                                                                                                         |
| Price\*               | Cập nhật giá của sản phẩm theo đơn vị VND                                                                                                                                                                        |
| Status\*              | <p>Chọn trạng thái của sản phẩm<br>- Active: Sản phẩm vẫn đang được kinh doanh<br>- Inactive: Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới</p> |

{% hint style="info" %}
User cần kiểm tra lại thông tin trước khi Save, đặc biệt là **Category, Subject, Construction Mode và Price**.
{% endhint %}
{% endstep %}

{% step %}
## Chọn Save để lưu thông tin

Sau khi cập nhật thông tin cần chỉnh sửa, chọn **Save** để lưu thông tin.

→ Hệ thống lưu thông tin đã chỉnh sửa của sản phẩm và quay lại màn Danh sách sản phẩm.

![](<../.gitbook/assets/image (408)>)
{% endstep %}
{% endstepper %}

### Xóa sản phẩm đơn lẻ

{% stepper %}
{% step %}
## Chọn sản phẩm cần xóa, chọn Action > Delete

Hệ thống hiển thị hộp thoại xác nhận xóa sản phẩm → User có thể chọn tiếp tục xóa hoặc hủy thao tác.

![](<../.gitbook/assets/image (410)>)
{% endstep %}

{% step %}
## Xác nhận thao tác xóa trên hộp thoại

![](<../.gitbook/assets/image (414)>)

Tại hộp thoại xác nhận, user chọn **Yes** để đồng ý xóa sản phẩm.

→ Kết quả mong đợi:

* Hệ thống xóa sản phẩm khỏi danh sách;
* Sản phẩm đã xóa không còn hiển thị trên màn hình danh sách sản phẩm;
* Sản phẩm bị xóa sẽ biến mất khỏi các nhóm sản phẩm **Combo Products** hoặc mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó.
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.
{% endstep %}

{% step %}
## Kiểm tra kết quả sau khi xóa

Sau khi xác nhận xóa, user kiểm tra lại danh sách sản phẩm.

→ Kết quả mong đợi:

* Sản phẩm vừa xóa không còn xuất hiện trên danh sách sản phẩm đơn lẻ.
* Các đơn hàng đã tạo trước đó có chứa sản phẩm này vẫn được giữ nguyên thông tin.
{% endstep %}
{% endstepper %}

## III. Lưu ý & Quy tắc nghiệp vụ

### Lưu ý quan trọng

1. Khi thay đổi **Price** của sản phẩm:
   * Các đơn hàng trong tương lai sẽ áp dụng giá mới của sản phẩm.
   * Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.
2. Khi đổi trạng thái sản phẩm từ **Active** sang **Inactive**:
   * Sản phẩm sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.
   * Các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái không bị ảnh hưởng.
3. Khi xóa sản phẩm, sản phẩm sẽ bị xóa khỏi:
   * **Combo Products** có chứa sản phẩm đó
   * Mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó

### Mẹo sử dụng

1. Khi tìm kiếm, có thể kết hợp nhiều điều kiện tìm kiếm để thu hẹp kết quả nhanh hơn

## IV. Các lỗi thường gặp & Cách xử lý

| Lỗi hoặc tình huống               | Nguyên nhân                                     | Cách xử lý                                                                                    |
| --------------------------------- | ----------------------------------------------- | --------------------------------------------------------------------------------------------- |
| Không tìm thấy dữ liệu            | Sai điều kiện tìm kiếm                          | Kiểm tra lại bộ lọc tìm kiếm                                                                  |
| Không truy cập được menu Products | Chưa được cấp quyền                             | Liên hệ quản trị hệ thống                                                                     |
| This field is required            | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ các trường Product name, Category, Construction mode, Price và Status |
| Only numbers > 5000 are allowed.  | Giá sản phẩm tại trường Price nhỏ hơn 5000      | Điền lại giá sản phẩm sao cho lớn hơn 5000.                                                   |

## V. Câu hỏi thường gặp

<details>

<summary>Vì sao sản phẩm không hiển thị trong danh sách?</summary>

**Bối cảnh:** Tìm kiếm sản phẩm

Có thể sản phẩm không thỏa điều kiện tìm kiếm hoặc người dùng chưa có quyền truy cập.

</details>

<details>

<summary>Sản phẩm Inactive có sử dụng được không?</summary>

**Bối cảnh:** Xem chi tiết sản phẩm

Không. Sản phẩm Inactive không thể thêm vào nhóm sản phẩm hoặc đơn hàng mới.

</details>

<details>

<summary>Sau khi tạo mới, sản phẩm hiển thị ở đâu?</summary>

**Bối cảnh:** Tạo mới sản phẩm

Sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách sản phẩm đơn lẻ.

</details>

<details>

<summary>Có thể tạo sản phẩm ở trạng thái Inactive không?</summary>

**Bối cảnh:** Tạo mới sản phẩm

**Có**. Tuy nhiên, sản phẩm ở trạng thái Inactive là sản phẩm đã ngừng kinh doanh và sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.

</details>

<details>

<summary>Có thể chỉnh sửa giá của sản phẩm không?</summary>

**Bối cảnh:** Chỉnh sửa sản phẩm

**Có**. Khi thay đổi giá sản phẩm, các đơn hàng trong tương lai sẽ áp dụng giá mới. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.

</details>

<details>

<summary>Việc đổi trạng thái sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?</summary>

**Bối cảnh:** Chỉnh sửa sản phẩm

**Không**. Việc đổi trạng thái sản phẩm từ Active sang Inactive không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.

</details>

<details>

<summary>Sản phẩm Inactive có được thêm vào nhóm sản phẩm hoặc đơn hàng mới không?</summary>

**Bối cảnh:** Chỉnh sửa sản phẩm

**Không**. Sản phẩm ở trạng thái Inactive sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.

</details>

<details>

<summary>Các trường nào bắt buộc khi chỉnh sửa sản phẩm đơn lẻ?</summary>

**Bối cảnh:** Chỉnh sửa sản phẩm

Các trường bắt buộc gồm Product name, Category, Construction mode, Price và Status.

</details>

<details>

<summary>Sau khi xóa, sản phẩm có còn hiển thị trên danh sách Products không?</summary>

**Bối cảnh:** Xóa sản phẩm

**Không**. Sản phẩm xóa thành công sẽ biến mất khỏi màn hình danh sách sản phẩm.

</details>

<details>

<summary>Xóa sản phẩm có ảnh hưởng đến nhóm sản phẩm hoặc mã khuyến mại đã gắn sản phẩm đó không?</summary>

**Bối cảnh:** Xóa sản phẩm

**Có**. Sản phẩm đã xóa sẽ biến mất khỏi các nhóm sản phẩm Combo Products hoặc mã khuyến mại Promotion Codes đã gắn với sản phẩm trước đó.

</details>

<details>

<summary>Xóa sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?</summary>

**Bối cảnh:** Xóa sản phẩm

**Không**. Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng chứa sản phẩm đã được tạo trước đó.

</details>

<details>

<summary>Nếu không muốn tiếp tục xóa sản phẩm thì thao tác như thế nào?</summary>

**Bối cảnh:** Xóa sản phẩm

Tại hộp thoại xác nhận, chọn **No** để hủy thao tác xóa.

</details>
