---
hidden: true
---

# Tạo mới mã khuyến mại

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| 15/08/2025     | Nhungdh       | A     | Create new         | 3.0.0   |

## Definitions and Acronyms

| #  | Term                      | Definition                                                               |
| -- | ------------------------- | ------------------------------------------------------------------------ |
| 1  | Ops                       | Operations                                                               |
| 2  | Promotion Codes           | Mã khuyến mại dùng để giảm giá cho sản phẩm, nhóm sản phẩm hoặc đơn hàng |
| 3  | Products                  | Sản phẩm đơn lẻ thuộc module Certificate Payments                        |
| 4  | Combo Products            | Nhóm sản phẩm gồm một hoặc nhiều sản phẩm đơn lẻ được kết hợp với nhau   |
| 5  | Apply for Product + Combo | Loại mã khuyến mại áp dụng theo sản phẩm hoặc nhóm sản phẩm              |
| 6  | Apply for Order           | Loại mã khuyến mại áp dụng theo đơn hàng                                 |
| 7  | Quantity                  | Số lượng mã khuyến mại                                                   |
| 8  | Discount                  | Lượng giảm giá của mã khuyến mại                                         |
| 9  | Fixed                     | Giảm giá theo số tiền cụ thể                                             |
| 10 | Percentage                | Giảm giá theo phần trăm giá trị đơn hàng                                 |
| 11 | Combined With             | Các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo           |

## I. Giới Thiệu Chung

### **1.1 Mục đích**

Tài liệu này hướng dẫn người dùng cách tạo mới mã khuyến mại trong tính năng **Promotion Codes** thuộc module **Payments** trên hệ thống **Operations**.

Mã khuyến mại có thể được tạo để áp dụng theo sản phẩm, nhóm sản phẩm hoặc theo toàn bộ đơn hàng, tùy theo loại mã được người dùng lựa chọn khi tạo mới.

### **1.2 Đối tượng áp dụng**

| Đối tượng               | Vai trò                                                           | Quyền hạn                             |
| ----------------------- | ----------------------------------------------------------------- | ------------------------------------- |
| Người vận hành hệ thống | Tạo và quản lý mã khuyến mại phục vụ thanh toán chứng chỉ Quốc tế | Có quyền xem và tạo mới mã khuyến mại |

### **1.3 Phạm vi & Module liên quan**

* **Tính năng chính:** Promotion Codes
* **Tính năng liên quan:** Products, Combo Products, List of Orders

### **1.4 Điều kiện tiên quyết**

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Người dùng có quyền tạo mới mã khuyến mại.
* Người dùng đang ở màn hình danh sách mã khuyến mại **Promotion Codes**.
* Với mã khuyến mại áp dụng theo sản phẩm hoặc nhóm sản phẩm, sản phẩm hoặc nhóm sản phẩm cần áp dụng mã đã được tạo trên hệ thống.

***

## II. Tổng Quan Giao Diện

Màn hình tạo mới mã khuyến mại cho phép người dùng nhập thông tin mã giảm giá, chọn loại áp dụng, cài đặt số lượng, thời gian hiệu lực, lượng giảm giá và phạm vi áp dụng.

Mã khuyến mại được chia làm 2 loại:

| Loại mã khuyến mại        | Ý nghĩa                                                     |
| ------------------------- | ----------------------------------------------------------- |
| Apply for Product + Combo | Mã khuyến mại áp dụng theo từng sản phẩm hoặc nhóm sản phẩm |
| Apply for Order           | Mã khuyến mại áp dụng theo từng đơn hàng                    |

Các thành phần chính trên màn hình gồm:

| Thành phần           | Mô tả                                                          |
| -------------------- | -------------------------------------------------------------- |
| Code                 | Tên mã khuyến mại                                              |
| Apply option         | Loại áp dụng của mã khuyến mại                                 |
| Quantity             | Số lượng mã khuyến mại                                         |
| No quantity required | Cho phép không giới hạn số lượng mã khuyến mại được sử dụng    |
| Start - End          | Thời gian hiệu lực của mã khuyến mại                           |
| Apply for Product    | Danh sách sản phẩm được áp dụng mã khuyến mại                  |
| Apply for Combo      | Danh sách nhóm sản phẩm được áp dụng mã khuyến mại             |
| Discount             | Lượng giảm giá của mã khuyến mại                               |
| Combined with        | Các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo |
| Save                 | Nút lưu thông tin mã khuyến mại                                |

<figure><img src="../../.gitbook/assets/image (363).png" alt=""><figcaption></figcaption></figure>

***

## III. Các Bước Thực Hiện Chi Tiết

### **3.1 Tạo mới mã khuyến mại áp dụng theo sản phẩm hoặc nhóm sản phẩm**

