# Quản lý danh sách giao dịch

Kết quả đạt được: Danh sách các giao dịch được thực hiện trên mỗi đơn hàng, bao gồm Thu học phí và Hoàn học phí.

## Record of changes

A - Add, M - Modify, D - Delete

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| June 18, 2026  | Nhungnth      | A     | Create New         | 1.0.0   |

## I. Thông tin chung

#### Đối tượng sử dụng

1. **Dành cho:** Admin, Kế toán, TVTS
2. **Đường dẫn:** Module **Order & Payment** → **Order List** → Chọn đơn hàng → **View Order Details** → Tab **Transaction List**

#### Phạm vi & Module liên quan

* **Module chính:** [Order List](payment/order-list.md)
* **Module liên quan:**
* **Hệ thống tích hợp:** HubSpot, VietQR, VNPay

#### Điều kiện tiên quyết:

Đã đăng nhập, được cấp quyền truy cập module **Order & Payment** và đơn hàng đã tồn tại trên hệ thống.

## II. Hướng dẫn chi tiết

> Quản lý các giao dịch tài chính phát sinh trên đơn hàng, gồm: **Thu học phí** và **Hoàn học phí**.

### Xem danh sách giao dịch

{% stepper %}
{% step %}
## Truy cập màn hình Order List

Tại thanh menu hệ thống:chọn Order & Payment → Order & Payment → chọn tab Transaction List

![](<.gitbook/assets/image (859)>)

Danh sách hiển thị các cột trên màn hình danh sách như sau:

| Cột                        | Mô tả                                                                                                                                                                                                                      |
| -------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No**                     | Số thứ tự                                                                                                                                                                                                                  |
| **Mã thanh toán**          | Tự động với giao dịch Chuyển khoản / VNPay                                                                                                                                                                                 |
| **Transaction type**       | Hiển thị phân loại giao dịch, bao gồm: - _**Thanh toán học phí**_\*:\* giao dịch đóng tiền được thực hiện bởi học viên/khách hàng **-** \*\*\*Hoàn học phí:\*\*\*giao dịch hoàn tiền được thực hiện bởi phòng TCKT         |
| **Payment Type**           | Hình thức thanh toán của giao dịch, bao gồm: - _Trả thẳng_\* - Trả góp\*                                                                                                                                                   |
| **Payment method**         | Phương thức thanh toán của giao dịch, bao gồm: - Chuyển khoản - Thanh toán qua thẻ (tương ứng khi khách hàng thanh toán qua VNPay) - VNPay - Tiền mặt - Quẹt POS                                                           |
| **Amount**                 | Số tiền thanh toán trên từng giao dịch thực hiện                                                                                                                                                                           |
| **Recipient Bank Account** | Tài khoản nhận tiền khi Payment Method = Chuyển khoản                                                                                                                                                                      |
| **Tuition Payment Office** | Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm: - NEU - UEH                                                                                                                                                      |
| **Remitting Bank Account** | <p>Tài khoản thực hiện hoàn học phí, bao gồm:<br><br>- MB SAPP<br>- MB SAA<br>- MB SCFA<br>- MB SCMA</p>                                                                                                                   |
| **Paid Date**              | Ngày thanh toán                                                                                                                                                                                                            |
| **Status**                 | Trạng thái của giao dịch, bao gồm: - _Chờ xác nhận_: giao dịch chờ xác nhận bởi TCKT\* - Đã thanh toán\*\*:\* giao dịch đã thực hiện thành công hoặc được xác nhận bởi TCKT\* - Thất bại:\* khách hàng thanh toán thất bại |
{% endstep %}

{% step %}
## User có thể tìm kiếm nhanh theo điều kiện

User có thể tìm kiếm theo các điều kiện dưới đây:

