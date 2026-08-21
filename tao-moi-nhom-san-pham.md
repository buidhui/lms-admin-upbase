# Tạo mới nhóm sản phẩm

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

## I. Giới Thiệu Chung

### **1.1 Mục đích**

Tài liệu này hướng dẫn người dùng cách tạo mới nhóm sản phẩm trong tính năng **Combo Products** thuộc module\*\* Payments\*\* trên hệ thống **Operations**.

Sau khi thực hiện xong, nhóm sản phẩm mới sẽ được lưu vào hệ thống và hiển thị trên danh sách nhóm sản phẩm để phục vụ cho các nghiệp vụ liên quan như tạo đơn hàng, gắn mã khuyến mại với nhóm sản phẩm.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                           | Quyền hạn                             |
| ----------------------- | ----------------------------------------------------------------- | ------------------------------------- |
| Người vận hành hệ thống | Tạo và quản lý nhóm sản phẩm phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và tạo mới nhóm sản phẩm |

### **1.3 Phạm vi & Module liên quan**

* **Tính năng chính:** Combo Products
* **Module liên quan:** Products, Promotion Code, Order List

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền tạo mới nhóm sản phẩm.
* Người dùng đang ở màn hình danh sách nhóm sản phẩm **Combo Products**.
* Các sản phẩm đơn lẻ cần đưa vào nhóm sản phẩm đã được tạo trên hệ thống.
* Các danh mục dùng để chọn sản phẩm đã có dữ liệu trong hệ thống.

***

## II. Tổng Quan Giao Diện

Màn hình tạo mới nhóm sản phẩm cho phép người dùng nhập thông tin nhóm sản phẩm và chọn các sản phẩm đơn lẻ thuộc nhóm.

Các thành phần chính trên màn hình gồm:

| Thành phần | Mô tả                                                                                                     |
| ---------- | --------------------------------------------------------------------------------------------------------- |
| Combo name | Tên nhóm sản phẩm                                                                                         |
| Products   | Danh sách sản phẩm được chọn vào nhóm                                                                     |
| Category   | Chương trình học của nhóm sản phẩm. Hệ thống tự tổng hợp từ chương trình học của từng sản phẩm trong nhóm |
| Price      | Giá của nhóm sản phẩm. Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm                     |
| Status     | Trạng thái của nhóm sản phẩm                                                                              |
| Save       | Nút lưu thông tin nhóm sản phẩm                                                                           |

Giá trị của trường **Status** gồm:

| Giá trị  | Ý nghĩa                                                                                               |
| -------- | ----------------------------------------------------------------------------------------------------- |
| Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |

![](<.gitbook/assets/image (823)>)

***

## III. Các Bước Thực Hiện Chi Tiết

{% hint style="info" %}
🎯 Mục tiêu: Tạo mới một nhóm sản phẩm trên hệ thống bằng cách nhập tên nhóm, chọn các sản phẩm thuộc nhóm và thiết lập trạng thái cho nhóm sản phẩm.
{% endhint %}

{% stepper %}
{% step %}
## Truy cập màn hình tạo mới nhóm sản phẩm

Tại màn hình danh sách nhóm sản phẩm **Combo Products (Order & Payment > Product & Combo > Combo Products**), chọn **New Combo**.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình tạo mới nhóm sản phẩm.
* Người dùng có thể bắt đầu nhập thông tin nhóm sản phẩm.

![](<.gitbook/assets/image (824)>)
{% endstep %}

{% step %}
## Nhập tên nhóm sản phẩm

Tại trường **Combo name**, nhập tên nhóm sản phẩm cần tạo.

| Trường thông tin | Bắt buộc | Hướng dẫn nhập                     |
| ---------------- | -------- | ---------------------------------- |
| Combo name       | Có       | Nhập tên nhóm sản phẩm cần tạo mới |

Kết quả mong đợi:

* Tên nhóm sản phẩm được ghi nhận trên form tạo mới.
* Người dùng có thể tiếp tục chọn sản phẩm vào nhóm.

![](<.gitbook/assets/image (825)>)
{% endstep %}

{% step %}
## Chọn sản phẩm vào nhóm

Tại trường **Products**, chọn vào vùng trống của trường để mở màn hình danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, người dùng thực hiện:

* Chọn checkbox tại một hoặc nhiều sản phẩm cần thêm vào nhóm.
* Chọn **Add** để thêm các sản phẩm đã chọn vào nhóm.

![](<.gitbook/assets/image (826)>)

Kết quả mong đợi:

* Các sản phẩm được chọn hiển thị tại trường **Products** của nhóm sản phẩm.
* Hệ thống sử dụng danh sách sản phẩm đã chọn để tự tổng hợp **Category** và tự tính **Price**.