> 🎯 Mục tiêu: Tạo mới mã khuyến mại áp dụng cho một hoặc nhiều sản phẩm, nhóm sản phẩm cụ thể.

**Bước 1:** Truy cập màn hình tạo mới mã khuyến mại

Tại màn hình danh sách mã khuyến mại **Promotion Codes**, chọn **New Promotion Code**.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình tạo mới mã khuyến mại.
* Người dùng có thể bắt đầu nhập thông tin mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (365).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Chọn loại mã khuyến mại

Tại trường **Apply option**, chọn **Apply for Product + Combo**.

Kết quả mong đợi:

* Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng theo sản phẩm hoặc nhóm sản phẩm.
* Người dùng có thể chọn sản phẩm hoặc nhóm sản phẩm được áp dụng mã.

<figure><img src="../../.gitbook/assets/image (366).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Nhập thông tin chung của mã khuyến mại

Người dùng nhập các thông tin sau:

| Trường thông tin     | Bắt buộc | Hướng dẫn nhập                                                                |
| -------------------- | -------- | ----------------------------------------------------------------------------- |
| Code                 | Có       | Nhập tên mã khuyến mại                                                        |
| Quantity             | Có       | Nhập số lượng mã khuyến mại                                                   |
| No quantity required | Không    | Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng |
| Start - End          | Không    | Chọn thời gian hiệu lực của mã khuyến mại                                     |
| Discount             | Có       | Nhập lượng giảm giá của mã khuyến mại                                         |
| Combined with        | Không    | Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo           |

Lưu ý:

* Nếu chọn **No quantity required**, người dùng không cần điền thông tin tại trường **Quantity**.
* Các trường được đánh dấu bắt buộc không được để trống.

<figure><img src="../../.gitbook/assets/image (367).png" alt=""><figcaption></figcaption></figure>

**Bước 4:** Chọn sản phẩm được áp dụng mã khuyến mại

Tại trường **Apply for Product**, chọn để mở danh sách sản phẩm.

Trên màn hình danh sách sản phẩm, người dùng thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách sản phẩm đã chọn.

Kết quả mong đợi:

* Các sản phẩm được chọn hiển thị tại trường **Apply for Product**.
* Mã khuyến mại sẽ được áp dụng cho các sản phẩm đã chọn sau khi mã được lưu thành công.

<figure><img src="../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (368).png" alt=""><figcaption></figcaption></figure>

**Bước 5:** Chọn nhóm sản phẩm được áp dụng mã khuyến mại

Tại trường **Apply for Combo**, chọn để mở danh sách nhóm sản phẩm.

Trên màn hình danh sách nhóm sản phẩm, người dùng thực hiện:

* Chọn hoặc bỏ chọn checkbox tại các nhóm sản phẩm cần áp dụng mã khuyến mại.
* Chọn **Select** để lưu danh sách nhóm sản phẩm đã chọn.

Kết quả mong đợi:

* Các nhóm sản phẩm được chọn hiển thị tại trường **Apply for Combo**.
* Mã khuyến mại sẽ được áp dụng cho các nhóm sản phẩm đã chọn sau khi mã được lưu thành công.

<figure><img src="../../.gitbook/assets/image (370).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (371).png" alt=""><figcaption></figcaption></figure>

**Bước 6:** Chọn loại giảm giá và nhập lượng giảm giá

Tại trường **Discount**, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |

Kết quả mong đợi:

* Hệ thống ghi nhận loại giảm giá và giá trị giảm giá của mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (372).png" alt=""><figcaption></figcaption></figure>

**Bước 7:** Lưu mã khuyến mại

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

Kết quả mong đợi:

* Hệ thống lưu thông tin mã khuyến mại mới.
* Mã khuyến mại vừa tạo hiển thị ở đầu danh sách mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>

### **3.2 Tạo mới mã khuyến mại áp dụng theo đơn hàng**

> 🎯 Mục tiêu: Tạo mới mã khuyến mại áp dụng theo từng đơn hàng.

**Bước 1:** Truy cập màn hình tạo mới mã khuyến mại

Tại màn hình danh sách mã khuyến mại **Promotion Codes**, chọn **New Promotion Code**.

Kết quả mong đợi:

* Hệ thống chuyển đến màn hình tạo mới mã khuyến mại.
* Người dùng có thể bắt đầu nhập thông tin mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (374).png" alt=""><figcaption></figcaption></figure>

**Bước 2:** Chọn loại mã khuyến mại

Tại trường **Apply option**, chọn **Apply for Order**.

Kết quả mong đợi:

* Hệ thống ghi nhận loại mã khuyến mại là mã áp dụng theo đơn hàng.
* Người dùng không cần chọn **Apply for Product** hoặc **Apply for Combo**.

