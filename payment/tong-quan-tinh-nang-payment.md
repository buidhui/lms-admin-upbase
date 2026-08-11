---
description: >-
  Nơi đội TVTS quản lý toàn bộ vòng đời của một đơn hàng — từ thiết lập sản
  phẩm/combo, mã khuyến mãi đến đơn hàng.
---

# Tổng quan tính năng Payment

{% hint style="info" %}
Dành cho: Đội ngũ Tư vấn tuyển sinh (TVTS)
{% endhint %}

#### Nhóm 1 - Quản lý sản phẩm (Products & Combo Products)

<table data-view="cards"><thead><tr><th data-type="content-ref"></th><th></th></tr></thead><tbody><tr><td><a href="product/">product</a></td><td>Quản lý danh sách sản phẩm đơn lẻ</td></tr><tr><td><a href="combo/">combo</a></td><td>Quản lý danh sách nhóm sản phẩm</td></tr></tbody></table>

#### Nhóm 2 - Quản lý mã khuyến mãi (Promotion Codes)

<table data-view="cards"><thead><tr><th></th><th data-type="content-ref"></th><th></th></tr></thead><tbody><tr><td></td><td><a href="promotion-code/">promotion-code</a></td><td>Quản lý các mã khuyến mãi được áp dụng cho từng sản phẩm hoặc nhóm sản phẩm</td></tr></tbody></table>

#### Nhóm 3 - Quản lý danh sách đơn hàng (List of Orders)

<table data-view="cards"><thead><tr><th data-type="content-ref"></th><th></th></tr></thead><tbody><tr><td><a href="order-list/">order-list</a></td><td>Quản lý danh sách đơn hàng, quản lý danh sách giao dịch và checkout</td></tr></tbody></table>

#### Mối liên hệ giữa các tính năng thuộc Module Payment

* Sản phẩm và mã khuyến mại là dữ liệu đầu vào cần được cấu hình trước khi tạo đơn hàng.
*   Khi tạo đơn hàng, người dùng sẽ chọn:

    * Sản phẩm hoặc combo sản phẩm
    * Áp dụng mã khuyến mại (nếu có)

    ⇒ Từ đó, hệ thống ghi nhận đơn hàng và cập nhật trạng thái thanh toán tương ứng.

<figure><img src="../.gitbook/assets/mermaid-diagram (2).png" alt=""><figcaption></figcaption></figure>
