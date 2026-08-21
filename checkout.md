# Checkout

Kết quả đạt được: Khách hàng có thể lựa chọn hình thức – phương thức thanh toán phù hợp để thực hiện thanh toán học phí.

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| June 18, 2026  | Nhungnth      | A     | Create New         | 1.0.0   |

## I. Thông tin chung

**Dành cho:** Học viên / Khách hàng

**Kích hoạt:** Nhấn vào đường link thanh toán được gửi qua email

#### Phạm vi & Module liên quan

* **Module chính:** [Order List](payment/order-list.md)
* **Module liên quan:** [Product](payment/product.md), [Combo](payment/combo.md), [Promotion Mode](payment/promotion-code.md)
* **Hệ thống tích hợp:** HubSpot, VNPay, VietQR

#### Điều kiện tiên quyết:

1. Đơn hàng đã được khởi tạo trên hệ thống;
2. Học viên đã nhận được email chứa đường link thanh toán do SAPP gửi. Đơn hàng đã được khởi tạo trên hệ thống.

## II. Hướng dẫn chi tiết

> Checkout cho phép học viên/khách hàng kiểm tra thông tin đơn hàng và thực hiện thanh toán học phí trực tuyến.

{% stepper %}
{% step %}
## Truy cập đường link thanh toán qua email → Hệ thống hiển thị màn hình Xác nhận thông tin

![](<.gitbook/assets/image (929)>)

Màn hình hiển thị đầy đủ thông tin đơn hàng ở chế độ read-only, bao gồm:

### 1.1. Thông tin học viên

| Trường             | Mô tả                          |
| ------------------ | ------------------------------ |
| **Full name**      | Họ tên đầy đủ của học viên     |
| **Phone**          | Số điện thoại của học viên     |
| **Email**          | Địa chỉ email của học viên     |
| **Tỉnh/Thành phố** | Khu vực sinh sống của học viên |
| **Địa chỉ**        | Địa chỉ của học viên           |
| **Deal ID**        | Mã deal trên hệ thống HubSpot  |

### 1.2. Thông tin sản phẩm

> Hiển thị danh sách sản phẩm trong đơn hàng gồm: Tên sản phẩm, Discount code, Số lượng.

### 1.3. Thông tin đơn hàng

| Trường            | Mô tả                                   |
| ----------------- | --------------------------------------- |
| **Giá**           | Tổng giá trị đơn hàng trước ưu đãi      |
| **Khuyến mãi**    | Tổng số tiền được ưu đãi                |
| **Đã thanh toán** | Số tiền đã thanh toán trước đó (nếu có) |
| **Còn lại**       | Số tiền còn phải thanh toán             |

Mục **Giá trị đã thanh toán** chỉ hiển thị khi học viên đã có lần thanh toán trước đó (Đã thanh toán > 0).
{% endstep %}

{% step %}
## Lựa chọn Hình thức thanh toán và Phương thức thanh toán

![](<.gitbook/assets/image (930)>)

User thực hiện lựa chọn hình thức và phương thức thanh toán tương ứng như sau:

| Hình thức     | Phương thức có thể chọn                                                               |
| ------------- | ------------------------------------------------------------------------------------- |
| **Trả thẳng** | <p>- Chuyển khoản<br>- Thanh toán qua thẻ (qua VNPay)<br>- Quẹt POS<br>- Tiền mặt</p> |
| **Trả góp**   | <p>- VNPay<br>- Quẹt POS</p>                                                          |

{% hint style="warning" %}
#### Lưu ý lựa chọn Hình thức thanh toán

Hình thức thanh toán chỉ được chọn **một lần duy nhất** ở lần thanh toán đầu tiên và không thể thay đổi ở các lần sau.
{% endhint %}
{% endstep %}

{% step %}
## Nhấn "Tiến hành thanh toán" để thực hiện thanh toán

![](<.gitbook/assets/image (931)>)

Dựa trên hình thức – phương thức thanh toán user đã chọn → Hệ thống hiển thị thông tin thanh toán tương ứng.

### 3.1. Đối với Hình thức thanh toán = Trả thẳng

#### Chuyển khoản

Hệ thống hiển thị **mã VietQR** để học viên chuyển khoản.

![](<.gitbook/assets/image (932)>)

