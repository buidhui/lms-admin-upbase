# Xem danh sách/chi tiết mã khuyến mại

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create new         | 3.0.0   |

## Definitions and Acronyms

| # | Term            | Definition                                                               |
| - | --------------- | ------------------------------------------------------------------------ |
| 1 | Ops             | Operations                                                               |
| 2 | Promotion Codes | Mã khuyến mại dùng để giảm giá cho sản phẩm, nhóm sản phẩm hoặc đơn hàng |
| 3 | Products        | Sản phẩm đơn lẻ thuộc module Certificate Payments                        |
| 4 | Combo Products  | Nhóm sản phẩm gồm một hoặc nhiều sản phẩm đơn lẻ được kết hợp với nhau   |
| 5 | Order           | Đơn hàng được tạo cho học viên                                           |
| 6 | Code            | Mã khuyến mại                                                            |
| 7 | Quantity        | Tổng số lượng mã khuyến mại                                              |
| 8 | Discount        | Lượng giảm giá của mã khuyến mại                                         |
| 9 | Combined With   | Các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang xem           |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách xem danh sách và xem thông tin chi tiết mã khuyến mại trong tính năng **Promotion Codes** thuộc module **Payments** trên hệ thống **Operations**.

Thông qua màn hình này, người dùng có thể tra cứu mã khuyến mại đã được tạo, kiểm tra số lượng mã, thời gian hiệu lực, phạm vi áp dụng, lượng giảm giá và danh sách đơn hàng đã sử dụng mã khuyến mại.

### 1.2 Đối tượng áp dụng

| Đối tượng               | Vai trò                                                                | Quyền hạn                                            |
| ----------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------- |
| Người vận hành hệ thống | Theo dõi và quản lý mã khuyến mại phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem danh sách và xem chi tiết mã khuyến mại |

### 1.3 Phạm vi & Module liên quan

* **Tính năng chính:** Promotion Codes
* **Tính năng liên quan:** Products, Combo Products, List of Orders

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền xem mã khuyến mại.
* Hệ thống đã có dữ liệu mã khuyến mại để hiển thị trên danh sách.

***

## II. Tổng Quan Giao Diện

Màn hình danh sách mã khuyến mại **Promotion Codes** cho phép người dùng xem danh sách các mã khuyến mại đã được tạo trên hệ thống.

Các thông tin hiển thị trên danh sách gồm:

| Thông tin          | Mô tả                                                                    |
| ------------------ | ------------------------------------------------------------------------ |
| Code               | Mã khuyến mại                                                            |
| Total              | Tổng số lượng mã khuyến mại                                              |
| Used               | Số lượng mã khuyến mại đã sử dụng trong các đơn hàng đã được thanh toán  |
| Reserved           | Số lượng mã khuyến mãi được sử dụng trong các Order chưa được thanh toán |
| Start - End        | Thời gian hiệu lực của mã khuyến mại                                     |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                  |
| Apply for Combos   | Các nhóm sản phẩm được áp dụng mã khuyến mại                             |
| Status             | Trạng thái của mã khuyến mại                                             |

Giá trị của trường **Status** gồm:

| Giá trị  | Ý nghĩa                             |
| -------- | ----------------------------------- |
| Active   | Mã khuyến mại còn thời gian sử dụng |
| Inactive | Mã khuyến mại đã hết hạn sử dụng    |

Các điều kiện tìm kiếm trên màn hình gồm:

| Điều kiện tìm kiếm | Hướng dẫn sử dụng                                     |
| ------------------ | ----------------------------------------------------- |
| Code name          | Nhập tên mã khuyến mại cần tìm                        |
| Category           | Chọn một chương trình học trong danh sách cho trước   |
| Status             | Chọn một trạng thái trong danh sách cho trước         |
| Sort by            | Chọn cách sắp xếp danh sách trong danh sách cho trước |
| Start - End        | Chọn thời gian hiệu lực của mã khuyến mại             |

Các nút thao tác chính gồm:

| Nút thao tác | Ý nghĩa                                                                 |
| ------------ | ----------------------------------------------------------------------- |
| Search       | Hiển thị các mã khuyến mại theo điều kiện tìm kiếm đã nhập hoặc đã chọn |
| Reset        | Xóa tất cả giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo    |