* Search mã thanh toán: Theo mã thanh toán của giao dịch
* Transaction Type: Theo phân loại giao dịch
* Payment Type: Theo hình thức thanh toán
* Payment Method: Theo phương thức thanh toán
* Sort list: Chọn cách sắp xếp danh sách giao dịch (A-Z, Z-A, Latest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

![](<.gitbook/assets/image (860)>)

Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết giao dịch

Áp dụng cho: Thanh toán học phí (Tiền mặt/Quẹt POS) và Hoàn học phí.

{% stepper %}
{% step %}
## Tại bản ghi cần xem thông tin chi tiết > Chọn **⁝** > Chọn **View Detail**

![](<.gitbook/assets/image (861)>)
{% endstep %}

{% step %}
## Hoàn tất

Hệ thống hiển thị màn hình chi tiết giao dịch tương ứng.

![](<.gitbook/assets/image (862)>)
{% endstep %}
{% endstepper %}

### Thêm mới giao dịch

{% stepper %}
{% step %}
## Tại màn hình List Transaction, chọn **"Add Transaction"**

Hệ thống chuyển tới màn hình tạo mới giao dịch

{% hint style="info" %}
#### Lưu ý khởi tạo giao dịch

User chỉ có thể khởi tạo giao dịch trong trường hợp khách hàng thanh toán với phương thức = Tiền mặt hoặc Quẹt POS
{% endhint %}

![](<.gitbook/assets/image (863)>)

![](<.gitbook/assets/image (864)>)
{% endstep %}

{% step %}
## Nhập thông tin giao dịch

![](<.gitbook/assets/image (865)>)

Chi tiết các trường thông tin dưới đây:

| Trường                       | Bắt buộc | Mô tả                                                                                                              |
| ---------------------------- | -------- | ------------------------------------------------------------------------------------------------------------------ |
| **Transaction type**         | Tự động  | Phân loại giao dịch, hiển thị mặc định = Thu học phí                                                               |
| **Payment Type**             | ✅        | Hình thức thanh toán của giao dịch, bao gồm: - _Trả thẳng - Trả góp_                                               |
| **Payment method**           | ✅        | Phương thức thanh toán của giao dịch, bao gồm: - Tiền mặt - Quẹt POS                                               |
| **Tuition Payment Office**   | ✅        | Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm: - NEU - UEH Chỉ hiển thị khi Payment method = Tiền mặt   |
| **Amount**                   | ✅        | Số tiền thanh toán trên từng giao dịch thực hiện                                                                   |
| **Paid Date**                | ✅        | Ngày thanh toán (≤ ngày hiện tại)                                                                                  |
| **Transaction Status**       | Tự động  | Trạng thái của giao dịch — hiển thị mặc định = _**Chờ xác nhận**_                                                  |
| **Upload chứng từ xác minh** | ✅        | Đăng tải chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG — tối đa 20MB/file, nhiều file |

**Logic Payment method:**

* Transaction type = Hoàn học phí → **Chuyển khoản**
* Payment Type = Trả thẳng → Tiền mặt, Quẹt POS
* Payment Type = Trả góp → Quẹt POS
{% endstep %}

{% step %}
## Nhấn **"Chuyển xác nhận"**

Sau khi nhập thông tin, chọn Chuyển xác nhận để lưu giao dịch và chuyển cho TCKT xác nhận. Sau đó, hệ thống thực hiện:

* Gửi thông báo **"Transaction successfully submitted for approval"**
* Tạo bản ghi xuất hiện trên lưới với trạng thái = **Chờ xác nhận**
* Hệ thống tạo task HubSpot (KT04) gửi Kế toán kèm link transaction

![](<.gitbook/assets/image (866)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa giao dịch

{% hint style="info" %}
#### Lưu ý chỉnh sửa giao dịch

Chỉ chỉnh sửa được khi **Transaction Status = Chờ xác nhận**
{% endhint %}

{% stepper %}
{% step %}
## Tại màn hình List Transaction > Chọn giao dịch cần chỉnh sửa > Chọn **⁝** > Chọn **Edit Transaction**

Hệ thống hiển thị màn hình chỉnh sửa thông tin của giao dịch.

![](<.gitbook/assets/image (867)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin giao dịch

Chi tiết các trường thông tin hiển thị được trình bày dưới đây:

| Trường thông tin             | Bắt buộc | Hướng dẫn chỉnh sửa                                                                                                |
| ---------------------------- | -------- | ------------------------------------------------------------------------------------------------------------------ |
| **Transaction type**         | Tự động  | Không được phép chỉnh sửa                                                                                          |
| **Payment Type**             | ✅        | Hình thức thanh toán của giao dịch, bao gồm: - _Trả thẳng - Trả góp_                                               |
| **Payment method**           | ✅        | Phương thức thanh toán của giao dịch, bao gồm: - Tiền mặt - Quẹt POS                                               |
| **Tuition Payment Office**   | ✅        | Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm: - NEU - UEH Chỉ hiển thị khi Payment method = Tiền mặt   |
| **Amount**                   | ✅        | Số tiền thanh toán trên từng giao dịch thực hiện                                                                   |
| **Paid Date**                | ✅        | Ngày thanh toán (≤ ngày hiện tại)                                                                                  |
| **Transaction Status**       | Tự động  | Không được phép chỉnh sửa                                                                                          |
| **Upload chứng từ xác minh** | ✅        | Đăng tải chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG — tối đa 20MB/file, nhiều file |
{% endstep %}

{% step %}
## Chọn **Update** để lưu thông tin đã chỉnh sửa

Hệ thống cập nhật thông tin của bản ghi theo dữ liệu user đã chỉnh sửa

![](<.gitbook/assets/image (868)>)
{% endstep %}
{% endstepper %}

### Xác nhận giao dịch — Thu học phí (dành cho TCKT)

{% stepper %}
{% step %}
## Kế toán truy cập Transaction List qua link trong task HubSpot (KT04)

Sau khi nhận được task kiểm tra thanh toán bằng Tiền mặt hoặc quẹt POS, TCKT thực hiện truy cập link đơn hàng trên task HubSpot (KT04).

→ Hệ thống hiển thị màn hình danh sách giao dịch.

![](<.gitbook/assets/image (869)>)

![](<.gitbook/assets/image (870)>)
{% endstep %}

{% step %}
## Chọn giao dịch cần kiểm tra > Chọn **⁝** > Chọn **Confirm Transaction**

Hệ thống hiển thị màn hình thông tin giao dịch để kiểm tra thông tin và chứng từ đính kèm.

![](<.gitbook/assets/image (871)>)

![](<.gitbook/assets/image (872)>)
{% endstep %}

{% step %}
## Kiểm tra thông tin giao dịch

User thực hiện kiểm tra thông tin giao dịch, chi tiết như sau:

| Trường                     | Mô tả                                                                                                            |
| -------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Transaction type**       | Phân loại giao dịch, hiển thị mặc định = Thu học phí                                                             |
| **Payment Type**           | Hình thức thanh toán của giao dịch, bao gồm: - _Trả thẳng - Trả góp_                                             |
| **Payment method**         | Phương thức thanh toán của giao dịch, bao gồm: - Tiền mặt - Quẹt POS                                             |
| **Tuition Payment Office** | Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm: - NEU - UEH Chỉ hiển thị khi Payment method = Tiền mặt |
| **Amount**                 | Số tiền thanh toán trên từng giao dịch thực hiện                                                                 |
| **Paid Date**              | Ngày thanh toán (≤ ngày hiện tại)                                                                                |
| **Transaction Status**     | Trạng thái của giao dịch — hiển thị mặc định = _**Chờ xác nhận**_                                                |
| **Tệp đính kèm**           | Chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG                                       |
{% endstep %}

{% step %}
## Nhấn **"Confirm"** để xác nhận

![](<.gitbook/assets/image (873)>)

User thực hiện xác nhận thông tin của giao dịch. Sau đó, nếu:

| Confirm                                                                                                                                                                                                                                                                                                       | Cancel                                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------- |
| <p>- Thông báo: <strong>"Transaction confirmed successfully";</strong><br>- Trạng thái chuyển sang <strong>Đã thanh toán;</strong><br>- Thông tin thanh toán, bao gồm Phương thức - Số tiền - Ngày thanh toán được đồng bộ về HubSpot;<br>- Task KT01, KT04 trên HubSpot được tick <strong>done.</strong></p> | - Nhấn **Cancel** — trạng thái giữ nguyên **Chờ xác nhận** |

**Chi tiết nguyên tắc đồng bộ phương thức thanh toán lần # lên HubSpot**

| Payment Type | Payment Method | Tuition Payment Office | Phương thức thanh toán lần # ghi nhận trênHubSpot |
| ------------ | -------------- | ---------------------- | ------------------------------------------------- |
| Trả thẳng    | Tiền mặt       | NEU                    | TM NEU                                            |
| Trả thẳng    | Tiền mặt       | UEH                    | TM UEH                                            |
| Trả thẳng    | Quẹt POS       | —                      | POS TT                                            |
| Trả góp      | Quẹt POS       | —                      | POS TG                                            |
{% endstep %}
{% endstepper %}

### Xác nhận giao dịch — Hoàn học phí (dành cho TCKT)

{% hint style="info" %}
#### Lưu ý về giao dịch Hoàn học phí

Giao dịch chỉ tồn tại trong trường hợp khách hàng thanh toán thừa học phí (Paid Amount > Net Amount)
{% endhint %}

#### Pre-condition

Sau khi xác định khách hàng thanh toán học phí (Pay-back >0), hệ thống tự tạo giao dịch hoàn học phí cho học viên. Trong đó:

* **Transaction Type** = Hoàn học phí;
* **Payment Method** = Chuyển khoản;
* **Amount** = Pay-back (Học phí hoàn lại)

Chi tiết quy trình xác nhận giao dịch Hoàn học phí như sau:

{% stepper %}
{% step %}
## Kế toán truy cập Transaction List qua task HubSpot (KT03)

Sau khi nhận được request hoàn học phí và thực hiện hoàn trả học phí cho học viên, TCKT thực hiện truy cập link đơn hàng trên task HubSpot (KT03).

→ Hệ thống hiển thị màn hình danh sách giao dịch

![](<.gitbook/assets/image (874)>)

![](<.gitbook/assets/image (875)>)
{% endstep %}

{% step %}
## Chọn giao dịch cần kiểm tra > Chọn **⁝** > Chọn **Confirm Transaction**

Hệ thống hiển thị màn hình thông tin giao dịch để cập nhật thông tin và chứng từ đính kèm.

![](<.gitbook/assets/image (876)>)

![](<.gitbook/assets/image (877)>)
{% endstep %}

{% step %}
## Cập nhật thông tin giao dịch

![](<.gitbook/assets/image (878)>)

User thực hiện cập nhật bổ sung các trường thông tin dưới đây:

| Trường                       | Mô tả                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Remitting Bank Account**   | Ngân hàng thực hiện hoàn học phí cho học viên/khách hàng, bao gồm: - _**MB SAPP**_: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = B2B hoặc CGMA - _**MB SAA**_: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = ACCA hoặc IFRS - _**MB SCFA**_: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = CFA - _**MB SCMA:**_ trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = CMA hoặc Short courses |
| **Paid Date**                | Ngày thực hiện hoàn học phí                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| **Upload chứng từ xác minh** | Cập nhật chứng từ xác minh đã thanh toán hoàn học phí cho học viên File chứng từ ở định dạng: JPG, JPEG, PNG — tối đa 20MB/file                                                                                                                                                                                                                                                                                                                                   |
{% endstep %}

{% step %}
## Chọn **Confirm** để xác nhận giao dịch và Hoàn tất

Sau khi user confirm giao dịch, hệ thống thực hiện:

* Gửi thông báo: **"Transaction confirmed successfully";**
* Chuyển trạng thái sang **Đã thanh toán;**
* Task KT01, KT03 được tick **done**; đồng bộ lên **\[FBP] Học phí hoàn trả** trên HubSpot.

![](<.gitbook/assets/image (879)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chỉ chỉnh sửa được giao dịch khi **Transaction Status = Chờ xác nhận**
2. **Paid Date** không được là ngày trong tương lai
3. Giao dịch **Hoàn học phí** do hệ thống tự tạo — Kế toán không tạo thủ công

### Mẹo sử dụng

1. Chuẩn bị sẵn file chứng từ (JPG/JPEG/PNG, dưới 20MB) trước khi thao tác
2. Kế toán nên truy cập từ link trong task HubSpot để tìm đúng đơn hàng nhanh hơn

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                       | Nguyên nhân                                                        | Cách xử lý                                        |
| ------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------- |
| _"This field is required"_                             | Chưa điền đủ trường bắt buộc                                       | Điền đầy đủ các trường có dấu ✅                   |
| _"Only supported these formats: JPG, JPEG, PNG"_       | Sai định dạng file                                                 | Chuyển file sang JPG, JPEG hoặc PNG               |
| _"Attachment exceeds the maximum size of 20MB"_        | File vượt 20MB                                                     | Nén file xuống dưới 20MB                          |
| Không thấy nút **Chỉnh sửa** / **Confirm Transaction** | Giao dịch đã **Đã thanh toán** hoặc tự động qua Chuyển khoản/VNPay | Kiểm tra trạng thái; liên hệ Admin nếu cần hỗ trợ |
| Không tìm thấy transaction cần xác nhận                | Nhầm đơn hàng                                                      | Truy cập lại từ link trong task HubSpot           |