Khách hàng có thể thực hiện thanh toán theo 1 trong 2 cách sau:

* **Cách 1**: Quét trực tiếp mã QR hiển thị để thực hiện thanh toán
* **Cách 2**: Copy thông tin thanh toán để thực hiện thanh toán

#### Thanh toán qua thẻ

{% stepper %}
{% step %}
## Lựa chọn Loại thẻ thanh toán → chọn Tiếp theo

User lựa chọn loại thẻ phù hợp để tiến hành thanh toán học phí, bao gồm:

* Thẻ nội địa & tài khoản ngân hàng
* Thẻ thanh toán quốc tế

![](<.gitbook/assets/image (933)>)
{% endstep %}

{% step %}
## Nhập số tiền thanh toán lần này → chọn Tiếp tục

* Khách hàng có thể nhập số tiền muốn thanh toán cho lần hiện tại box như dưới đây:

![](<.gitbook/assets/image (934)>)

* Trường hợp khách hàng muốn thanh toán toàn bộ giá trị đơn hàng, chọn checkbox **Thanh toán tổng giá trị đơn hàng**.

![](<.gitbook/assets/image (935)>)

→ Hệ thống tự động xác định số tiền còn phải thanh toán.

**Lưu ý đối với số tiền thanh toán theo từng lần thanh toán**

1. Trường hợp khách hàng thanh toán lần đầu hoặc lần 2: Khách hàng có thể nhập số tiền thanh toán hoặc lựa chọn Thanh toán tổng giá trị đơn hàng.
2. Trường hợp khách hàng thanh toán lần cuối (lần 3): Khách hàng thanh toán chính xác số tiền còn phải thanh toán.
{% endstep %}

{% step %}
## Nhập thông tin thẻ thanh toán

Đối với từng loại thẻ, khách hàng nhập các thông tin theo yêu cầu. Cụ thể:

| Loại thẻ               | Thông tin cần nhập                                                                                                                                                                                                                                                            |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Thẻ nội địa            | <p>1. Số thẻ<br>2. Tên chủ thẻ<br>3. Ngày phát hành<br>4. Mã khuyến mại (nếu có)</p>                                                                                                                                                                                          |
| Thẻ thanh toán quốc tế | <p>1. Số thẻ<br>2. Ngày hết hạn: được in trên mặt trước của thẻ (ví dụ: 12/25)<br>3. CVC/CVV: mã xác thực gồm 3 chữ số được in trên mặt sau của thẻ<br>4. Họ và tên khách hàng<br>5. Email<br>6. Quốc gia<br>7. Tỉnh/Thành phố<br>8. Địa chỉ<br>9. Mã khuyến mại (nếu có)</p> |

![](<.gitbook/assets/image (936)>)

![](<.gitbook/assets/image (937)>)

Trường hợp khách hàng muốn dừng quá trình thanh toán, vui lòng chọn **Hủy thanh toán**.
{% endstep %}

{% step %}
## Xác nhận điều khoản sử dụng > Chọn Đồng ý & Tiếp tục

![](<.gitbook/assets/image (938)>)
{% endstep %}

{% step %}
## Nhập mã xác thực OTP > Chọn Thanh toán (nếu có)

Khách hàng thực hiện nhập mã OTP được gửi về số điện thoại đăng ký.

Sau đó, chọn Thanh toán để hoàn tất thực hiện thanh toán.
{% endstep %}
{% endstepper %}

#### Quẹt POS hoặc Tiền mặt

Hệ thống hiển thị thông báo hướng dẫn học viên **đến văn phòng SAPP** dưới đây để thực hiện thanh toán trực tiếp:

* Văn phòng Hà Nội: Số 54, Phố Lê Thanh Nghị, Phường Bạch Mai, Thành phố Hà Nội
* Văn phòng Hồ Chí Minh: Tầng 1, Số 2A, Đường Lương Hữu Khánh, Phường Bến Thành, Thành phố Hồ Chí Minh

![](<.gitbook/assets/image (939)>)

### 3.2. Đối với Hình thức thanh toán = Trả góp (còn VNPay)

#### VNPay

{% stepper %}
{% step %}
## Chọn ngân hàng trả góp

![](<.gitbook/assets/image (940)>)
{% endstep %}

