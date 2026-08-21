---
hidden: true
---

# Chỉnh sửa thông tin nhóm sản phẩm

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create new         | 3.0.0   |

## Definitions and Acronyms

| # | Term           | Definition                                                             |
| - | -------------- | ---------------------------------------------------------------------- |
| 1 | Ops            | Operations                                                             |
| 2 | Combo Products | Nhóm sản phẩm gồm một hoặc nhiều sản phẩm đơn lẻ được kết hợp với nhau |
| 3 | Products       | Sản phẩm đơn lẻ thuộc module Certificate Payments                      |
| 4 | Category       | Chương trình học của sản phẩm hoặc nhóm sản phẩm                       |
| 5 | Price          | Giá của sản phẩm hoặc nhóm sản phẩm                                    |
| 6 | Status         | Trạng thái hoạt động của sản phẩm hoặc nhóm sản phẩm                   |
| 7 | Order          | Đơn hàng được tạo cho học viên                                         |

## I. Giới Thiệu Chung

### **1.1 Mục đích**

Tài liệu này hướng dẫn người dùng cách chỉnh sửa thông tin nhóm sản phẩm trong tính năng **Combo Products** thuộc module**Payments** trên hệ thống **Operations**.

Sau khi thực hiện xong, thông tin nhóm sản phẩm sẽ được cập nhật trên hệ thống. Các thay đổi về sản phẩm trong nhóm, giá hoặc trạng thái có thể ảnh hưởng đến việc sử dụng nhóm sản phẩm trong các đơn hàng được tạo sau thời điểm chỉnh sửa.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                                | Quyền hạn                               |
| ----------------------- | ---------------------------------------------------------------------- | --------------------------------------- |
| Người vận hành hệ thống | Quản lý và cập nhật nhóm sản phẩm phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và chỉnh sửa nhóm sản phẩm |

### **1.3 Phạm vi & Module liên quan**

* **Tính năng chính:** Combo Products
* **Module liên quan:** Products, Promotion Code, Order List

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền chỉnh sửa nhóm sản phẩm.
* Nhóm sản phẩm cần chỉnh sửa đã tồn tại trên danh sách nhóm sản phẩm **Combo Products**.
* Các sản phẩm đơn lẻ cần thêm vào nhóm sản phẩm đã được tạo trên hệ thống.

***

## II. Tổng Quan Giao Diện

Màn hình chỉnh sửa thông tin nhóm sản phẩm cho phép người dùng xem và cập nhật các thông tin của nhóm sản phẩm đã tạo trước đó.

Các thành phần chính trên màn hình gồm:

| Thành phần | Mô tả                                                                                                     |
| ---------- | --------------------------------------------------------------------------------------------------------- |
| Combo name | Tên nhóm sản phẩm                                                                                         |
| Products   | Danh sách sản phẩm trong nhóm                                                                             |
| Category   | Chương trình học của nhóm sản phẩm. Hệ thống tự tổng hợp từ chương trình học của từng sản phẩm trong nhóm |
| Price      | Giá của nhóm sản phẩm. Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm                     |
| Status     | Trạng thái của nhóm sản phẩm                                                                              |
| Save       | Nút lưu thông tin nhóm sản phẩm sau khi chỉnh sửa                                                         |

Giá trị của trường **Status** gồm:

| Giá trị  | Ý nghĩa                                                                                               |
| -------- | ----------------------------------------------------------------------------------------------------- |
| Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |

<figure><img src="../../.gitbook/assets/image (325).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

### **3.1 Chỉnh sửa thông tin nhóm sản phẩm**

> 🎯 Mục tiêu: Cập nhật thông tin của một nhóm sản phẩm đã tồn tại trên hệ thống.

**Bước 1:** Truy cập màn hình chỉnh sửa nhóm sản phẩm

Tại màn hình danh sách nhóm sản phẩm **Combo Products**, người dùng có thể truy cập màn hình chỉnh sửa nhóm sản phẩm bằng một trong hai cách sau:

| Cách thực hiện | Thao tác                                               |
| -------------- | ------------------------------------------------------ |
| Cách 1         | Chọn **Combo Name** của nhóm sản phẩm cần chỉnh sửa    |
| Cách 2         | Chọn **Action > Edit** tại nhóm sản phẩm cần chỉnh sửa |

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình chỉnh sửa thông tin nhóm sản phẩm.
* Màn hình hiển thị thông tin hiện tại của nhóm sản phẩm đã chọn.

<figure><img src="../../.gitbook/assets/image (326).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Cập nhật tên nhóm sản phẩm

Tại trường **Combo name**, cập nhật tên nhóm sản phẩm nếu cần.

| Trường thông tin | Bắt buộc | Hướng dẫn chỉnh sửa        |
| ---------------- | -------- | -------------------------- |
| Combo name       | Có       | Cập nhật tên nhóm sản phẩm |

Kết quả mong đợi: Tên nhóm sản phẩm mới được ghi nhận trên form chỉnh sửa.

**Bước 3:** Cập nhật danh sách sản phẩm trong nhóm

