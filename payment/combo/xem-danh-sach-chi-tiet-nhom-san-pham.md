---
hidden: true
---

# Xem danh sách/chi tiết nhóm sản phẩm

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create New         | 3.0.0   |

***

## Definitions and Acronyms

| # | Term          | Definition       |
| - | ------------- | ---------------- |
| 1 | Ops           | Operations       |
| 2 | Product       | Sản phẩm đơn lẻ  |
| 3 | Category      | Chương trình học |
| 4 | Combo Product | Nhóm sản phẩm    |

## I. Giới Thiệu Chung

### **1.1 Mục đích**

Tài liệu này hướng dẫn người dùng cách xem danh sách và xem thông tin chi tiết nhóm sản phẩm trong tính năng **Combo Products** thuộc module **Payments** trên hệ thống **Operations**.

Thông qua màn hình này, người dùng có thể tra cứu các nhóm sản phẩm đã được tạo, kiểm tra danh sách sản phẩm trong từng nhóm, chương trình học, giá và trạng thái của nhóm sản phẩm.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                                | Quyền hạn                                            |
| ----------------------- | ---------------------------------------------------------------------- | ---------------------------------------------------- |
| Người vận hành hệ thống | Theo dõi và quản lý nhóm sản phẩm phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem danh sách và xem chi tiết nhóm sản phẩm |

### **1.3 Phạm vi và Module liên quan**

* **Tính năng chính:** Combo Products
* **Tính năng liên quan:** Products, Promotion Codes, List of Orders

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền xem nhóm sản phẩm.
* Hệ thống đã có dữ liệu nhóm sản phẩm để hiển thị trên danh sách.

***

## II. Tổng Quan Giao Diện

Màn hình danh sách nhóm sản phẩm **Combo Products** cho phép người dùng xem danh sách các nhóm sản phẩm đã được tạo trên hệ thống.

Các thông tin hiển thị trên danh sách gồm:

| Thông tin  | Mô tả                                                                                                                                                                                                         |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Combo name | Tên nhóm sản phẩm                                                                                                                                                                                             |
| Products   | Danh sách sản phẩm trong nhóm                                                                                                                                                                                 |
| Category   | Chương trình học của nhóm sản phẩm. Hệ thống tổng hợp từ chương trình học của từng sản phẩm trong nhóm                                                                                                        |
| Price      | Giá của nhóm sản phẩm. Giá trị này là tổng giá trị của các sản phẩm trong nhóm                                                                                                                                |
| Status     | <p>Trạng thái của nhóm sản phẩm:<br>- Active: Nhóm sản phẩm vẫn đang được kinh doanh<br>- Inactive: Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới</p> |

Các điều kiện tìm kiếm trên màn hình gồm:

| Điều kiện tìm kiếm | Hướng dẫn sử dụng                                     |
| ------------------ | ----------------------------------------------------- |
| Search Combo       | Nhập tên nhóm sản phẩm cần tìm                        |
| Product            | Chọn một sản phẩm trong danh sách cho trước           |
| Category           | Chọn một chương trình học trong danh sách cho trước   |
| Status             | Chọn một trạng thái trong danh sách cho trước         |
| Sort by            | Chọn cách sắp xếp danh sách trong danh sách cho trước |

<figure><img src="../../.gitbook/assets/image (299).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

### **3.1 Xem danh sách nhóm sản phẩm**

**Mục tiêu:** Truy cập và xem danh sách các nhóm sản phẩm trên hệ thống.

**Bước 1:** Truy cập màn hình danh sách nhóm sản phẩm

Tại thanh Menu hệ thống **Operations**, chọn **Order & Payment > Product & Combo** **> Combo Products**.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình danh sách nhóm sản phẩm **Combo Products**.
* Các nhóm sản phẩm hiển thị theo thời gian tạo từ gần đến xa.
* Danh sách nhóm sản phẩm hiển thị các thông tin gồm **Combo name**, **Products**, **Category**, **Price** và **Status**.

| Thông tin  | Ý nghĩa                                  |
| ---------- | ---------------------------------------- |
| Combo name | Tên nhóm sản phẩm                        |
| Products   | Danh sách sản phẩm thuộc nhóm sản phẩm   |
| Category   | Chương trình học của nhóm sản phẩm       |
| Price      | Tổng giá trị của các sản phẩm trong nhóm |
| Status     | Trạng thái của nhóm sản phẩm             |