{% step %}
## Chọn loại thẻ trả góp tương ứng của ngân hàng đã chọn

![](<.gitbook/assets/image (941)>)
{% endstep %}

{% step %}
## Chọn Số tháng trả góp

Khách hàng lựa chọn số tháng trả góp phù hợp với 3 tháng, 6 tháng, 9 tháng hoặc 12 tháng.

![](<.gitbook/assets/image (942)>)
{% endstep %}

{% step %}
## Xác nhận điều khoản > chọn Tiếp tục

Khách hàng xác nhận điều khoản qua checkbox _**"Tôi đồng ý với điều khoản của VNPay"**_.

![](<.gitbook/assets/image (943)>)

Khách hàng chọn **Hủy thanh toán** để tạm dừng quá trình thanh toán.
{% endstep %}

{% step %}
## Nhập thông tin thẻ trả góp > Chọn Tiếp tục

Khách hàng thực hiện nhập các thông tin dưới đây:

* Số thẻ
* Ngày hết hạn
* CVC/CVV
* Số CMND/CCCD/HC (theo chủ thẻ)

![](<.gitbook/assets/image (944)>)

![](<.gitbook/assets/image (945)>)
{% endstep %}

{% step %}
## Chọn Đồng ý & Tiếp tục để xác nhận điều khoản sử dụng & hoàn tất

Sau khi xác nhận, một số thẻ yêu cầu nhập Purchase Authentication được gửi qua Số điện thoại của chủ thẻ.

⇒ Khách hàng nhập code và chọn **Submit** để hoàn tất thanh toán

![](<.gitbook/assets/image (946)>)

![](<.gitbook/assets/image (947)>)
{% endstep %}
{% endstepper %}

#### Quẹt POS hoặc Tiền mặt

Hệ thống hiển thị thông báo hướng dẫn học viên **đến văn phòng SAPP** dưới đây để thực hiện thanh toán trực tiếp:

* Văn phòng Hà Nội: Số 54, Phố Lê Thanh Nghị, Phường Bạch Mai, Thành phố Hà Nội
* Văn phòng Hồ Chí Minh: Tầng 1, Số 2A, Đường Lương Hữu Khánh, Phường Bến Thành, Thành phố Hồ Chí Minh

![](<.gitbook/assets/image (939)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. **Hình thức thanh toán** (Trả thẳng / Trả góp) chỉ chọn được ở lần thanh toán đầu tiên — không thể thay đổi ở lần sau
2. Tài khoản VietQR để chuyển khoản được xác định **tự động** theo danh mục sản phẩm trong đơn hàng
3. Nếu nhấn **Confirm** khi hủy thanh toán, hệ thống ghi nhận trạng thái **Thất bại** — học viên cần liên hệ SAPP để tiếp tục

### Mẹo sử dụng

1. Kiểm tra kỹ thông tin cá nhân và sản phẩm trước khi nhấn "Tiến hành thanh toán"
2. Với phương thức Chuyển khoản, quét mã QR trực tiếp trên màn hình để tránh nhập sai số tài khoản
3. Nếu thanh toán thất bại, kiểm tra email xác nhận — nếu không có email, liên hệ SAPP để xác minh giao dịch

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                  | Nguyên nhân                                           | Cách xử lý                                                    |
| ------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------- |
| Link thanh toán không mở được                     | Link hết hạn hoặc đã được sử dụng                     | Liên hệ SAPP để được cấp lại link                             |
| **"Thanh toán đơn hàng thất bại"**                | Giao dịch không thành công hoặc học viên xác nhận hủy | Thử lại hoặc liên hệ SAPP để được hỗ trợ                      |
| Thông tin học viên hiển thị sai                   | Dữ liệu đồng bộ từ HubSpot chưa được cập nhật         | Liên hệ SAPP để kiểm tra và cập nhật thông tin trên Deal      |
| Không nhận được email xác nhận sau khi thanh toán | Thanh toán chưa được ghi nhận hoặc email vào spam     | Kiểm tra thư mục spam; nếu không có liên hệ SAPP              |
| Mã QR không quét được                             | Chất lượng màn hình hoặc ứng dụng ngân hàng           | Chụp ảnh màn hình rồi quét từ ảnh, hoặc nhập tay số tài khoản |
