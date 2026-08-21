# Quản lý danh sách đơn hàng

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date  | Update Person | A,M,D | Change Description                                | Version |
| --------------- | ------------- | ----- | ------------------------------------------------- | ------- |
| August 15, 2025 | Nhungdh       | A     | Create New                                        | 3.0.0   |
| June 8, 2026    | Nhungnth      | M     | Cập nhật tính năng Order List                     | 3.1.0   |
| July 15, 2026   | Nhungnth      | M     | Cập nhật tính năng thanh toán nhiều lần qua VNPay | 3.2.0   |

## I. Thông tin chung

### **Đối tượng sử dụng**

* Dành cho: Admin, TVTS
* Đường dẫn: [https://ops.sapp.edu.vn/operations/sales/orders?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/operations/sales/orders?page_index=1\&page_size=10)

#### Phạm vi & Module liên quan

* **Module chính**: Order List
* **Module liên quan**: [Product](payment/product.md), [Combo Product](payment/combo.md), [Promotion Codes](payment/promotion-code.md)
* **Hệ thống tích hợp**: Hubspot

### Điều kiện tiên quyết

Đã đăng nhập và được quyền truy cập vào module Order List.

## II. Hướng dẫn chi tiết

> Order List là danh sách các đơn hàng được tạo bởi TVTS, khi khách hàng mua các sản phẩm (khóa học) được cung cấp bởi SAPP.

### Xem danh sách đơn hàng

{% stepper %}
{% step %}
## Truy cập màn hình List of Orders

Tại thanh menu hệ thống: chọn Order & Payment → **Order List**

![](<.gitbook/assets/image (880)>)
{% endstep %}

{% step %}
## User có thể tìm kiếm đơn hàng theo điều kiện

* Search Deal ID: theo deal id của deal hubspot gắn với đơn hàng
* Product: Chọn 1 giá trị trong danh sách cho trước
* Status: Chọn 1 giá trị trong danh sách cho trước.
* Sort by: Chọn cách sắp xếp sản phẩm (A-Z, Z-A, Lastest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

![](<.gitbook/assets/image (881)>)

Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết đơn hàng

{% stepper %}
{% step %}
## Chọn đơn hàng cần xem chi tiết

Tại màn hình danh sách Orders, click chọn 1 trong các thông tin dưới đây để xem chi tiết thông tin đơn hàng:

* Mã đơn hàng
* Product
* Combo

![](<.gitbook/assets/image (882)>)

![](<.gitbook/assets/image (883)>)
{% endstep %}

{% step %}
## Xem thông tin **Overview** của đơn hàng

Tab Overview của đơn hàng bao gồm các sections cụ thể dưới đây.

### 2.1. Section Order Amount

| Trường thông tin           | Ý nghĩa                                                                                                                                       |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Gross Amount**           | <p>Tổng giá trị của Order (trước ưu đãi)<br><br>Công thức tính: Gross Amount = Gross Price (Product) + Gross Price (Combo Product)</p>        |
| **Total Product Discount** | Số tiền ưu đãi được áp dụng cho Product và Combo Product user đã chọn                                                                         |
| **Order Discount**         | Số tiền ưu đãi được áp dụng trên toàn bộ đơn hàng                                                                                             |
| **Net Amount**             | <p>Học phí sau ưu đãi của đơn hàng<br><br>Công thức tính: Net Amount = Gross Amount - Total Product Discount - Order Discount</p>             |
| **Paid Amount**            | Tổng số tiền khách hàng đã thanh toán                                                                                                         |
| **Pay-back**               | Tổng số học phí cần hoàn lại cho khách hàng                                                                                                   |
| **Total Amount Due**       | <p>Tổng số tiền khách hàng còn phải thanh toán trên đơn hàng<br><br>Công thức tính: Total Amount Due = Net Amount - Paid Amount + Payback</p> |

![](<.gitbook/assets/image (884)>)

### 2.2. Section Customer Info

| Trường thông tin được đồng bộ     | Ý nghĩa                                                            | Property đồng bộ                                        |
| --------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------- |
| **Deal ID**                       | Deal ID tương ứng với đơn hàng                                     |                                                         |
| **Full name**                     | Tên đầy đủ của khách hàng.                                         | Đồng bộ từ Contact property: \[TVTS] Họ tên             |
| **Email**                         | Email của khách hàng                                               | Đồng bộ từ Contact property: Email                      |
| **Phone**                         | Số điện thoại của khách hàng                                       | Đồng bộ từ Contact property: \[TVTS] Phone number       |
| **Tỉnh/Thành phố**                | Khu vực sinh sống của khách hàng                                   | Đồng bộ từ Contact property: \[TVTS] Khu vực sinh sống  |
| **Địa chỉ**                       | Địa chỉ của khách hàng                                             | Đồng bộ từ Contact property: \[TVTS] Địa chỉ            |
| **Deal ID đã thanh toán học phí** | Deal của khách hàng đã bị đánh lost trước đó (do có lỗi phát sinh) | Đồng bộ từ Deal property: Deal ID đã thanh toán học phí |

![](<.gitbook/assets/image (885)>)

### 2.3. Section Product Info

Các thông tin được thể hiện theo _**từng sản phẩm**_ như sau:

| Trường thông tin            | Ý nghĩa                                                                                                                                                                          |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Product #**               | Tên từng sản phẩm có trong đơn hàng Cho phép chọn các sản phẩm từ danh sách                                                                                                      |
| **Product - Main course**   | <p>Gói khóa học tương ứng với sản phẩm khách hàng mua.<br><br>Tự động cập nhật theo Product đã chọn. Trong đó, <em>Product</em> được xác định dựa trên Category của sản phẩm</p> |
| **Gross Price**             | Giá gốc của sản phẩm lựa chọn Hệ thống cập nhật tự động                                                                                                                          |
| **Product Discount**        | Tổng số tiền được discount đối với sản phẩm lựa chọn                                                                                                                             |
| **Custom Product Discount** | Số tiền học viên được discount bổ sung đối với sản phẩm được chọn                                                                                                                |
| **Net Price**               | <p>Giá sau ưu đãi của sản phẩm<br><br>Công thức tính: Net Price = Gross Price - (Product Discount + Custom Product Discount)</p>                                                 |

![](<.gitbook/assets/image (886)>)

Các thông tin được thể hiện theo từng _**nhóm sản phẩm**_ như sau:

| Trường thông tin          | Ý nghĩa                                                                                                                                                                               |
| ------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Combo #**               | Tên từng nhóm sản phẩm có trong đơn hàng Cho phép chọn nhiều nhóm sản phẩm từ danh sách                                                                                               |
| **Product - Main course** | <p>Gói khóa học tương ứng với các sản phẩm có trong combo khách hàng mua.<br><br>Tự động cập nhật theo Product thuộc Combo đã chọn - được xác định dựa trên Category của sản phẩm</p> |
| **Gross Price**           | Giá gốc của nhóm sản phẩm lựa chọn. Hệ thống cập nhật tự động                                                                                                                         |
| **Combo Discount**        | <p>Tổng số tiền được discount đối với nhóm sản phẩm lựa chọn<br><br>Hệ thống cập nhật tự động.</p>                                                                                    |
| **Custom Combo Discount** | Số tiền học viên được discount bổ sung đối với nhóm sản phẩm được chọn Tự động cập nhật theo Discount rate và Custom Discount                                                         |
| **Net Price**             | <p>Giá sau ưu đãi của nhóm sản phẩm<br><br>Công thức tính: Net Price = Gross Price - (Product Discount + Custom Product Discount)</p>                                                 |

![](<.gitbook/assets/image (887)>)

### 2.4. Section Course Package

| Trường thông tin   | Ý nghĩa                              |
| ------------------ | ------------------------------------ |
| **Add-On Courses** | Gói khóa học tặng kèm cho khách hàng |

![](<.gitbook/assets/image (888)>)

### 2.5. Section Order Info

| Trường thông tin                   | Ý nghĩa                                                       |
| ---------------------------------- | ------------------------------------------------------------- |
| **Discount Code for Entire Order** | Danh sách các mã khuyến mãi được áp dụng cho toàn bộ đơn hàng |
| **Order Discount**                 | Giá trị ưu đãi được áp dụng cho toàn bộ đơn hàng              |

![](<.gitbook/assets/image (889)>)

### 2.4. Section Payment Info

| Trường thông tin     | Ý nghĩa                                                                                                                                       |
| -------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| **Paid Amount**      | Tổng số tiền khách hàng đã thanh toán                                                                                                         |
| **Total Amount Due** | <p>Tổng số tiền khách hàng còn phải thanh toán trên đơn hàng<br><br>Công thức tính: Total Amount Due = Net Amount - Paid Amount + Payback</p> |

![](<.gitbook/assets/image (890)>)
{% endstep %}

{% step %}
## Xem thông tin đồng bộ giữa Hubspot và Ops

Tab Hubspot của đơn hàng bao gồm các sections cụ thể dưới đây.

### 3.1. Data Synchronized from HubSpot

| Trường thông tin được đồng bộ     | Ý nghĩa                                                            | Property đồng bộ từ Hubspot                             |
| --------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------- |
| **Deal ID**                       | Deal ID tương ứng với đơn hàng                                     |                                                         |
| **Full name**                     | Tên đầy đủ của khách hàng.                                         | Đồng bộ từ Contact property: \[TVTS] Họ tên             |
| **Email**                         | Email của khách hàng                                               | Đồng bộ từ Contact property: Email                      |
| **Phone**                         | Số điện thoại của khách hàng                                       | Đồng bộ từ Contact property: \[TVTS] Phone number       |
| **Tỉnh/Thành phố**                | Khu vực sinh sống của khách hàng                                   | Đồng bộ từ Contact property: \[TVTS] Khu vực sinh sống  |
| **Địa chỉ**                       | Địa chỉ của khách hàng                                             | Đồng bộ từ Contact property: \[TVTS] Địa chỉ            |
| **Deal ID đã thanh toán học phí** | Deal của khách hàng đã bị đánh lost trước đó (do có lỗi phát sinh) | Đồng bộ từ Deal property: Deal ID đã thanh toán học phí |

![](<.gitbook/assets/image (891)>)

### 3.2. Data Synchronized to HubSpot

| Trường thông tin được đồng bộ | Ý nghĩa                                                                                                                                | Property đồng bộ từ Hubspot                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ----------------------------- | -------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Product - Main couse**      | Deal ID tương ứng với đơn hàng                                                                                                         | <p>Tương ứng với Category, được đồng bộ về các Deal properties:<br><br>1. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=G%C3%B3i%20kh%C3%B3a%20h%E1%BB%8Dc%20ch%C3%ADnh&#x26;action=edit&#x26;property=acca___lo_trinh_dang_ky">ACCA - Gói khóa học chính</a><br>2. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=G%C3%B3i%20kh%C3%B3a%20h%E1%BB%8Dc%20ch%C3%ADnh&#x26;action=edit&#x26;property=cfa___lo_trinh_dang_ky">CFA - Gói khóa học chính</a><br>3. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=G%C3%B3i%20kh%C3%B3a%20h%E1%BB%8Dc%20ch%C3%ADnh&#x26;action=edit&#x26;property=cma___lo_trinh_dang_ky">CMA - Gói khóa học chính</a><br>4. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=G%C3%B3i%20kh%C3%B3a%20h%E1%BB%8Dc%20ch%C3%ADnh&#x26;action=edit&#x26;property=ifrs___lo_trinh_dang_ky">IFRS - Gói khóa học chính</a><br>5. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=G%C3%B3i%20kh%C3%B3a%20h%E1%BB%8Dc%20ch%C3%ADnh&#x26;action=edit&#x26;property=shortcourse___lo_trinh_dang_ky">Shortcourse - Gói khóa học chính</a><br>6. <a href="https://app.hubspot.com/property-settings/1774127/properties?type=0-3&#x26;search=CGMA%20-&#x26;action=edit&#x26;property=cgma___goi_khoa_hoc_chinh">CGMA - Gói khóa học chính</a></p> |
| **Add-on Couse**              | Tên đầy đủ của khách hàng.                                                                                                             | Đồng bộ về Deal property: [\[TVTS\] Gói khóa học tặng kèm](https://app.hubspot.com/property-settings/1774127/properties?type=0-3\&search=t%E1%BA%B7ng%20k%C3%A8m\&action=edit\&property=goi_khoa_hoc_tang_kem)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| **Gross Amount**              | <p>Tổng giá trị của Order (trước ưu đãi)<br><br>Công thức tính: Gross Amount = Gross Price (Product) + Gross Price (Combo Product)</p> | Đồng bộ về Deal property: [\[TVTS\] Học phí gốc](https://app.hubspot.com/property-settings/1774127/properties?type=0-3\&search=h%E1%BB%8Dc%20ph%C3%AD%20g%E1%BB%91c\&action=edit\&property=hoc_phi_goc)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Total Order Discount**      | Số điện thoại của khách hàng                                                                                                           | Đồng bộ về Deal property: [\[TVTS\] Học phí ưu đãi áp dụng](https://app.hubspot.com/property-settings/1774127/properties?type=0-3\&search=%C6%B0u%20%C4%91%C3%A3i\&action=edit\&property=hoc_phi_uu_dai)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Net Amount**                | Khu vực sinh sống của khách hàng                                                                                                       | Đồng bộ về Deal property: [Amount](https://app.hubspot.com/property-settings/1774127/properties?type=0-3\&search=amount\&action=edit\&property=amount)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| **Paid Amount**               | Địa chỉ của khách hàng                                                                                                                 | Hệ thống tính tự động                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Total Amount Due**          | Deal của khách hàng đã bị đánh lost trước đó (do có lỗi phát sinh)                                                                     | Hệ thống tính tự động                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| **Order ID**                  | Mã đơn hàng trên Ops                                                                                                                   | Đồng bộ về Deal property: [Order ID](https://app.hubspot.com/property-settings/1774127/properties?type=0-3\&search=order%20id\&action=edit\&property=order_id)                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |

#### Lưu ý về đồng bộ thông tin lên HubSpot

User có thể chọn **Resync** để đồng bộ lại thông tin đơn hàng trong trường hợp Synchronized Status = Thất bại

![](<.gitbook/assets/image (892)>)

### 3.3. Data Synchronized — Thông tin giao dịch

Tương ứng mỗi Transaction với Transaction Type = Thu học phí, thông tin giao dịch đều được đồng bộ lên HubSpot theo nguyên tắc như sau:

| Trường thông tin            | Ý nghĩa                              |
| --------------------------- | ------------------------------------ |
| **Amount paid by students** | Số tiền học viên thanh toán từng lần |
| **Payment Method**          | Phương thức thanh toán từng lần      |
| **Paid date**               | Ngày thanh toán từng lần             |

Trong đó, chi tiết Payment Method được ghi nhận như sau:

| Phương thức thanh toán lần # | Trường hợp ghi nhận                                              |
| ---------------------------- | ---------------------------------------------------------------- |
| MB SAPP                      | Khách hàng mua các sản phẩm có Category = B2B hoặc CGMA          |
| MB SAA                       | Khách hàng mua các sản phẩm có Category = ACCA hoặc Cert/Dip     |
| MB SCFA                      | Khách hàng mua các sản phẩm có Category = CFA                    |
| MB SCMA                      | Khách hàng mua các sản phẩm có Category = CMA hoặc Short courses |

| Phương thức thanh toán lần # | Trường hợp ghi nhận                                                                                     |
| ---------------------------- | ------------------------------------------------------------------------------------------------------- |
| VNPay TT                     | Khách hàng thanh toán với Hình thức thanh toán = Trả thẳng, phương thức thanh toán = Thanh toán qua thẻ |
| VNPay TG                     | Khách hàng thanh toán với Hình thức thanh toán = Trả góp, phương thức thanh toán = VNPay                |

| Phương thức thanh toán lần # | Trường hợp ghi nhận                                                                                     |
| ---------------------------- | ------------------------------------------------------------------------------------------------------- |
| POS TT                       | Khách hàng thanh toán với Hình thức thanh toán = Trả thẳng, phương thức thanh toán = Thanh toán qua thẻ |
| POS TG                       | Khách hàng thanh toán với Hình thức thanh toán = Trả góp, phương thức thanh toán = VNPay                |

| Phương thức thanh toán lần # | Trường hợp ghi nhận                                   |
| ---------------------------- | ----------------------------------------------------- |
| TM NEU                       | Khách hàng thanh toán học phí trực tiếp tại cơ sở NEU |
| TM UEH                       | Khách hàng thanh toán học phí trực tiếp tại cơ sở UEH |

![](<.gitbook/assets/image (893)>)
{% endstep %}

{% step %}
## Xem **Transaction List** của đơn hàng

Tham chiếu nội dung chi tiết tại [Quản lý danh sách giao dịch](quan-ly-danh-sach-giao-dich.md)
{% endstep %}
{% endstepper %}

### Tạo mới đơn hàng

{% stepper %}
{% step %}
## Tại màn hình List of Orders, chọn **New Order**

![](<.gitbook/assets/image (894)>)
{% endstep %}

{% step %}
## Tại section Customer Info: Cập nhật **Deal ID** > Chọn **Đồng bộ thông tin**

* User nhập Deal ID của deal tương ứng trên HubSpot.
* Hệ thống tự động đồng bộ thông tin khách hàng từ HubSpot như dưới đây:

| Trường thông tin được đồng bộ | Ý nghĩa                                                            | Property đồng bộ                                        |
| ----------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------- |
| Full name                     | Tên đầy đủ của khách hàng.                                         | Đồng bộ từ Contact property: \[TVTS] Họ tên             |
| Email                         | Email của khách hàng                                               | Đồng bộ từ Contact property: Email                      |
| Phone                         | Số điện thoại của khách hàng                                       | Đồng bộ từ Contact property: \[TVTS] Phone number       |
| Tỉnh/Thành phố                | Khu vực sinh sống của khách hàng                                   | Đồng bộ từ Contact property: \[TVTS] Khu vực sinh sống  |
| Địa chỉ                       | Địa chỉ của khách hàng                                             | Đồng bộ từ Contact property: \[TVTS] Địa chỉ            |
| Deal ID đã thanh toán học phí | Deal của khách hàng đã bị đánh lost trước đó (do có lỗi phát sinh) | Đồng bộ từ Deal property: Deal ID đã thanh toán học phí |

![](<.gitbook/assets/image (895)>)

![](<.gitbook/assets/image (896)>)
{% endstep %}

{% step %}
## Tại section **Product Info**: Thêm **Product** (nếu có)

* Chọn Add Product > Chọn **Select** để thêm các sản phẩm từ màn hình danh sách.

![](<.gitbook/assets/image (897)>)

![](<.gitbook/assets/image (898)>)

{% hint style="info" %}
User tìm kiếm nhanh sản phẩm theo các điều kiện dưới đây:

* Product name
* Category
* Sort by (A-Z, Z-A, Latest, Oldest)
{% endhint %}

* Chọn Discount code tương ứng của sản phẩm, cho phép _**chọn nhiều mã cùng lúc**_.

![](<.gitbook/assets/image (899)>)

![](<.gitbook/assets/image (900)>)

{% hint style="info" %}
**Lưu ý**: Trường hợp không tìm được discount code phù hợp, cho phép user **tạo Promotion code** ngay tại giao diện Select Promotions. Chi tiết hướng dẫn tạo Promotion code [tại đây](payment/promotion-code.md#tao-moi-ma-khuyen-mai).
{% endhint %}

![](<.gitbook/assets/image (901)>)

![](<.gitbook/assets/image (902)>)

* Tick checkbox "_**Apply a custom discount on this product?**_" trong trường hợp sản phẩm được áp dụng bổ sung các mã khuyến mãi.

→ Chọn **Type of Custom Product Discount**

![](<.gitbook/assets/image (903)>)

Chi tiết các trường thông tin của Product trên đơn hàng được thể hiện dưới đây:

| Trường thông tin                  | Ý nghĩa                                                                                                                                                                                                     |
| --------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Product #                         | Tên từng sản phẩm có trong đơn hàng Cho phép chọn các sản phẩm từ danh sách                                                                                                                                 |
| Product - Main course             | <p>Gói khóa học tương ứng với sản phẩm khách hàng mua.<br><br>Tự động cập nhật theo Product đã chọn. Trong đó, <em>Product</em> được xác định dựa trên Category của sản phẩm</p>                            |
| Gross Price                       | Giá gốc của sản phẩm lựa chọn Hệ thống cập nhật tự động                                                                                                                                                     |
| Discount code                     | Mã khuyến mãi áp dụng trên sản phẩm Cho phép _**chọn nhiều mã**_ khuyến mại cùng lúc                                                                                                                        |
| Product Discount                  | <p>Tổng số tiền được discount đối với sản phẩm lựa chọn<br><br>Hệ thống cập nhật tự động.</p>                                                                                                               |
| Apply of Custom Product Discount? | Xác nhận áp dụng khuyến mại bổ sung                                                                                                                                                                         |
| Type of Custom Product Discount   | <p>Lựa chọn loại khuyến mại bổ sung được áp dụng, bao gồm:<br><br>- <strong>Fixed Amount</strong>: giảm trừ bổ sung theo số tiền nhất định<br>- <strong>Percent</strong>: giảm trừ bổ sung theo tỷ lệ %</p> |
| Discount Rate                     | Tỷ lệ % khuyến mại được áp dụng bổ sung Chỉ cập nhật trong trường hợp Type of Custom Product Discount = Percent                                                                                             |
| Custom Discount                   | Số tiền học viên được discount bổ sung Chỉ cập nhật trong trường hợp Type of Custom Product Discount = Fixed Amount                                                                                         |
| Custom Product Discount           | Số tiền học viên được discount bổ sung đối với sản phẩm được chọn Hệ thống cập nhật tự động dựa trên Discount Rate và Custom Discount                                                                       |
| Net Price                         | <p>Giá sau ưu đãi của sản phẩm<br><br>Công thức tính: Net Price = Gross Price - (Product Discount + Custom Product Discount)</p>                                                                            |

Lưu ý: Trường hợp user muốn **Xóa** hoặc **Thêm** sản phẩm > Chọn Delete Product hoặc Add Product tại section Product.

![](<.gitbook/assets/image (904)>)
{% endstep %}

{% step %}
## Tại section **Product Info**: Thêm **Combo** **(nếu có)**

* Chọn Add Combo > Chọn **Select** để thêm các nhóm sản phẩm từ màn hình danh sách

![](<.gitbook/assets/image (905)>)

![](<.gitbook/assets/image (906)>)

{% hint style="info" %}
User tìm kiếm nhanh nhóm sản phẩm theo các điều kiện dưới đây:

* Combo name
* Product
* Category
* Sort by (A-Z, Z-A, Latest, Oldest)
{% endhint %}

* Chọn Discount code áp dụng cho nhóm sản phẩm, cho phép _**chọn nhiều mã cùng lúc**_.

![](<.gitbook/assets/image (907)>)

![](<.gitbook/assets/image (908)>)

{% hint style="info" %}
**Lưu ý**: Trường hợp không tìm được discount code phù hợp, cho phép user **tạo Promotion code** ngay tại giao diện Select Promotions. Chi tiết hướng dẫn tạo Promotion code [tại đây](payment/promotion-code.md#tao-moi-ma-khuyen-mai).
{% endhint %}

* Tick checkbox "_**Apply a custom discount on this combo?**_" trong trường hợp nhóm sản phẩm được áp dụng bổ sung các mã khuyến mãi.

→ Chọn **Type of Custom Combo Discount**

![](<.gitbook/assets/image (909)>)

Chi tiết các trường thông tin của Combo trên đơn hàng được thể hiện dưới đây:

| Trường thông tin                | Ý nghĩa                                                                                                                                                                                                     |
| ------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Combo #                         | Tên từng nhóm sản phẩm có trong đơn hàng Cho phép chọn nhiều nhóm sản phẩm từ danh sách                                                                                                                     |
| Product - Main course           | <p>Gói khóa học tương ứng với các sản phẩm có trong combo khách hàng mua.<br><br>Tự động cập nhật theo Product thuộc Combo đã chọn - được xác định dựa trên Category của sản phẩm</p>                       |
| Gross Price                     | Giá gốc của nhóm sản phẩm lựa chọn. Hệ thống cập nhật tự động                                                                                                                                               |
| Discount code                   | Mã khuyến mãi áp dụng trên nhóm sản phẩm Cho phép _**chọn nhiều mã**_ khuyến mại cùng lúc                                                                                                                   |
| Combo Discount                  | <p>Tổng số tiền được discount đối với nhóm sản phẩm lựa chọn<br><br>Hệ thống cập nhật tự động.</p>                                                                                                          |
| Apply of Custom Combo Discount? | Xác nhận áp dụng khuyến mại bổ sung đối với combo                                                                                                                                                           |
| Type of Custom Combo Discount   | <p>Lựa chọn loại khuyến mại bổ sung được áp dụng, bao gồm:<br><br>- <strong>Fixed Amount</strong>: giảm trừ bổ sung theo số tiền nhất định<br>- <strong>Percent</strong>: giảm trừ bổ sung theo tỷ lệ %</p> |
| Discount Rate                   | Tỷ lệ % khuyến mại được áp dụng bổ sung Chỉ cập nhật trong trường hợp Type of Custom Product Discount = **Percent**                                                                                         |
| Custom Discount                 | Số tiền học viên được discount bổ sung Chỉ cập nhật trong trường hợp Nếu Type of Custom Product Discount = **Fixed Amount**                                                                                 |
| Custom Combo Discount           | Số tiền học viên được discount bổ sung đối với nhóm sản phẩm được chọn Tự động cập nhật theo Discount rate và Custom Discount                                                                               |
| Net Price                       | <p>Giá sau ưu đãi của nhóm sản phẩm<br><br>Công thức tính: Net Price = Gross Price - (Product Discount + Custom Product Discount)</p>                                                                       |

Lưu ý: Trường hợp user muốn **Xóa** hoặc **Thêm** nhóm sản phẩm > Chọn Delete Combo Product hoặc Add Combo Product tại section Combo.

![](<.gitbook/assets/image (910)>)
{% endstep %}

{% step %}
## Chọn **Discount Code for Entire Order** **(nếu có)**

User chọn Discount Code từ màn hình danh sách Promotion Code.

![](<.gitbook/assets/image (911)>)

Cho phép tìm kiếm nhanh theo các điều kiện dưới đây:

* Name: Tên của mã khuyến mại
* Category:
* Sort by (A-Z, Z-A, Latest, Oldest)
* From date - To date: Thời gian hiệu lực của promotion code

| Trường thông tin               | Ý nghĩa                                                                                                         |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------- |
| Discount code for Entire Order | Các mã khuyến mại được áp dụng cho toàn bộ đơn hàng                                                             |
| Order Discount                 | Số tiền học viên được giảm giá trên toàn bộ đơn hàng Hệ thống tự động cập nhật theo Order Discount Code đã chọn |
{% endstep %}

{% step %}
## Tại section Course Package: Chọn **Add-on Course**

User chọn các khóa học học viên được tặng kèm trên Order

![](<.gitbook/assets/image (912)>)
{% endstep %}

{% step %}
## Tại section Payment Info: User quyết định khách hàng có thể thanh toán nhiều lần qua VNPay hay không?

Trong đó, nếu:

* Nếu khách hàng có thể thanh toán thành nhiều lần khi trả thẳng qua VNPay: User tick vào checkbox **Allow customer to split payment via VNPay**
* Nếu khách hàng không được thanh toán thành nhiều lần khi trả thẳng qua VNPay: User KHÔNG TICK vào checkbox trên

![](<.gitbook/assets/image (913)>)

Lưu ý về một số bối cảnh để đảm bảo khách hàng được thanh toán nhiều lần qua VNPay. Cụ thể như sau:

| Tình huống                                                                                                                                                                       | Cách thức xử lý của TVTS                                           | Cách thức hệ thống xử lý                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Khách hàng muốn chuyển khoản/tiền mặt/quẹt POS một phần, còn lại là Trả góp.                                                                                                     | Không tick checkbox **Allow customer to split payment via VNPay?** | Hoạt động vận hành không thay đổi so với hiện tại                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Khách hàng muốn thanh toán 2 lần qua chuyển khoản/tiền mặt/quẹt POS và VNPay _**(không xác định thứ tự trước - sau)**_                                                           | Tick checkbox **Allow customer to split payment via VNPay?**       | <p>Trong trường hợp khách hàng lựa chọn thanh toán qua VNPay trước, hệ thống sẽ hiển thị màn hình cho phép:<br><br>1. Lựa chọn Ngân hàng thanh toán<br>2. Nhập số tiền muốn thanh toán từng lần</p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| Khách hàng muốn Trả thẳng qua thẻ một phần, còn lại là Trả góp.                                                                                                                  | Tick checkbox **Allow customer to split payment via VNPay?**       | <p>1. <strong>Khách hàng thanh toán 1 &#x26; 2 qua VNPay TT</strong>: Hệ thống sẽ hiển thị màn hình cho phép:<br>- Lựa chọn Ngân hàng thanh toán<br>- Nhập số tiền muốn thanh toán từng lần hoặc chọn Thanh toán toàn bộ giá trị đơn hàng<br><br>2. <strong>Khách hàng thanh toán lần 3 qua VNPay TG</strong>: Khách hàng thanh toán toàn bộ số tiền còn lại</p>                                                                                                                                                                                                                                                                                                                                                                                                |
| Khách hàng muốn thanh toán thành 3 lần, mỗi lần với 1 thẻ thanh toán khác nhau                                                                                                   | Tick checkbox **Allow customer to split payment via VNPay?**       | <p>1. <strong>Khách hàng thanh toán lần 1 &#x26; lần 2</strong>: Hệ thống sẽ hiển thị màn hình cho phép:<br>- Lựa chọn Ngân hàng thanh toán<br>- Nhập số tiền muốn thanh toán từng lần hoặc chọn Thanh toán toàn bộ giá trị đơn hàng<br><br>2. <strong>Khách hàng thanh toán lần 3→</strong> Hệ thống hiển thị cho phép:Khách hàng lựa chọn ngân hàng thanh toán &#x26; hiển thị chính xác số tiền còn phải thanh toán</p>                                                                                                                                                                                                                                                                                                                                      |
| <p>Khách hàng muốn thanh toán thành 3 lần, trong đó:<br><br>1. Lần 1: Chuyển khoản<br>2. Lần 2: Thanh toán qua thẻ trả thẳng<br>3. Lần 3: Ghé qua SAPP trả nốt bằng tiền mặt</p> | Tick vào checkbox **Allow customer to split payment via VNPay?**   | <p>1. <strong>Khách hàng thanh toán lần 1 → Hệ thống hiển thị cho phép:</strong> Khách hàng truy cập và thực hiện thanh toán bằng VietQR trước → Chọn Trả thẳng, chọn Chuyển khoản qua VietQR<br><br>2. <strong>Khách hàng thanh toán lần 2 → Hệ thống hiển thị cho phép:</strong><br>1. Khách hàng truy cập và thực hiện thanh toán bằng VNPay với thẻ → Chọn Trả thẳng, chọn Thanh toán qua Thẻ.<br>2. Chọn loại thẻ thanh toán &#x26; Tiếp tục → Nhập số tiền muốn thanh toán. Trường hợp muốn thanh toán toàn bộ, tick vào checkbox Thanh toán toàn bộ giá trị đơn hàng.<br><br>3. <strong>Khách hàng thanh toán lần 3 → Hệ thống hiển thị cho phép:</strong> Khách hàng đến SAPP thanh toán số tiền còn lại (Quy trình vận hành của TVTS như hiện tại)</p> |
{% endstep %}

{% step %}
## Chọn **Next** để kiểm tra thông tin đơn hàng

![](<.gitbook/assets/image (914)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin trước khi hoàn tất khởi tạo

User kiểm tra thông tin đơn hàng trước khi Confirm khởi tạo, bao gồm:

* Thông tin thanh toán;
* Thông tin sản phẩm;
* Thông tin đơn hàng.

![](<.gitbook/assets/image (915)>)
{% endstep %}

{% step %}
## Xác nhận đồng bộ thông tin đơn hàng lên HubSpot và Hoàn tất

Sau khi kiểm tra thông tin đơn hàng, nếu:

* Nếu thông tin cần chỉnh sửa, quay lại Tab 1: Create Order để chỉnh sửa;
* Nếu thông tin đã chính xác, user chọn **Finish >** Chọn **Confirm** trên pop-up xác nhậnĐồng bộ thông tin đơn hàng về HubSpot

![](<.gitbook/assets/image (916)>)

![](<.gitbook/assets/image (917)>)

* Sau khi hoàn tất, hệ thống tạo bản ghi mới trên màn hình lưới với **Order status = Chờ thanh toán**
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin đơn hàng

{% hint style="info" %}
User chỉ có thể chỉnh sửa thông tin đơn hàng trong trường hợp **Order status = Chờ thanh toán**. → Tương ứng với Deal, user chỉ có thể cập nhật thông tin Order & đồng bộ lên Hubspot khi Deal chưa được chuyển sang bước Soạn thảo hợp đồng.
{% endhint %}

{% stepper %}
{% step %}
## Tại đơn hàng cần chỉnh sửa > Chọn ⁝ > Chọn **Edit**

![](<.gitbook/assets/image (918)>)
{% endstep %}

{% step %}
## Cập nhật Customer Info: Cập nhật **Deal ID** > Chọn **Đồng bộ thông tin**

* User nhập Deal ID của deal tương ứng trên HubSpot.
* Hệ thống tự động đồng bộ thông tin khách hàng từ HubSpot như dưới đây:

| Trường thông tin được đồng bộ | Ý nghĩa                                                            | Property đồng bộ                                        |
| ----------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------- |
| Full name                     | Tên đầy đủ của khách hàng.                                         | Đồng bộ từ Contact property: \[TVTS] Họ tên             |
| Email                         | Email của khách hàng                                               | Đồng bộ từ Contact property: Email                      |
| Phone                         | Số điện thoại của khách hàng                                       | Đồng bộ từ Contact property: \[TVTS] Phone number       |
| Tỉnh/Thành phố                | Khu vực sinh sống của khách hàng                                   | Đồng bộ từ Contact property: \[TVTS] Khu vực sinh sống  |
| Địa chỉ                       | Địa chỉ của khách hàng                                             | Đồng bộ từ Contact property: \[TVTS] Địa chỉ            |
| Deal ID đã thanh toán học phí | Deal của khách hàng đã bị đánh lost trước đó (do có lỗi phát sinh) | Đồng bộ từ Deal property: Deal ID đã thanh toán học phí |

![](<.gitbook/assets/image (919)>)
{% endstep %}

{% step %}
## Cập nhật Product Info (nếu có)

| Nhu cầu                             | Thao tác                                                                                                                                                                                                                                                       |
| ----------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Xóa sản phẩm                        | Chọn **Delete Product** tại sản phẩm cần xóa                                                                                                                                                                                                                   |
| Thêm sản phẩm                       | <p>1. Chọn <strong>Add Product</strong><br>2. Chọn vào vùng trống của trường <strong>Product</strong> để mở màn hình danh sách sản phẩm.<br>3. Sau đó chọn checkbox tại các sản phẩm cần thêm và chọn <strong>Add</strong> để lưu</p>                          |
| Xóa nhóm sản phẩm                   | Chọn **Delete Combo** tại sản phẩm cần xóa                                                                                                                                                                                                                     |
| Thêm nhóm sản phẩm                  | <p>1. Chọn <strong>Add</strong> <strong>Combo</strong><br>2. Chọn vào vùng trống của trường <strong>Combo</strong> để mở màn hình danh sách sản phẩm.<br>3. Sau đó chọn checkbox tại các nhóm sản phẩm cần thêm và chọn <strong>Add</strong> để lưu</p>        |
| Xóa Discount code                   | Chọn **X** tại mã khuyến mại cần xóa                                                                                                                                                                                                                           |
| Thêm Discount code                  | <p>1. Chọn vào vùng trống của trường <strong>Discount code</strong> để mở màn hình danh sách mã khuyến mại áp dụng cho product/combo đó<br>2. Sau đó chọn checkbox tại các mã khuyến mại cần thêm và chọn <strong>Add</strong> để lưu</p>                      |
| Xóa Custom Discount                 | Bỏ chọn checkbox **Apply a custom product / combo discount**                                                                                                                                                                                                   |
| Thêm hoặc Chỉnh lại Custom Discount | <p>1. Chọn checkbox <strong>Apply a custom product/combo discount</strong> (nếu cần)<br>2. Chọn hoặc cập nhật <strong>Type of Custom Discount</strong> > Nhập hoặc cập nhật <strong>Discount Rate</strong> hoặc <strong>Custom Discount</strong> tương ứng</p> |
{% endstep %}

{% step %}
## Cập nhật **Discount code for Entire Order** **(nếu có)**

User có thể Thêm hoặc Xóa mã khuyến mại được áp dụng cho đơn hàng như sau:

| Nhu cầu            | Thao tác                                                                                                                                                                                                                                      |
| ------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Xóa Discount code  | Chọn **X** tại mã khuyến mại cần xóa                                                                                                                                                                                                          |
| Thêm Discount code | <p>- Chọn vào vùng trống của trường <strong>Discount code for Entire Order</strong> để mở màn hình danh sách mã khuyến mại áp dụng cho order<br>- Sau đó chọn checkbox tại các mã khuyến mại cần thêm và chọn <strong>Add</strong> để lưu</p> |

Cho phép tìm kiếm nhanh theo các điều kiện dưới đây:

* Name: Tên của mã khuyến mại
* Category:
* Sort by (A-Z, Z-A, Latest, Oldest)
* From date - To date: Thời gian hiệu lực của promotion code
{% endstep %}

{% step %}
## Cập nhật **Add-on Course** **(nếu có)**

User có thể Thêm hoặc Xóa gói khóa học tặng kèm trên đơn hàng như sau:

| Nhu cầu            | Thao tác                                                                                                                                                   |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Xóa Add-on Course  | Chọn **X** tại gói khóa học tặng kèm cần xóa                                                                                                               |
| Thêm Add-on Course | <p>- Chọn vào vùng trống của trường <strong>Add-on course</strong> để hiện danh sách các khóa học được tặng kèm<br>- Sau đó chọn gói khóa học cần thêm</p> |
{% endstep %}

{% step %}
## Cập nhật **Payment Info** **(nếu có)**

Trong trường hợp khách hàng thay đổi và muốn thanh toán nhiều lần qua VNPay, user thực hiện tick vào checkbox **Allow customer to split payment via VNPay**

![](<.gitbook/assets/image (920)>)
{% endstep %}

{% step %}
## Chọn **Next** để kiểm tra thông tin đơn hàng

![](<.gitbook/assets/image (921)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin trước khi hoàn tất cập nhật

User kiểm tra thông tin đơn hàng trước khi Confirm cập nhật, bao gồm:

* Thông tin thanh toán;
* Thông tin sản phẩm;
* Thông tin đơn hàng.

![](<.gitbook/assets/image (922)>)
{% endstep %}

{% step %}
## Xác nhận đồng bộ thông tin đơn hàng lên HubSpot và Hoàn tất

Sau khi kiểm tra thông tin đơn hàng, nếu:

* Nếu thông tin cần chỉnh sửa, quay lại Tab 1: Create Order để chỉnh sửa;
* Nếu thông tin đã chính xác, user chọn **Finish >** Chọn **Confirm** trên pop-up xác nhậnĐồng bộ thông tin đơn hàng về HubSpot

![](<.gitbook/assets/image (923)>)

![](<.gitbook/assets/image (924)>)
{% endstep %}
{% endstepper %}

### Gia hạn đơn hàng

#### Lưu ý về thời gian hiệu lực của đơn hàng

* Đơn hàng có thời gian hiệu lực trong _**30 ngày**_.
* Sau đó, với các đơn hàng có trạng thái = Chờ thanh toán, Đã thanh toán một phần → Trạng thái của đơn hàng được cập nhật = Hết hạn

→ Vì vậy, sau 30 ngày, nếu khách hàng chưa hoàn tất thanh toán nhưng đơn hàng đã hết hạn, user cần thực hiện gia hạn đơn hàng trên Ops.

{% stepper %}
{% step %}
## Tại đơn hàng cần gia hạn: Chọn ⁝ > Chọn **Gia hạn**

![](<.gitbook/assets/image (925)>)
{% endstep %}

{% step %}
## Chọn **Yes** trên pop-up Xác nhận gia hạn và Hoàn tất

Sau khi xác nhận gia hạn, đơn hàng sẽ được gia hạn thêm 30 ngày và được cập nhật về trạng thái cũ trước khi hết hạn.

Ví dụ: Order status = Đã thanh toán một phần ⇒ Hết hạn sau 30 ngày chưa hoàn tất thanh toán. Sau khi được gia hạn, order status = Đã thanh toán một phần

![](<.gitbook/assets/image (926)>)
{% endstep %}
{% endstepper %}

### Hủy đơn hàng

{% stepper %}
{% step %}
## Tại đơn hàng cần xóa, chọn nút Action ⁝ > Chọn **Cancel**

![](<.gitbook/assets/image (927)>)
{% endstep %}

{% step %}
## Chọn **Yes** trên pop-up Xác nhận hủy đơn hàng và Hoàn tất

Đơn hàng được cập nhật Order status = _**Đã hủy**_ & khách hàng không thể thanh toán cho đơn hàng nữa.

![](<.gitbook/assets/image (928)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. **Deal ID là bắt buộc và phải hợp lệ** — hệ thống chỉ tạo order khi Deal ID tồn tại trên HubSpot. Không thể nhập tay thông tin học viên; toàn bộ thông tin được đồng bộ tự động từ HubSpot sau khi xác nhận Deal ID.
2. **Chỉnh sửa Order chỉ khả dụng khi Order status = Chờ thanh toán** — sau khi order chuyển sang Đã thanh toán hoặc Hủy, không thể sửa bất kỳ thông tin nào.
3. **Hủy Order là thao tác không thể hoàn tác** — hệ thống yêu cầu xác nhận qua pop-up trước khi thực hiện. Kiểm tra kỹ trước khi nhấn xác nhận.

### Quy tắc nghiệp vụ

1. **Luồng trạng thái Order:** Chờ thanh toán → Đang thanh toán → Đã thanh toán một phần hoặc Đã thanh toán.
2. **Thông tin học viên trên Order phản ánh dữ liệu tại thời điểm đồng bộ** — nếu thông tin trên HubSpot thay đổi sau khi tạo Order, cần chỉnh sửa lại đơn hàng.
3. **Mỗi Deal ID chỉ tương ứng với một Order đang hoạt động** — kiểm tra kỹ trước khi tạo mới để tránh trùng lặp.

### Mẹo sử dụng

1. Trước khi tạo Order, kiểm tra Deal ID trên HubSpot để đảm bảo thông tin học viên (họ tên, số điện thoại, địa chỉ) đã đầy đủ và chính xác — việc này giúp tránh phải quay lại sửa sau khi đồng bộ.
2. Dùng bộ lọc **Status** kết hợp **Sort by** để nhanh chóng tìm các đơn hàng cần xử lý.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                             | Nguyên nhân                                                    | Cách xử lý                                                                                  |
| ------------------------------------------------------------ | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------- |
| _"Deal ID không tồn tại"_                                    | Deal ID nhập sai hoặc chưa được tạo trên HubSpot               | Kiểm tra lại Deal ID trên HubSpot; đảm bảo deal đã được khởi tạo trước khi tạo Order        |
| Thông tin học viên đồng bộ về sai (sai tên, SĐT, địa chỉ...) | Dữ liệu trên HubSpot (Deal/Contact) đang sai                   | Cập nhật lại thông tin trên HubSpot → quay lại Create Order, nhập lại Deal ID → đồng bộ lại |
| Không thấy nút **Chỉnh sửa** (Edit)                          | Order status không phải _Chờ thanh toán_                       | Kiểm tra trạng thái order; nếu cần sửa order đã thanh toán/hủy, liên hệ Admin               |
| Không thể thêm sản phẩm / mã khuyến mãi khi tạo Order        | Sản phẩm chưa được cấu hình hoặc promotion code không hợp lệ   | Kiểm tra lại danh sách Product & Combo; xác nhận mã promotion code còn hiệu lực             |
| Đồng bộ thông tin về HubSpot thất bại                        | Lỗi kết nối tạm thời hoặc dữ liệu Order có trường không hợp lệ | Thử lại thao tác đồng bộ; nếu vẫn lỗi, liên hệ Admin kiểm tra cấu hình tích hợp HubSpot     |
| Order bị Hủy nhầm                                            | Nhấn xác nhận hủy không đúng                                   | Tạo lại Deal và Order mới                                                                   |
| Không tìm thấy Order cần xử lý                               | Dùng sai bộ lọc hoặc Order thuộc Deal ID khác                  | Dùng ô tìm kiếm theo **Mã đơn hàng** hoặc **Deal ID**; kiểm tra lại bộ lọc Status           |
