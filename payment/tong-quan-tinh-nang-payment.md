# Tổng quan tính năng Payment

Nơi đội TVTS quản lý toàn bộ vòng đời của một đơn hàng — từ thiết lập sản phẩm/combo, mã khuyến mãi đến đơn hàng.

Dành cho: Đội ngũ Tư vấn tuyển sinh (TVTS)

#### Nhóm 1 - Quản lý sản phẩm (Products & Combo Products)

[Product](product.md)

Quản lý danh sách sản phẩm đơn lẻ

[Combo](combo.md)

Quản lý danh sách nhóm sản phẩm

#### Nhóm 2 - Quản lý mã khuyến mãi (Promotion Codes)

[Promotion Code](promotion-code.md)

Quản lý các mã khuyến mãi được áp dụng cho từng sản phẩm hoặc nhóm sản phẩm

#### Nhóm 3 - Quản lý danh sách đơn hàng (List of Orders)

[Order List](order-list.md)

Quản lý danh sách đơn hàng, quản lý danh sách giao dịch và checkout

#### Mối liên hệ giữa các tính năng thuộc Module Payment

* Sản phẩm và mã khuyến mại là dữ liệu đầu vào cần được cấu hình trước khi tạo đơn hàng.
*   Khi tạo đơn hàng, người dùng sẽ chọn:

    * Sản phẩm hoặc combo sản phẩm
    * Áp dụng mã khuyến mại (nếu có)

    ⇒ Từ đó, hệ thống ghi nhận đơn hàng và cập nhật trạng thái thanh toán tương ứng.

![](<../.gitbook/assets/image (391)>)
