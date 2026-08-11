---
hidden: true
---

# Tạo mới sản phẩm đơn lẻ

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

Tài liệu này hướng dẫn người dùng cách tạo mới sản phẩm đơn lẻ trong tính năng **Products** thuộc module **Payments** trên hệ thống **Operations**.

Sau khi thực hiện xong, sản phẩm đơn lẻ mới sẽ được lưu vào hệ thống và hiển thị trên danh sách sản phẩm để phục vụ cho việc tạo nhóm sản phẩm hoặc tạo đơn hàng.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                                      | Quyền hạn                               |
| ----------------------- | ---------------------------------------------------------------------------- | --------------------------------------- |
| Người vận hành hệ thống | Tạo và quản lý danh mục sản phẩm đơn lẻ phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và tạo mới sản phẩm đơn lẻ |

### **1.3 Phạm vi và Module liên quan**

* **Tính năng chính:** Products
* **Tính năng liên quan:** Combo Products, List of Orders

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền tạo mới sản phẩm đơn lẻ.
* Người dùng đang ở màn hình danh sách sản phẩm đơn lẻ **Products**.

***

## II. Tổng Quan Giao Diện

Màn hình tạo mới sản phẩm đơn lẻ cho phép người dùng nhập các thông tin cần thiết để tạo một sản phẩm mới.

Các thành phần chính trên màn hình gồm:

* **Product name:** Tên sản phẩm.
* **Category:** Chương trình học của sản phẩm.
* **Construction mode:** Hình thức học của sản phẩm.
* **Price:** Giá của sản phẩm, theo đơn vị VND.
* **Status:** Trạng thái của sản phẩm.
* **Save:** Nút lưu thông tin sản phẩm.

<figure><img src="../../.gitbook/assets/image (288).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

**Mục tiêu:** Tạo mới một sản phẩm đơn lẻ trên hệ thống để phục vụ cho việc quản lý sản phẩm, tạo nhóm sản phẩm hoặc tạo đơn hàng.

**Bước 1:** Truy cập màn hình tạo mới sản phẩm

Tại màn hình danh sách sản phẩm đơn lẻ **Products (Operations → Order & Payment → Products & Combo → Products)**, chọn **New Product**.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình tạo mới sản phẩm đơn lẻ.
* Người dùng có thể bắt đầu nhập thông tin sản phẩm.

<figure><img src="../../.gitbook/assets/image (289).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Nhập thông tin sản phẩm

Người dùng nhập các thông tin sau:

| Trường thông tin  | Bắt buộc | Hướng dẫn nhập                                            |
| ----------------- | -------- | --------------------------------------------------------- |
| Product name      | Có       | Nhập tên sản phẩm cần tạo mới                             |
| Category          | Có       | Chọn chương trình học của sản phẩm từ danh sách cho trước |
| Construction mode | Có       | Chọn hình thức học của sản phẩm từ danh sách cho trước    |
| Price             | Có       | Nhập giá của sản phẩm theo đơn vị VND                     |
| Status            | Có       | Chọn trạng thái của sản phẩm                              |

Giá trị của trường **Status** gồm:

| Giá trị  | Ý nghĩa                                                                                                        |
| -------- | -------------------------------------------------------------------------------------------------------------- |
| Active   | Sản phẩm vẫn đang được kinh doanh                                                                              |
| Inactive | Sản phẩm đã ngừng kinh doanh. Sản phẩm ở trạng thái này sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới |

Lưu ý:

* Các trường được đánh dấu bắt buộc không được để trống.
* Người dùng cần kiểm tra lại thông tin trước khi lưu, đặc biệt là **Product name**, **Category**, **Construction mode** và **Price**.

<figure><img src="../../.gitbook/assets/image (290).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Lưu thông tin sản phẩm

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin sản phẩm.

Kết quả mong đợi:

* Hệ thống lưu thông tin sản phẩm mới.
* Sản phẩm vừa tạo hiển thị ở đầu danh sách sản phẩm đơn lẻ.

<figure><img src="../../.gitbook/assets/image (291).png" alt=""><figcaption></figcaption></figure>

***

## IV. Lưu Ý và Quy Tắc Nghiệp Vụ

**Lưu ý quan trọng**

* Các trường bắt buộc không được để trống.
* Trường **Price** sử dụng đơn vị VND, cần điền số khác 0.
* Sản phẩm có trạng thái **Active** có thể được sử dụng trong các nghiệp vụ liên quan như Combo, Order,...
* Sản phẩm có trạng thái **Inactive** không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.
* Sản phẩm vừa tạo thành công sẽ hiển thị ở đầu danh sách sản phẩm.

***

## V. Các lỗi thường gặp và cách xử lý

Hiện tài liệu gốc chưa cung cấp thông báo lỗi cụ thể của hệ thống. Có thể bổ sung sau khi có ảnh màn hình hoặc nội dung message thực tế.

| Lỗi hoặc tình huống    | Nguyên nhân                                     | Cách xử lý                                                                                    |
| ---------------------- | ----------------------------------------------- | --------------------------------------------------------------------------------------------- |
| This field is required | Người dùng chưa nhập đầy đủ các trường bắt buộc | Kiểm tra và nhập đầy đủ các trường Product name, Category, Construction mode, Price và Status |

***

## VI. Câu Hỏi Thường Gặp

**Q: Sau khi tạo mới, sản phẩm hiển thị ở đâu?**\
A: Sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách sản phẩm đơn lẻ.

**Q: Có thể tạo sản phẩm ở trạng thái Inactive không?**\
A: Có. Tuy nhiên, sản phẩm ở trạng thái Inactive là sản phẩm đã ngừng kinh doanh và sẽ không được thêm vào nhóm sản phẩm hoặc đơn hàng mới.
