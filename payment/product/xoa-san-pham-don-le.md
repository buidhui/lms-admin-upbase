---
hidden: true
---

# Xóa sản phẩm đơn lẻ

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

Tài liệu này hướng dẫn người dùng cách xóa sản phẩm đơn lẻ trong tính năng **Products** thuộc module **Payments** trên hệ thống **Operations**.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                               | Quyền hạn                           |
| ----------------------- | --------------------------------------------------------------------- | ----------------------------------- |
| Người vận hành hệ thống | Quản lý danh mục sản phẩm đơn lẻ phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và xóa sản phẩm đơn lẻ |

### **1.3 Phạm vi và Module liên quan**

* **Tính năng chính:** Products
* **Tính năng liên quan:** Combo Products, Promotion Codes, Order List

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền xóa sản phẩm đơn lẻ.
* Sản phẩm cần xóa đã tồn tại trên danh sách sản phẩm đơn lẻ **Products**.
* Người dùng đã xác định đúng sản phẩm cần xóa trước khi thực hiện thao tác.

***

## II. Tổng Quan Giao Diện

Màn hình danh sách sản phẩm đơn lẻ **Products** cho phép người dùng thực hiện thao tác xóa sản phẩm thông qua nút **Action > Delete** tại từng dòng sản phẩm.

Các thành phần chính liên quan đến thao tác xóa gồm:

* **Product Name:** Tên sản phẩm cần xóa.
* **Action:** Khu vực thao tác với sản phẩm.
* **Delete:** Chức năng xóa sản phẩm.
* **Yes:** Xác nhận đồng ý xóa sản phẩm.
* **No:** Hủy thao tác xóa sản phẩm.

<figure><img src="../../.gitbook/assets/image (296).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

**Mục tiêu:** Xóa một sản phẩm đơn lẻ ra khỏi danh sách sản phẩm trên hệ thống.

**Bước 1:** Chọn sản phẩm cần xóa

Tại màn hình danh sách sản phẩm đơn lẻ **Products (Operations → Order & Payment → Products & Combo → Products)**, tìm sản phẩm cần xóa.

Tại dòng sản phẩm cần xóa, chọn **Action > Delete**.

Kết quả mong đợi:

* Hệ thống hiển thị hộp thoại xác nhận xóa sản phẩm.
* Người dùng có thể chọn tiếp tục xóa hoặc hủy thao tác.

<figure><img src="../../.gitbook/assets/image (297).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Xác nhận thao tác xóa

Tại hộp thoại xác nhận:

| Nút thao tác | Ý nghĩa                   |
| ------------ | ------------------------- |
| Yes          | Đồng ý xóa sản phẩm       |
| No           | Hủy thao tác xóa sản phẩm |

Người dùng chọn **Yes** để đồng ý xóa sản phẩm.

Kết quả mong đợi:

* Hệ thống xóa sản phẩm khỏi danh sách sản phẩm đơn lẻ.
* Sản phẩm đã xóa không còn hiển thị trên màn hình danh sách sản phẩm.
* Sản phẩm bị xóa sẽ biến mất khỏi các nhóm sản phẩm **Combo Products** hoặc mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó.
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.

<figure><img src="../../.gitbook/assets/image (298).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Kiểm tra kết quả sau khi xóa

Sau khi xác nhận xóa, người dùng kiểm tra lại danh sách sản phẩm.

Kết quả mong đợi:

* Sản phẩm vừa xóa không còn xuất hiện trên danh sách sản phẩm đơn lẻ.
* Các đơn hàng đã tạo trước đó có chứa sản phẩm này vẫn được giữ nguyên thông tin.

***

## IV. Lưu Ý và Quy Tắc Nghiệp Vụ

**Lưu ý quan trọng**

* Người dùng cần kiểm tra kỹ sản phẩm trước khi chọn **Yes** để xác nhận xóa.
* Sau khi xóa thành công, sản phẩm sẽ biến mất khỏi màn hình danh sách sản phẩm.
* Sản phẩm đã xóa sẽ biến mất khỏi các nhóm sản phẩm **Combo Products** hoặc mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó.
* Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa sản phẩm này.

***

## V. Các lỗi thường gặp và cách xử lý

Chưa có

***

## VI. Câu Hỏi Thường Gặp

**Q: Sau khi xóa, sản phẩm có còn hiển thị trên danh sách Products không?**\
A: Không. Sản phẩm xóa thành công sẽ biến mất khỏi màn hình danh sách sản phẩm.

**Q: Xóa sản phẩm có ảnh hưởng đến nhóm sản phẩm hoặc mã khuyến mại đã gắn sản phẩm đó không?**\
A: Có. Sản phẩm đã xóa sẽ biến mất khỏi các nhóm sản phẩm **Combo Products** hoặc mã khuyến mại **Promotion Codes** đã gắn với sản phẩm trước đó.

**Q: Xóa sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?**\
A: Không. Việc xóa sản phẩm không ảnh hưởng đến các đơn hàng chứa sản phẩm đã được tạo trước đó.

**Q: Nếu không muốn tiếp tục xóa sản phẩm thì thao tác như thế nào?**\
A: Tại hộp thoại xác nhận, chọn **No** để hủy thao tác xóa.
