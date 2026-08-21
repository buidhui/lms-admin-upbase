# Xem danh sách/chi tiết sản phẩm đơn lẻ

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create New         | 3.0.0   |

## Definitions and Acronyms

| # | Term     | Definition       |
| - | -------- | ---------------- |
| 1 | Ops      | Operations       |
| 2 | Product  | Sản phẩm đơn lẻ  |
| 3 | Category | Chương trình học |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách xem danh sách sản phẩm đơn lẻ và xem thông tin chi tiết sản phẩm trong hệ thống.

### 1.2 Đối tượng áp dụng

| Đối tượng       | Vai trò                 | Quyền hạn                          |
| --------------- | ----------------------- | ---------------------------------- |
| Operations User | Người vận hành hệ thống | Xem danh sách và chi tiết sản phẩm |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Products
* **Module liên quan:** [Program](/broken/pages/60d8ad886d1deb674dc83f513d97c407496f5c4d)
* **Hệ thống tích hợp:** Không áp dụng

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập hệ thống.
* Người dùng có quyền truy cập menu: **Operations → Order & Payment → Products & Combo → Products**

## II. Tổng Quan Giao Diện

![](<.gitbook/assets/image (801)>)

Màn hình Products cho phép người dùng:

* Xem danh sách sản phẩm đơn lẻ
* Tìm kiếm sản phẩm
* Xem thông tin chi tiết sản phẩm

Các thông tin hiển thị trên màn hình:

| Thông tin         | Mô tả               |
| ----------------- | ------------------- |
| Product name      | Tên sản phẩm        |
| Price             | Đơn giá sản phẩm    |
| Category          | Chương trình học    |
| Construction mode | Hình thức học       |
| Status            | Trạng thái sản phẩm |

#### Ý nghĩa trạng thái sản phẩm

| Trạng thái | Mô tả                                                                              |
| ---------- | ---------------------------------------------------------------------------------- |
| Active     | Sản phẩm đang được kinh doanh                                                      |
| Inactive   | Sản phẩm đã ngừng kinh doanh và không thể thêm vào nhóm sản phẩm hoặc đơn hàng mới |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Xem danh sách sản phẩm đơn lẻ

{% hint style="info" %}
🎯 **Mục tiêu:** Người dùng xem danh sách sản phẩm và tìm kiếm sản phẩm theo điều kiện mong muốn.
{% endhint %}

{% stepper %}
{% step %}
#### Truy cập màn hình Products

Tại thanh menu hệ thống, chọn: **Operations → Order & Payment → Products & Combo → Products**

![](<.gitbook/assets/image (804)>)

Hệ thống hiển thị danh sách sản phẩm đơn lẻ.

Người dùng có thể tìm kiếm theo các điều kiện:

| Điều kiện tìm kiếm | Mô tả                      |
| ------------------ | -------------------------- |
| Search Product     | Tìm theo tên sản phẩm      |
| Category           | Chọn chương trình học      |
| Status             | Chọn trạng thái sản phẩm   |
| Sort by            | Chọn cách sắp xếp sản phẩm |

Chọn **Search** để hiển thị danh sách sản phẩm theo điều kiện tìm kiếm.

Chọn **Reset** để xóa toàn bộ điều kiện tìm kiếm và hiển thị lại danh sách mặc định.
{% endstep %}
{% endstepper %}

### 3.2 Xem chi tiết sản phẩm đơn lẻ

{% hint style="info" %}
🎯 **Mục tiêu:** Người dùng xem thông tin chi tiết của sản phẩm.
{% endhint %}

{% stepper %}
{% step %}
#### Chọn sản phẩm cần xem

Tại màn hình danh sách sản phẩm, click vào giá trị tại cột **Product Name**.

![](<.gitbook/assets/image (806)>)
{% endstep %}

{% step %}
#### Hoàn tất

Hệ thống hiển thị màn hình chi tiết sản phẩm tương ứng.

![](<.gitbook/assets/image (808)>)
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
**⚠️ Lưu ý quan trọng**

* Các sản phẩm ở trạng thái **Inactive** sẽ không thể thêm vào nhóm sản phẩm hoặc đơn hàng mới.
* Người dùng nên sử dụng bộ lọc tìm kiếm để dễ dàng tra cứu dữ liệu khi danh sách sản phẩm lớn.
{% endhint %}

{% hint style="info" %}
**💡 Mẹo sử dụng**

* Có thể kết hợp nhiều điều kiện tìm kiếm để thu hẹp kết quả nhanh hơn.
{% endhint %}

## V. Các lỗi thường gặp và cách xử lý

| Lỗi / Tình huống                  | Nguyên nhân            | Cách xử lý                   |
| --------------------------------- | ---------------------- | ---------------------------- |
| Không tìm thấy dữ liệu            | Sai điều kiện tìm kiếm | Kiểm tra lại bộ lọc tìm kiếm |
| Không truy cập được menu Products | Chưa được cấp quyền    | Liên hệ quản trị hệ thống    |

## VI. Câu Hỏi Thường Gặp

<details>

<summary>Vì sao sản phẩm không hiển thị trong danh sách?</summary>

Có thể sản phẩm không thỏa điều kiện tìm kiếm hoặc người dùng chưa có quyền truy cập.

</details>

<details>

<summary>Sản phẩm Inactive có sử dụng được không?</summary>

Không. Sản phẩm Inactive không thể thêm vào nhóm sản phẩm hoặc đơn hàng mới.

</details>