Người dùng có thể cập nhật danh sách sản phẩm trong nhóm theo một trong các cách sau:

| Nhu cầu                                | Thao tác                                                                                                                                                              |
| -------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Xóa sản phẩm khỏi nhóm                 | Chọn dấu **x** tại sản phẩm cần xóa                                                                                                                                   |
| Thêm hoặc chọn lại sản phẩm trong nhóm | Chọn vào vùng trống của trường **Products** để mở màn hình danh sách sản phẩm. Sau đó chọn hoặc bỏ chọn checkbox tại các sản phẩm cần thay đổi và chọn **Add** để lưu |

Kết quả mong đợi:

* Danh sách sản phẩm trong nhóm được cập nhật theo lựa chọn của người dùng.
* Hệ thống sử dụng danh sách sản phẩm đã cập nhật để tự tổng hợp **Category** và tự tính **Price**.

<figure><img src="../../.gitbook/assets/image (327).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (329).png" alt=""><figcaption></figcaption></figure>

**Bước 4:** Kiểm tra thông tin Category và Price

Sau khi cập nhật danh sách sản phẩm trong nhóm, người dùng kiểm tra các thông tin hệ thống tự hiển thị.

| Trường thông tin | Cách xử lý                                                                                                      |
| ---------------- | --------------------------------------------------------------------------------------------------------------- |
| Category         | Hệ thống tự tổng hợp các chương trình học của từng sản phẩm trong nhóm. Người dùng không cần điền thông tin này |
| Price            | Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm. Người dùng không cần điền thông tin này         |

Kết quả mong đợi:

* **Category** hiển thị theo thông tin của các sản phẩm hiện có trong nhóm.
* **Price** hiển thị theo tổng giá trị của các sản phẩm hiện có trong nhóm.

**Bước 5:** Cập nhật trạng thái nhóm sản phẩm

Tại trường **Status**, chọn trạng thái của nhóm sản phẩm.

| Trường thông tin | Bắt buộc | Giá trị  | Ý nghĩa                                                                                               |
| ---------------- | -------- | -------- | ----------------------------------------------------------------------------------------------------- |
| Status           | Có       | Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Status           | Có       | Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |

Kết quả mong đợi: Trạng thái nhóm sản phẩm được ghi nhận trên form chỉnh sửa.

**Bước 6:** Lưu thông tin chỉnh sửa

Sau khi cập nhật đầy đủ thông tin cần thay đổi, chọn **Save** để lưu thông tin.

Kết quả mong đợi:

* Hệ thống lưu thông tin đã chỉnh sửa của nhóm sản phẩm.
* Thông tin mới của nhóm sản phẩm được cập nhật trên hệ thống.

<figure><img src="../../.gitbook/assets/image (330).png" alt=""><figcaption></figcaption></figure>

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

* Các trường được đánh dấu bắt buộc không được để trống.
* **Price** của nhóm sản phẩm được hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm.
* Người dùng không cần nhập thủ công **Category** và **Price**.
  * **Category** của nhóm sản phẩm được hệ thống tự tổng hợp từ chương trình học của từng sản phẩm trong nhóm.
  * **Price** của nhóm sản phẩm được hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm.
* Khi **Price** của nhóm sản phẩm thay đổi, các đơn hàng trong tương lai có chứa nhóm sản phẩm sẽ áp dụng giá mới.
* Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ.
* Việc đổi trạng thái nhóm sản phẩm từ **Active** sang **Inactive** không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.
* Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.
* Trường **Products** có bắt buộc phải còn ít nhất một sản phẩm sau khi chỉnh sửa không

***

## V. Các lỗi thường gặp và cách xử lý

Hiện tài liệu gốc chưa cung cấp thông báo lỗi cụ thể của hệ thống. Có thể bổ sung sau khi có ảnh màn hình hoặc nội dung message thực tế.

| Lỗi / Tình huống       | Nguyên nhân                                    | Cách xử lý                                                      |
| ---------------------- | ---------------------------------------------- | --------------------------------------------------------------- |
| This field is required | Người dùng chưa nhập đầy đủ thông tin bắt buộc | Kiểm tra và nhập đầy đủ **Combo name** và **Status, Products.** |

***

## VI. Câu Hỏi Thường Gặp

**Q: Khi thay đổi sản phẩm trong nhóm làm Price thay đổi thì đơn hàng cũ có bị ảnh hưởng không?**\
A: Không. Các đơn hàng đã được tạo trước thời điểm thay đổi giá vẫn áp dụng giá cũ. Các đơn hàng trong tương lai có chứa nhóm sản phẩm sẽ áp dụng giá mới.

**Q: Việc đổi trạng thái nhóm sản phẩm từ Active sang Inactive có ảnh hưởng đến đơn hàng cũ không?**\
A: Không. Việc đổi trạng thái nhóm sản phẩm từ **Active** sang **Inactive** không ảnh hưởng đến các đơn hàng đã được tạo trước thời điểm chuyển đổi trạng thái.

**Q: Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?**\
A: Không. Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.