![](<.gitbook/assets/image (837)>)

***

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Xem danh sách mã khuyến mại

> 🎯 Mục tiêu: Truy cập và xem danh sách các mã khuyến mại trên hệ thống.

{% stepper %}
{% step %}
#### Truy cập màn hình danh sách mã khuyến mại

Tại thanh Menu hệ thống **Operations**, chọn **Order & Payments > Promotion Codes**.

**Kết quả mong đợi:**

* Hệ thống chuyển đến màn hình danh sách mã khuyến mại **Promotion Codes**.
* Danh sách mã khuyến mại hiển thị các thông tin gồm **Code**, **Total**, **Used**, **Reserved**, **Start - End**, **Apply for Products**, **Apply for Combos** và **Status**.

| Thông tin          | Ý nghĩa                                                                  |
| ------------------ | ------------------------------------------------------------------------ |
| Code               | Mã khuyến mại                                                            |
| Total              | Tổng số lượng mã khuyến mại                                              |
| Used               | Số lượng mã khuyến mại đã sử dụng trong các đơn hàng đã được thanh toán  |
| Reserved           | Số lượng mã khuyến mãi được sử dụng trong các Order chưa được thanh toán |
| Start - End        | Thời gian hiệu lực của mã khuyến mại                                     |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại                                  |
| Apply for Combos   | Các nhóm sản phẩm được áp dụng mã khuyến mại                             |
| Status             | Trạng thái của mã khuyến mại                                             |

![](<.gitbook/assets/image (839)>)
{% endstep %}
{% endstepper %}

### 3.2 Tìm kiếm mã khuyến mại

> 🎯 Mục tiêu: Lọc danh sách mã khuyến mại theo điều kiện tìm kiếm.

{% stepper %}
{% step %}
#### Nhập hoặc chọn điều kiện tìm kiếm

Người dùng có thể tìm mã khuyến mại theo một hoặc nhiều điều kiện sau:

| Điều kiện tìm kiếm | Hướng dẫn                                             |
| ------------------ | ----------------------------------------------------- |
| Code name          | Nhập tên mã khuyến mại                                |
| Category           | Chọn một chương trình học trong danh sách cho trước   |
| Status             | Chọn một trạng thái trong danh sách cho trước         |
| Sort by            | Chọn cách sắp xếp danh sách trong danh sách cho trước |
| Start - End        | Chọn thời gian hiệu lực của mã khuyến mại             |

![](<.gitbook/assets/image (840)>)
{% endstep %}

{% step %}
#### Thực hiện tìm kiếm

Chọn **Search** để hiển thị các mã khuyến mại theo điều kiện tìm kiếm.

**Kết quả mong đợi:**

* Hệ thống hiển thị danh sách mã khuyến mại phù hợp với điều kiện tìm kiếm.
* Nếu không có dữ liệu phù hợp, hệ thống hiển thị kết quả theo hành vi hiện tại của hệ thống.

![](<.gitbook/assets/image (841)>)
{% endstep %}

{% step %}
#### Xóa điều kiện tìm kiếm

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm.

**Kết quả mong đợi:**

* Hệ thống xóa các điều kiện tìm kiếm đã nhập hoặc đã chọn.
* Danh sách mã khuyến mại được hiển thị theo thời gian tạo.

![](<.gitbook/assets/image (842)>)
{% endstep %}
{% endstepper %}

### 3.3 Xem chi tiết mã khuyến mại

> 🎯 Mục tiêu: Xem thông tin chi tiết của một mã khuyến mại đã có trên hệ thống.

{% stepper %}
{% step %}
#### Chọn mã khuyến mại cần xem

Tại màn hình danh sách mã khuyến mại **Promotion Codes**, chọn **Code** của mã khuyến mại cần xem.

**Kết quả mong đợi:**

* Hệ thống chuyển đến màn hình chi tiết mã khuyến mại.
* Người dùng xem được thông tin chi tiết của mã khuyến mại đã chọn.

![](<.gitbook/assets/image (843)>)
{% endstep %}

{% step %}
#### Xem thông tin chung của mã khuyến mại

Tại khu vực **Overview**, người dùng xem các thông tin sau:

