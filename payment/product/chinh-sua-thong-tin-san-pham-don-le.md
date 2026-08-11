---
hidden: true
---

# Chỉnh sửa thông tin sản phẩm đơn lẻ

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create New         | 3.0.0   |

***

## Definitions and Acronyms

| # | Term     | Definition       |
| - | -------- | ---------------- |
| 1 | Ops      | Operations       |
| 2 | Product  | Sản phẩm đơn lẻ  |
| 3 | Category | Chương trình học |

## I. Giới Thiệu Chung

### **1.1 Mục đích**

Tài liệu này hướng dẫn người dùng cách chỉnh sửa thông tin sản phẩm đơn lẻ trong tính năng **Products** thuộc module **Payments** trên hệ thống **Operations**.

Sau khi thực hiện xong, thông tin sản phẩm sẽ được cập nhật trên hệ thống. Các thay đổi có thể ảnh hưởng đến việc sử dụng sản phẩm trong các nghiệp vụ liên quan như tạo nhóm sản phẩm hoặc tạo đơn hàng mới.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                                            | Quyền hạn                                 |
| ----------------------- | ---------------------------------------------------------------------------------- | ----------------------------------------- |
| Người vận hành hệ thống | Quản lý và cập nhật thông tin sản phẩm đơn lẻ phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và chỉnh sửa sản phẩm đơn lẻ |

### **1.3 Phạm vi và Module liên quan**

* **Tính năng chính:** Products
* **Tính năng liên quan:** Combo Products, Promotion Codes, Order List

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền chỉnh sửa sản phẩm đơn lẻ.
* Sản phẩm cần chỉnh sửa đã tồn tại trên danh sách sản phẩm đơn lẻ **Products**.
* Các danh mục dùng để chọn tại trường **Category** và **Construction mode** đã có dữ liệu trong hệ thống.

***

## II. Tổng Quan Giao Diện

Màn hình chỉnh sửa thông tin sản phẩm đơn lẻ cho phép người dùng xem và cập nhật các thông tin của sản phẩm đã tạo trước đó.

Các thành phần chính trên màn hình gồm:

* **Product name:** Tên sản phẩm.
* **Category:** Chương trình học của sản phẩm.
* **Construction mode:** Hình thức học của sản phẩm.
* **Price:** Giá của sản phẩm, theo đơn vị VND.
* **Status:** Trạng thái của sản phẩm.
* **Save:** Nút lưu thông tin sau khi chỉnh sửa.

<figure><img src="../../.gitbook/assets/image (292).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

**Mục tiêu:** Cập nhật thông tin của một sản phẩm đơn lẻ đã tồn tại trên hệ thống.

**Bước 1:** Truy cập màn hình chỉnh sửa sản phẩm

Tại màn hình danh sách sản phẩm đơn lẻ **Products (Operations → Order & Payment → Products & Combo → Products)**, người dùng có thể truy cập màn hình chỉnh sửa sản phẩm bằng một trong hai cách sau:

| Cách thực hiện | Thao tác                                          |
| -------------- | ------------------------------------------------- |
| Cách 1         | Chọn **Product Name** của sản phẩm cần chỉnh sửa  |
| Cách 2         | Chọn **Action > Edit** tại sản phẩm cần chỉnh sửa |

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình chỉnh sửa thông tin sản phẩm.
* Màn hình hiển thị thông tin hiện tại của sản phẩm đã chọn.

<figure><img src="../../.gitbook/assets/image (293).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Cập nhật thông tin sản phẩm

Người dùng nhập hoặc chỉnh sửa các thông tin cần thay đổi.

| Trường thông tin  | Bắt buộc | Hướng dẫn chỉnh sửa                                       |
| ----------------- | -------- | --------------------------------------------------------- |
| Product name      | Có       | Cập nhật tên sản phẩm                                     |
| Category          | Có       | Chọn chương trình học của sản phẩm từ danh sách cho trước |
| Construction mode | Có       | Chọn hình thức học của sản phẩm từ danh sách cho trước    |
| Price             | Có       | Cập nhật giá của sản phẩm theo đơn vị VND                 |
| Status            | Có       | Chọn trạng thái của sản phẩm                              |

Giá trị của trường **Status** gồm:

| Giá trị  | Ý nghĩa                                                                                                        |
| -------- | -------------------------------------------------------------------------------------------------------------- |
| Active   | Sản phẩm vẫn đang được kinh doanh                                                                              |
| Inactive | Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới |

Lưu ý:

* Các trường được đánh dấu bắt buộc không được để trống.
* Người dùng cần kiểm tra lại thông tin trước khi lưu, đặc biệt là **Product name**, **Category**, **Construction mode**, **Price** và **Status**.

<figure><img src="../../.gitbook/assets/image (294).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Lưu thông tin chỉnh sửa

Sau khi cập nhật đầy đủ thông tin cần thay đổi, chọn **Save** để lưu thông tin.

Kết quả mong đợi:

* Hệ thống lưu thông tin đã chỉnh sửa của sản phẩm và quay lại màn Danh sách sản phẩm.
* Thông tin mới của sản phẩm được cập nhật trên hệ thống.

<figure><img src="../../.gitbook/assets/image (295).png" alt=""><figcaption></figcaption></figure>

***

## IV. Lưu Ý và Quy Tắc Nghiệp Vụ

**Lưu ý quan trọng**

* Các trường bắt buộc không được để trống.
* Trường **Price** sử dụng đơn vị VND, cần điền giá trị khác lớn hơn 5000.
* Khi thay đổi **Price** của sản phẩm:
  * Các đơn hàng trong tương lai sẽ áp dụng giá mới của sản phẩm.
  * Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.
* Khi đổi trạng thái sản phẩm từ **Active** sang **Inactive**:
  * Sản phẩm sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.
  * Các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái không bị ảnh hưởng.

***

## V. Các lỗi thường gặp và cách xử lý

Hiện tài liệu gốc chưa cung cấp thông báo lỗi cụ thể của hệ thống. Có thể bổ sung sau khi có ảnh màn hình hoặc nội dung message thực tế.

| Lỗi hoặc tình huống              | Nguyên nhân                                     | Cách xử lý                                                                                    |
| -------------------------------- | ----------------------------------------------- | --------------------------------------------------------------------------------------------- |
| This field is required           | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ các trường Product name, Category, Construction mode, Price và Status |
| Only numbers > 5000 are allowed. | Giá sản phẩm tại trường Price nhỏ hơn 5000      | Điền lại giá sản phẩm sao cho lớn hơn 5000.                                                   |

***

## VI. Câu Hỏi Thường Gặp

**Q: Có thể chỉnh sửa giá của sản phẩm không?**\
A: Có. Khi thay đổi giá sản phẩm, các đơn hàng trong tương lai sẽ áp dụng giá mới. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.

**Q: Việc đổi trạng thái sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?**\
A: Không. Việc đổi trạng thái sản phẩm từ Active sang Inactive không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.

**Q: Sản phẩm Inactive có được thêm vào nhóm sản phẩm hoặc đơn hàng mới không?**\
A: Không. Sản phẩm ở trạng thái Inactive sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.

**Q: Các trường nào bắt buộc khi chỉnh sửa sản phẩm đơn lẻ?**\
A: Các trường bắt buộc gồm Product name, Category, Construction mode, Price và Status.