<figure><img src="../../.gitbook/assets/image (375).png" alt=""><figcaption></figcaption></figure>

**Bước 3:** Nhập thông tin mã khuyến mại

Người dùng nhập các thông tin sau:

| Trường thông tin     | Bắt buộc | Hướng dẫn nhập                                                                |
| -------------------- | -------- | ----------------------------------------------------------------------------- |
| Code                 | Có       | Nhập tên mã khuyến mại                                                        |
| Quantity             | Có       | Nhập số lượng mã khuyến mại                                                   |
| No quantity required | Không    | Chọn checkbox này nếu không muốn giới hạn số lượng mã khuyến mại được sử dụng |
| Start - End          | Không    | Chọn thời gian hiệu lực của mã khuyến mại                                     |
| Discount             | Có       | Nhập lượng giảm giá của mã khuyến mại                                         |
| Combined with        | Không    | Chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo           |

Lưu ý:

* Nếu chọn **No quantity required**, người dùng không cần điền thông tin tại trường **Quantity**.
* Các trường được đánh dấu bắt buộc không được để trống.

<figure><img src="../../.gitbook/assets/image (376).png" alt=""><figcaption></figcaption></figure>

**Bước 4:** Chọn loại giảm giá và nhập lượng giảm giá

Tại trường **Discount**, người dùng chọn loại giảm giá và nhập giá trị giảm giá.

| Loại giảm giá | Ý nghĩa                                  |
| ------------- | ---------------------------------------- |
| Fixed         | Giảm giá theo số tiền cụ thể, đơn vị VND |
| Percentage    | Giảm giá theo phần trăm giá trị đơn hàng |

Kết quả mong đợi:

* Hệ thống ghi nhận loại giảm giá và giá trị giảm giá của mã khuyến mại.

**Bước 5:** Lưu mã khuyến mại

Sau khi nhập đầy đủ thông tin bắt buộc, chọn **Save** để lưu thông tin.

Kết quả mong đợi:

* Hệ thống lưu thông tin mã khuyến mại mới.
* Mã khuyến mại vừa tạo hiển thị ở đầu danh sách mã khuyến mại.

<figure><img src="../../.gitbook/assets/image (377).png" alt=""><figcaption></figcaption></figure>

***

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

* Mã khuyến mại được chia làm 2 loại: **Apply for Product + Combo** và **Apply for Order**.
  * Với **Apply for Product + Combo**, mã khuyến mại áp dụng theo từng sản phẩm hoặc nhóm sản phẩm.
  * Với **Apply for Order**, mã khuyến mại áp dụng theo từng đơn hàng.
* Nếu chọn **No quantity required**, người dùng không cần điền thông tin tại trường **Quantity**.
* **Combined with** dùng để chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo.
* Với **Apply for Product + Combo**, người dùng chỉ cần điền một trong hai thông tin **Apply for Product** hoặc **Apply for Combo**, không bắt buộc phải điền cả hai.

***

## V. Các lỗi thường gặp và cách xử lý

Hiện tài liệu gốc chưa cung cấp thông báo lỗi cụ thể của hệ thống. Có thể bổ sung sau khi có ảnh màn hình hoặc nội dung message thực tế.

| Lỗi / Tình huống       | Nguyên nhân                                              | Cách xử lý                                                                                                                                                |
| ---------------------- | -------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| This field is required | Người dùng chưa nhập đầy đủ thông tin bắt buộc           | Kiểm tra và nhập đầy đủ **Code**, **Apply option**, **Quantity** nếu không chọn **No quantity required**, **Discount** và các trường bắt buộc khác nếu có |
| Code already exist     | Code của mã khuyến mại đang tạo đã tồn tại trên hệ thống | Kiếm tra lại Code của mã khuyến mại, và điền lại sao cho Code của mã khuyến mại là duy nhất trên hệ thống.                                                |

***

## VI. Câu Hỏi Thường Gặp

**Q: Nếu không muốn giới hạn số lượng mã khuyến mại thì làm thế nào?**\
A: Chọn checkbox **No quantity required**. Khi đó, người dùng không cần điền thông tin tại trường **Quantity**.

**Q: Với Apply for Product + Combo, có bắt buộc chọn cả Apply for Product và Apply for Combo không?**\
A: Không. Người dùng chỉ cần điền một trong hai thông tin **Apply for Product** hoặc **Apply for Combo**, không bắt buộc phải điền cả hai.

**Q: Discount có những loại nào?**\
A: **Discount** có thể là **Fixed**, giảm theo số tiền cụ thể, đơn vị VND, hoặc **Percentage**, giảm theo phần trăm giá trị đơn hàng.

**Q: Combined with dùng để làm gì?**\
A: **Combined with** dùng để chọn các mã giảm giá có thể dùng kết hợp với mã khuyến mại đang tạo.