<figure><img src="../../.gitbook/assets/image (300).png" alt=""><figcaption></figcaption></figure>

### **3.2 Tìm kiếm nhóm sản phẩm**

**Mục tiêu:** Lọc danh sách nhóm sản phẩm theo điều kiện tìm kiếm.

**Bước 1:** Nhập hoặc chọn điều kiện tìm kiếm

Người dùng có thể tìm nhóm sản phẩm theo một hoặc nhiều điều kiện sau:

| Điều kiện tìm kiếm | Hướng dẫn                                             |
| ------------------ | ----------------------------------------------------- |
| Search Combo       | Nhập tên nhóm sản phẩm                                |
| Product            | Chọn một sản phẩm trong danh sách cho trước           |
| Category           | Chọn một chương trình học trong danh sách cho trước   |
| Status             | Chọn một trạng thái trong danh sách cho trước         |
| Sort by            | Chọn cách sắp xếp danh sách trong danh sách cho trước |

**Bước 2:** Thực hiện tìm kiếm

Chọn **Search** để hiển thị các nhóm sản phẩm theo điều kiện tìm kiếm.

Kết quả mong đợi:

* Hệ thống hiển thị danh sách nhóm sản phẩm phù hợp với điều kiện tìm kiếm.
* Nếu không có dữ liệu phù hợp, hệ thống hiển thị kết quả theo hành vi hiện tại của hệ thống.

<figure><img src="../../.gitbook/assets/image (301).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Xóa điều kiện tìm kiếm

Chọn **Reset** để xóa tất cả các giá trị tìm kiếm.

Kết quả mong đợi:

* Hệ thống xóa các điều kiện tìm kiếm đã nhập hoặc đã chọn.
* Danh sách nhóm sản phẩm được hiển thị theo thời gian tạo.

<figure><img src="../../.gitbook/assets/image (302).png" alt=""><figcaption></figcaption></figure>

### **3.3 Xem chi tiết nhóm sản phẩm**

**Mục tiêu:** Xem thông tin chi tiết của một nhóm sản phẩm đã có trên hệ thống.

**Bước 1:** Chọn nhóm sản phẩm cần xem

Tại màn hình danh sách nhóm sản phẩm **Combo Products**, chọn **Combo Name** của nhóm sản phẩm cần xem.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình chi tiết nhóm sản phẩm.
* Người dùng xem được thông tin chi tiết của nhóm sản phẩm đã chọn.

<figure><img src="../../.gitbook/assets/image (303).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Xem thông tin chi tiết nhóm sản phẩm

Màn hình chi tiết nhóm sản phẩm hiển thị các thông tin sau:

| Thông tin  | Mô tả                                                                                                  |
| ---------- | ------------------------------------------------------------------------------------------------------ |
| Combo name | Tên nhóm sản phẩm                                                                                      |
| Products   | Danh sách sản phẩm trong nhóm                                                                          |
| Category   | Chương trình học của nhóm sản phẩm. Hệ thống tổng hợp từ chương trình học của từng sản phẩm trong nhóm |
| Price      | Giá của nhóm sản phẩm. Giá trị này là tổng giá trị của các sản phẩm trong nhóm                         |
| Status     | Trạng thái của nhóm sản phẩm                                                                           |

Kết quả mong đợi:

* Người dùng xem được đầy đủ thông tin chi tiết của nhóm sản phẩm.
* Người dùng kiểm tra được danh sách sản phẩm trong nhóm, chương trình học, giá và trạng thái của nhóm sản phẩm.

<figure><img src="../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>

***

## IV. Lưu Ý và Quy Tắc Nghiệp Vụ

**Lưu ý quan trọng**

* **Category** của nhóm sản phẩm được hệ thống tổng hợp từ chương trình học của từng sản phẩm trong nhóm.
* **Price** của nhóm sản phẩm là tổng giá trị của các sản phẩm trong nhóm.
* Nhóm sản phẩm có trạng thái **Active** là nhóm sản phẩm vẫn đang được kinh doanh.
* Nhóm sản phẩm có trạng thái **Inactive** là nhóm sản phẩm đã ngừng kinh doanh và không được thêm vào đơn hàng mới.

***

## V. Các lỗi thường gặp và cách xử lý

Updating...

***

#### VI. Câu Hỏi Thường Gặp

**Q: Price của nhóm sản phẩm được hiểu như thế nào?**\
A: **Price** là tổng giá trị của các sản phẩm trong nhóm.

**Q: Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?**\
A: Không. Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.