![](<.gitbook/assets/image (827)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin Category và Price

Sau khi chọn sản phẩm vào nhóm, người dùng kiểm tra các thông tin hệ thống tự hiển thị.

| Trường thông tin | Cách xử lý                                                                                                      |
| ---------------- | --------------------------------------------------------------------------------------------------------------- |
| Category         | Hệ thống tự tổng hợp các chương trình học của từng sản phẩm trong nhóm. Người dùng không cần điền thông tin này |
| Price            | Hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm. Người dùng không cần điền thông tin này         |

Kết quả mong đợi:

* **Category** hiển thị theo thông tin của các sản phẩm đã chọn.
* **Price** hiển thị theo tổng giá trị của các sản phẩm đã chọn.
{% endstep %}

{% step %}
## Chọn trạng thái nhóm sản phẩm

Tại trường **Status**, chọn trạng thái của nhóm sản phẩm.

| Trường thông tin | Bắt buộc | Giá trị  | Ý nghĩa                                                                                               |
| ---------------- | -------- | -------- | ----------------------------------------------------------------------------------------------------- |
| Status           | Có       | Active   | Nhóm sản phẩm vẫn đang được kinh doanh                                                                |
| Status           | Có       | Inactive | Nhóm sản phẩm đã ngừng kinh doanh. Nhóm sản phẩm ở trạng thái này sẽ không được thêm vào đơn hàng mới |

Kết quả mong đợi:

* Trạng thái nhóm sản phẩm được ghi nhận trên form tạo mới.

![](<.gitbook/assets/image (828)>)
{% endstep %}

{% step %}
## Lưu thông tin nhóm sản phẩm

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

Kết quả mong đợi:

* Hệ thống lưu thông tin nhóm sản phẩm mới.
* Nhóm sản phẩm vừa tạo hiển thị ở đầu danh sách nhóm sản phẩm.

![](<.gitbook/assets/image (829)>)
{% endstep %}
{% endstepper %}

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

* Các trường được đánh dấu bắt buộc không được để trống.
* Người dùng không cần nhập thủ công **Category** và **Price**.
  * **Category** của nhóm sản phẩm được hệ thống tự tổng hợp từ chương trình học của từng sản phẩm trong nhóm.
  * **Price** của nhóm sản phẩm được hệ thống tự tính bằng tổng giá trị của các sản phẩm trong nhóm.
* Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.
* Nhóm sản phẩm vừa tạo thành công sẽ hiển thị ở đầu danh sách nhóm sản phẩm.

***

## V. Các lỗi thường gặp và cách xử lý

Hiện tài liệu gốc chưa cung cấp thông báo lỗi cụ thể của hệ thống. Có thể bổ sung sau khi có ảnh màn hình hoặc nội dung message thực tế.

| Lỗi / Tình huống       | Nguyên nhân                                    | Cách xử lý                                                         |
| ---------------------- | ---------------------------------------------- | ------------------------------------------------------------------ |
| This field is required | Người dùng chưa nhập đầy đủ thông tin bắt buộc | Kiểm tra và nhập đầy đủ **Combo name**, **Products** và **Status** |

***

## VI. Câu Hỏi Thường Gặp

<details>

<summary>Có cần nhập Category khi tạo nhóm sản phẩm không?</summary>

Không. Hệ thống tự tổng hợp **Category** từ chương trình học của từng sản phẩm trong nhóm.

</details>

<details>

<summary>Có cần nhập Price khi tạo nhóm sản phẩm không?</summary>

Không. Hệ thống tự tính **Price** bằng tổng giá trị của các sản phẩm trong nhóm.

</details>

<details>

<summary>Làm thế nào để thêm sản phẩm vào nhóm?</summary>

Tại trường **Products**, chọn vào vùng trống để mở danh sách sản phẩm. Sau đó chọn checkbox tại một hoặc nhiều sản phẩm và chọn **Add**.

</details>

<details>

<summary>Có thể thêm các sản phẩm Inactive vào nhóm sản phẩm không?</summary>

Không. Danh sách Products chỉ gồm các sản phẩm đang ở trạng thái Active.

</details>

<details>

<summary>Nhóm sản phẩm Inactive có được thêm vào đơn hàng mới không?</summary>

Không. Nhóm sản phẩm ở trạng thái **Inactive** sẽ không được thêm vào đơn hàng mới.

</details>

<details>

<summary>Sau khi tạo mới, nhóm sản phẩm hiển thị ở đâu?</summary>

Nhóm sản phẩm vừa tạo sẽ hiển thị ở đầu danh sách nhóm sản phẩm.

</details>
