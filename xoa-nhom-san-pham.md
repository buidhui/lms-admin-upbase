# Xóa nhóm sản phẩm

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
| 4 | Order          | Đơn hàng được tạo cho học viên                                         |
| 5 | Action         | Khu vực thao tác với một bản ghi trên danh sách                        |
| 6 | Delete         | Chức năng xóa bản ghi khỏi hệ thống hoặc khỏi danh sách hiển thị       |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách xóa nhóm sản phẩm trong tính năng **Combo Products** thuộc module **Payments** trên hệ thống **Operations**.

Sau khi thực hiện xong, nhóm sản phẩm bị xóa sẽ không còn hiển thị trên danh sách nhóm sản phẩm. Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.

### 1.2 Đối tượng áp dụng

| Đối tượng               | Vai trò                                                             | Quyền hạn                         |
| ----------------------- | ------------------------------------------------------------------- | --------------------------------- |
| Người vận hành hệ thống | Quản lý danh mục nhóm sản phẩm phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và xóa nhóm sản phẩm |

### 1.3 Phạm vi & Module liên quan

* **Tính năng chính:** Combo Products
* **Module liên quan:** Products, Promotion Code, Order List

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền xóa nhóm sản phẩm.
* Nhóm sản phẩm cần xóa đã tồn tại trên danh sách nhóm sản phẩm **Combo Products**.
* Người dùng đã xác định đúng nhóm sản phẩm cần xóa trước khi thực hiện thao tác.

***

## II. Tổng Quan Giao Diện

Màn hình danh sách nhóm sản phẩm **Combo Products** cho phép người dùng thực hiện thao tác xóa nhóm sản phẩm thông qua nút **Action > Delete** tại từng dòng nhóm sản phẩm.

![](<.gitbook/assets/image (830)>)

***

## III. Các Bước Thực Hiện Chi Tiết

{% hint style="info" %}
🎯 Mục tiêu: Xóa một nhóm sản phẩm khỏi danh sách nhóm sản phẩm trên hệ thống.
{% endhint %}

{% stepper %}
{% step %}
## Chọn nhóm sản phẩm cần xóa

Tại màn hình danh sách nhóm sản phẩm **Combo Products**, tìm nhóm sản phẩm cần xóa.

Tại dòng nhóm sản phẩm cần xóa, chọn **Action > Delete**.

Kết quả mong đợi:

* Hệ thống hiển thị hộp thoại xác nhận xóa nhóm sản phẩm.
* Người dùng có thể chọn tiếp tục xóa hoặc hủy thao tác.

![](<.gitbook/assets/image (831)>)
{% endstep %}

{% step %}
## Xác nhận thao tác xóa

Tại hộp thoại xác nhận, người dùng chọn một trong hai thao tác sau:

| Nút thao tác | Ý nghĩa                        |
| ------------ | ------------------------------ |
| Yes          | Đồng ý xóa nhóm sản phẩm       |
| No           | Hủy thao tác xóa nhóm sản phẩm |

Người dùng chọn **Yes** để đồng ý xóa nhóm sản phẩm.

Nếu không muốn tiếp tục xóa, người dùng chọn **No** tại hộp thoại xác nhận.

Kết quả mong đợi:

* Hệ thống xóa nhóm sản phẩm khỏi danh sách nhóm sản phẩm.
* Nhóm sản phẩm đã xóa không còn hiển thị trên màn hình danh sách nhóm sản phẩm.
* Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.

![](<.gitbook/assets/image (832)>)
{% endstep %}

{% step %}
## Kiểm tra kết quả sau khi xóa

Sau khi xác nhận xóa, người dùng kiểm tra lại danh sách nhóm sản phẩm.

Kết quả mong đợi:

* Nhóm sản phẩm vừa xóa không còn xuất hiện trên danh sách nhóm sản phẩm.
* Các đơn hàng đã tạo trước đó có chứa nhóm sản phẩm này vẫn được giữ nguyên thông tin.
{% endstep %}
{% endstepper %}

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

* Người dùng cần kiểm tra kỹ nhóm sản phẩm trước khi chọn **Yes** để xác nhận xóa.
* Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.

***

## V. Các lỗi thường gặp và cách xử lý

Updating...

***

## VI. Câu Hỏi Thường Gặp

<details>

<summary>Q: Xóa nhóm sản phẩm có ảnh hưởng đến đơn hàng đã tạo trước đó không?</summary>

A: Không. Việc xóa nhóm sản phẩm không ảnh hưởng đến các đơn hàng đã được tạo trước đó có chứa nhóm sản phẩm này.

</details>

<details>

<summary>Q: Có thể khôi phục nhóm sản phẩm đã xóa không?</summary>

A: Không. Combo đã bị xóa không thể được khôi phục.

</details>