| Thông tin          | Mô tả                                        |
| ------------------ | -------------------------------------------- |
| Code               | Mã khuyến mại                                |
| Quantity           | Tổng số lượng mã khuyến mại                  |
| Start - End        | Thời gian hiệu lực của mã khuyến mại         |
| Apply for Products | Các sản phẩm được áp dụng mã khuyến mại      |
| Apply for Combos   | Các nhóm sản phẩm được áp dụng mã khuyến mại |
| Discount           | Lượng giảm giá của mã khuyến mại             |
| Combined With      | Các mã giảm giá được kết hợp cùng mã này     |

Lượng giảm giá **Discount** có thể được áp dụng theo:

| Loại giảm giá                   | Ý nghĩa                                  |
| ------------------------------- | ---------------------------------------- |
| Theo phần trăm giá trị đơn hàng | Giảm giá theo tỷ lệ phần trăm            |
| Theo số tiền cụ thể             | Giảm giá theo số tiền cụ thể, đơn vị VND |

**Combined With** cho phép người dùng sử dụng nhiều mã khuyến mại cho cùng một sản phẩm hoặc nhóm sản phẩm trong đơn hàng.

**Kết quả mong đợi:**

* Người dùng xem được thông tin cấu hình chung của mã khuyến mại.
* Người dùng kiểm tra được phạm vi áp dụng, thời gian hiệu lực, lượng giảm giá và khả năng kết hợp với mã khác.

![](<.gitbook/assets/image (844)>)
{% endstep %}

{% step %}
#### Xem danh sách đơn hàng sử dụng mã khuyến mại

Tại khu vực **List Orders**, người dùng xem danh sách các đơn hàng đã sử dụng mã khuyến mại.

Các thông tin hiển thị gồm:

| Thông tin | Mô tả                                          |
| --------- | ---------------------------------------------- |
| Product   | Tên sản phẩm sử dụng mã khuyến mại             |
| Combo     | Tên nhóm sản phẩm sử dụng mã khuyến mại        |
| Customer  | Khách hàng                                     |
| Deal ID   | Mã Deal trên Hubspot của khách hàng            |
| Price     | Giá trị sản phẩm sau khi áp dụng mã khuyến mại |
| Status    | Trạng thái của đơn hàng                        |

Trạng thái đơn hàng có thể gồm:

| Trạng thái      | Ý nghĩa                                  |
| --------------- | ---------------------------------------- |
| Chờ thanh toán  | Đơn hàng đang chờ học viên thanh toán    |
| Đang thanh toán | Đơn hàng đang trong quá trình thanh toán |
| Đã thanh toán   | Đơn hàng đã được thanh toán              |
| Hết hạn         | Đơn hàng đã hết hạn thanh toán           |
| Đã hủy          | Đơn hàng đã bị hủy                       |

**Kết quả mong đợi:**

* Người dùng xem được danh sách đơn hàng đã sử dụng mã khuyến mại.
* Người dùng kiểm tra được sản phẩm, nhóm sản phẩm, khách hàng, Deal ID, giá trị sau khuyến mại và trạng thái của từng đơn hàng.

![](<.gitbook/assets/image (845)>)
{% endstep %}
{% endstepper %}

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

* Mã khuyến mại có trạng thái **Active** là mã còn thời gian sử dụng.
* Mã khuyến mại có trạng thái **Inactive** là mã đã hết hạn sử dụng.
* **Combined With** cho phép dùng nhiều mã khuyến mại cho cùng một sản phẩm hoặc nhóm sản phẩm trong đơn hàng.
* Khu vực **List Orders** hiển thị các đơn hàng đã sử dụng mã khuyến mại.

***

## V. Các lỗi thường gặp và cách xử lý

Updating...

***

## VI. Câu Hỏi Thường Gặp

<details>

<summary>Q: Combined With dùng để làm gì?</summary>

**A:** **Combined With** cho phép người dùng sử dụng nhiều mã khuyến mại cho cùng một sản phẩm hoặc nhóm sản phẩm trong đơn hàng.

</details>

<details>

<summary>Q: List Orders hiển thị thông tin gì?</summary>

**A:** **List Orders** hiển thị danh sách đơn hàng đã sử dụng mã khuyến mại, gồm sản phẩm, nhóm sản phẩm, khách hàng, Deal ID, giá trị sau khuyến mại và trạng thái đơn hàng.

</details>
