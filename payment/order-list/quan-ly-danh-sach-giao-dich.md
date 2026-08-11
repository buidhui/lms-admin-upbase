---
description: >-
  Kết quả đạt được: Danh sách các giao dịch được thực hiện trên mỗi đơn hàng,
  bao gồm Thu học phí và Hoàn học phí.
---

# Quản lý danh sách giao dịch

## Record of changes

A - Add, M - Modify, D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th></tr></thead><tbody><tr><td>June 18, 2026</td><td>Nhungnth</td><td>A</td><td>Create New</td><td>1.0.0</td></tr></tbody></table>

## I. Thông tin chung

{% hint style="success" %}
#### Đối tượng sử dụng

1. **Dành cho:** Admin, Kế toán, TVTS
2. **Đường dẫn:** Module **Order & Payment** → **Order List** → Chọn đơn hàng → **View Order Details** → Tab **Transaction List**
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** [Order List](./)
* **Module liên quan:**
* **Hệ thống tích hợp:** HubSpot, VietQR, VNPay
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

Đã đăng nhập, được cấp quyền truy cập module **Order & Payment** và đơn hàng đã tồn tại trên hệ thống.
{% endhint %}

## II. Hướng dẫn chi tiết

> Quản lý các giao dịch tài chính phát sinh trên đơn hàng, gồm: **Thu học phí** và **Hoàn học phí**.

<details>

<summary>Xem danh sách giao dịch</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Order List**

Tại thanh menu hệ thống: chọn <mark style="color:$primary;">Order & Payment → Order & Payment → chọn tab Transaction List</mark>

<figure><img src="../../.gitbook/assets/image (1427).png" alt=""><figcaption></figcaption></figure>

Danh sách hiển thị các cột trên màn hình danh sách như sau:

| Cột                        | Mô tả                                                                                                                                                                                                                                                                       |
| -------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **No**                     | Số thứ tự                                                                                                                                                                                                                                                                   |
| **Mã thanh toán**          | Tự động với giao dịch Chuyển khoản / VNPay                                                                                                                                                                                                                                  |
| **Transaction type**       | <p>Hiển thị phân loại giao dịch, bao gồm:<br>- <em><strong>Thanh toán học phí</strong>:</em> giao dịch đóng tiền được thực hiện bởi học viên/khách hàng<br><strong>- </strong><em><strong>Hoàn học phí:</strong></em> giao dịch hoàn tiền được thực hiện bởi phòng TCKT</p> |
| **Payment Type**           | <p>Hình thức thanh toán của giao dịch, bao gồm:<br>- <em>Trả thẳng</em><br><em>- Trả góp</em></p>                                                                                                                                                                           |
| **Payment method**         | <p>Phương thức thanh toán của giao dịch, bao gồm:<br>- Chuyển khoản<br>- Thanh toán qua thẻ (tương ứng khi khách hàng thanh toán qua VNPay)<br>- VNPay<br>- Tiền mặt<br>- Quẹt POS</p>                                                                                      |
| **Amount**                 | Số tiền thanh toán trên từng giao dịch thực hiện                                                                                                                                                                                                                            |
| **Recipient Bank Account** | Tài khoản nhận tiền khi Payment Method = Chuyển khoản                                                                                                                                                                                                                       |
| **Tuition Payment Office** | <p>Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm:<br>- NEU<br>- UEH</p>                                                                                                                                                                                          |
| **Remitting Bank Account** | <p>Tài khoản thực hiện hoàn học phí, bao gồm:</p><ul><li>MB SAPP</li><li>MB SAA</li><li>MB SCFA</li><li>MB SCMA</li></ul>                                                                                                                                                   |
| **Paid Date**              | Ngày thanh toán                                                                                                                                                                                                                                                             |
| **Status**                 | <p>Trạng thái của giao dịch, bao gồm:<br>- <em>Chờ xác nhận</em>: giao dịch chờ xác nhận bởi TCKT<br><em>- Đã thanh toán:</em> giao dịch đã thực hiện thành công hoặc được xác nhận bởi TCKT<br><em>- Thất bại:</em> khách hàng thanh toán thất bại</p>                     |
{% endstep %}

{% step %}
**User có thể tìm kiếm nhanh theo điều kiện**

User có thể tìm kiếm theo các điều kiện dưới đây:

* <mark style="color:$primary;">Search mã thanh toán:</mark> Theo mã thanh toán của giao dịch
* <mark style="color:$primary;">Transaction Type:</mark> Theo phân loại giao dịch
* <mark style="color:$primary;">Payment Type:</mark> Theo hình thức thanh toán
* <mark style="color:$primary;">Payment Method:</mark> Theo phương thức thanh toán
* <mark style="color:$primary;">Sort list:</mark> Chọn cách sắp xếp danh sách giao dịch (A-Z, Z-A, Latest, Oldest)

Sau đó, bấm **Search** để hiển thị kết quả mong muốn.

<figure><img src="../../.gitbook/assets/image (1083).png" alt=""><figcaption></figcaption></figure>

Khi muốn xóa bộ lọc, user bấm **Reset** để hiển thị toàn bộ sản phẩm mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết giao dịch</summary>

{% hint style="info" %}
Áp dụng cho: Thanh toán học phí (Tiền mặt/Quẹt POS) và Hoàn học phí.
{% endhint %}

{% stepper %}
{% step %}
**Tại bản ghi cần xem thông tin chi tiết > Chọn&#x20;**<mark style="color:$primary;">**⁝**</mark>**&#x20;> Chọn&#x20;**<mark style="color:$primary;">**View Detail**</mark>

<figure><img src="../../.gitbook/assets/image (1084).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hoàn tất**

Hệ thống hiển thị màn hình chi tiết giao dịch tương ứng.

<figure><img src="../../.gitbook/assets/image (1085).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thêm mới giao dịch</summary>

{% stepper %}
{% step %}
**Tại màn hình List Transaction, chọn&#x20;**<mark style="color:$primary;">**"Add Transaction"**</mark>

Hệ thống chuyển tới màn hình tạo mới giao dịch

{% hint style="info" %}
#### Lưu ý khởi tạo giao dịch

User chỉ có thể khởi tạo giao dịch trong trường hợp khách hàng thanh toán với phương thức = Tiền mặt hoặc Quẹt POS
{% endhint %}

<div><figure><img src="../../.gitbook/assets/image (1086).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1087).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Nhập thông tin giao dịch**

<figure><img src="../../.gitbook/assets/image (1088).png" alt=""><figcaption></figcaption></figure>

Chi tiết các trường thông tin dưới đây:

<table><thead><tr><th>Trường</th><th width="137" align="center">Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td><strong>Transaction type</strong></td><td align="center">Tự động</td><td>Phân loại giao dịch, hiển thị mặc định = Thu học phí</td></tr><tr><td><strong>Payment Type</strong></td><td align="center">✅</td><td>Hình thức thanh toán của giao dịch, bao gồm:<br>- <em>Trả thẳng</em><br><em>- Trả góp</em></td></tr><tr><td><strong>Payment method</strong></td><td align="center">✅</td><td>Phương thức thanh toán của giao dịch, bao gồm:<br>- Tiền mặt<br>- Quẹt POS</td></tr><tr><td><strong>Tuition Payment Office</strong></td><td align="center">✅</td><td>Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm:<br>- NEU<br>- UEH<br><br>Chỉ hiển thị khi Payment method = Tiền mặt</td></tr><tr><td><strong>Amount</strong></td><td align="center">✅</td><td>Số tiền thanh toán trên từng giao dịch thực hiện</td></tr><tr><td><strong>Paid Date</strong></td><td align="center">✅</td><td>Ngày thanh toán (≤ ngày hiện tại)</td></tr><tr><td><strong>Transaction Status</strong></td><td align="center">Tự động</td><td>Trạng thái của giao dịch — hiển thị mặc định = <em><strong>Chờ xác nhận</strong></em></td></tr><tr><td><strong>Upload chứng từ xác minh</strong></td><td align="center">✅</td><td>Đăng tải chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG — tối đa 20MB/file, nhiều file</td></tr></tbody></table>

{% hint style="info" %}
**Logic Payment method:**

* Transaction type = Hoàn học phí → **Chuyển khoản**
* Payment Type = Trả thẳng → Tiền mặt, Quẹt POS
* Payment Type = Trả góp → Quẹt POS
{% endhint %}
{% endstep %}

{% step %}
**Nhấn&#x20;**<mark style="color:$primary;">**"Chuyển xác nhận"**</mark>

Sau khi nhập thông tin, chọn Chuyển xác nhận để lưu giao dịch và chuyển cho TCKT xác nhận. Sau đó, hệ thống thực hiện:

* Gửi thông báo **"Transaction successfully submitted for approval"**
* Tạo bản ghi xuất hiện trên lưới với trạng thái = **Chờ xác nhận**
* Hệ thống tạo task HubSpot (KT04) gửi Kế toán kèm link transaction

<figure><img src="../../.gitbook/assets/image (1089).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa giao dịch</summary>

{% hint style="warning" %}
#### Lưu ý chỉnh sửa giao dịch

Chỉ chỉnh sửa được khi **Transaction Status = Chờ xác nhận**
{% endhint %}

{% stepper %}
{% step %}
**Tại màn hình List Transaction > Chọn giao dịch cần chỉnh sửa > Chọn&#x20;**<mark style="color:$primary;">**⁝**</mark>**&#x20;> Chọn&#x20;**<mark style="color:$primary;">**Edit Transaction**</mark>

Hệ thống hiển thị màn hình chỉnh sửa thông tin của giao dịch.

<figure><img src="../../.gitbook/assets/image (1090).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin giao dịch**

Chi tiết các trường thông tin hiển thị được trình bày dưới đây:

<table><thead><tr><th>Trường thông tin</th><th width="137" align="center">Bắt buộc</th><th>Hướng dẫn chỉnh sửa</th></tr></thead><tbody><tr><td><strong>Transaction type</strong></td><td align="center">Tự động</td><td>Không được phép chỉnh sửa</td></tr><tr><td><strong>Payment Type</strong></td><td align="center">✅</td><td>Hình thức thanh toán của giao dịch, bao gồm:<br>- <em>Trả thẳng</em><br><em>- Trả góp</em></td></tr><tr><td><strong>Payment method</strong></td><td align="center">✅</td><td>Phương thức thanh toán của giao dịch, bao gồm:<br>- Tiền mặt<br>- Quẹt POS</td></tr><tr><td><strong>Tuition Payment Office</strong></td><td align="center">✅</td><td>Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm:<br>- NEU<br>- UEH<br><br>Chỉ hiển thị khi Payment method = Tiền mặt</td></tr><tr><td><strong>Amount</strong></td><td align="center">✅</td><td>Số tiền thanh toán trên từng giao dịch thực hiện</td></tr><tr><td><strong>Paid Date</strong></td><td align="center">✅</td><td>Ngày thanh toán (≤ ngày hiện tại)</td></tr><tr><td><strong>Transaction Status</strong></td><td align="center">Tự động</td><td>Không được phép chỉnh sửa</td></tr><tr><td><strong>Upload chứng từ xác minh</strong></td><td align="center">✅</td><td>Đăng tải chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG — tối đa 20MB/file, nhiều file</td></tr></tbody></table>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Update**</mark>**&#x20;để lưu thông tin đã chỉnh sửa**

Hệ thống cập nhật thông tin của bản ghi theo dữ liệu user đã chỉnh sửa

<figure><img src="../../.gitbook/assets/image (1091).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xác nhận giao dịch — Thu học phí (dành cho TCKT)</summary>

{% stepper %}
{% step %}
**Kế toán truy cập Transaction List qua link trong task HubSpot (KT04)**

Sau khi nhận được task kiểm tra thanh toán bằng Tiền mặt hoặc quẹt POS, TCKT thực hiện truy cập link đơn hàng trên task HubSpot (KT04).

→ Hệ thống hiển thị màn hình danh sách giao dịch.

<div><figure><img src="../../.gitbook/assets/image (1093).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1094).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Chọn giao dịch cần kiểm tra > Chọn&#x20;**<mark style="color:$primary;">**⁝**</mark>**&#x20;> Chọn&#x20;**<mark style="color:$primary;">**Confirm Transaction**</mark>

Hệ thống hiển thị màn hình thông tin giao dịch để kiểm tra thông tin và chứng từ đính kèm.

<div><figure><img src="../../.gitbook/assets/image (1095).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1096).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Kiểm tra thông tin giao dịch**

User thực hiện kiểm tra thông tin giao dịch, chi tiết như sau:

<table><thead><tr><th width="172.66668701171875">Trường</th><th>Mô tả</th></tr></thead><tbody><tr><td><strong>Transaction type</strong></td><td>Phân loại giao dịch, hiển thị mặc định = Thu học phí</td></tr><tr><td><strong>Payment Type</strong></td><td>Hình thức thanh toán của giao dịch, bao gồm:<br>- <em>Trả thẳng</em><br><em>- Trả góp</em></td></tr><tr><td><strong>Payment method</strong></td><td>Phương thức thanh toán của giao dịch, bao gồm:<br>- Tiền mặt<br>- Quẹt POS</td></tr><tr><td><strong>Tuition Payment Office</strong></td><td>Cơ sở thu học phí khi payment method = Tiền mặt, bao gồm:<br>- NEU<br>- UEH<br><br>Chỉ hiển thị khi Payment method = Tiền mặt</td></tr><tr><td><strong>Amount</strong></td><td>Số tiền thanh toán trên từng giao dịch thực hiện</td></tr><tr><td><strong>Paid Date</strong></td><td>Ngày thanh toán (≤ ngày hiện tại)</td></tr><tr><td><strong>Transaction Status</strong></td><td>Trạng thái của giao dịch — hiển thị mặc định = <em><strong>Chờ xác nhận</strong></em></td></tr><tr><td><strong>Tệp đính kèm</strong></td><td>Chứng từ xác minh đã thanh toán học phí theo các định dạng: JPG, JPEG, PNG</td></tr></tbody></table>
{% endstep %}

{% step %}
**Nhấn&#x20;**<mark style="color:$primary;">**"Confirm"**</mark>**&#x20;để xác nhận**

<figure><img src="../../.gitbook/assets/image (1092).png" alt=""><figcaption></figcaption></figure>

User thực hiện xác nhận thông tin của giao dịch. Sau đó, nếu:

{% tabs %}
{% tab title="Confirm" icon="octagon-check" %}
* Thông báo: **"Transaction confirmed successfully";**
* Trạng thái chuyển sang **Đã thanh toán;**
* Thông tin thanh toán, bao gồm Phương thức - Số tiền - Ngày thanh toán được đồng bộ về HubSpot;
* Task KT01, KT04 trên HubSpot được tick **done.**
{% endtab %}

{% tab title="Cancel" icon="circle-x" %}
* Nhấn **Cancel** — trạng thái giữ nguyên **Chờ xác nhận**
{% endtab %}
{% endtabs %}

{% hint style="info" %}
**Chi tiết nguyên tắc đồng bộ phương thức thanh toán lần # lên HubSpot**
{% endhint %}

<table><thead><tr><th width="129">Payment Type</th><th width="135">Payment Method</th><th width="144">Tuition Payment Office</th><th>Phương thức thanh toán lần # ghi nhận trênHubSpot</th></tr></thead><tbody><tr><td>Trả thẳng</td><td>Tiền mặt</td><td>NEU</td><td>TM NEU</td></tr><tr><td>Trả thẳng</td><td>Tiền mặt</td><td>UEH</td><td>TM UEH</td></tr><tr><td>Trả thẳng</td><td>Quẹt POS</td><td>—</td><td>POS TT</td></tr><tr><td>Trả góp</td><td>Quẹt POS</td><td>—</td><td>POS TG</td></tr></tbody></table>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xác nhận giao dịch — Hoàn học phí (dành cho TCKT)</summary>

{% hint style="info" %}
#### Lưu ý về giao dịch Hoàn học phí

Giao dịch chỉ tồn tại trong trường hợp khách hàng thanh toán thừa học phí (Paid Amount > Net Amount)
{% endhint %}

{% hint style="success" %}
#### Pre-condition

Sau khi xác định khách hàng thanh toán học phí (Pay-back >0), hệ thống tự tạo giao dịch hoàn học phí cho học viên. Trong đó:

* **Transaction Type** = Hoàn học phí;
* **Payment Method** = Chuyển khoản;
* **Amount** = Pay-back (Học phí hoàn lại)
{% endhint %}

Chi tiết quy trình xác nhận giao dịch Hoàn học phí như sau:

{% stepper %}
{% step %}
**Kế toán truy cập Transaction List qua task HubSpot (KT03)**

Sau khi nhận được request hoàn học phí và thực hiện hoàn trả học phí cho học viên, TCKT thực hiện truy cập link đơn hàng trên task HubSpot (KT03).

→ Hệ thống hiển thị màn hình danh sách giao dịch

<div><figure><img src="../../.gitbook/assets/image (1100).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1101).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Chọn giao dịch cần kiểm tra > Chọn&#x20;**<mark style="color:$primary;">**⁝**</mark>**&#x20;> Chọn&#x20;**<mark style="color:$primary;">**Confirm Transaction**</mark>

Hệ thống hiển thị màn hình thông tin giao dịch để cập nhật thông tin và chứng từ đính kèm.

<div><figure><img src="../../.gitbook/assets/image (1102).png" alt=""><figcaption></figcaption></figure> <figure><img src="../../.gitbook/assets/image (1103).png" alt=""><figcaption></figcaption></figure></div>
{% endstep %}

{% step %}
**Cập nhật thông tin giao dịch**

<figure><img src="../../.gitbook/assets/image (1105).png" alt=""><figcaption></figcaption></figure>

User thực hiện cập nhật bổ sung các trường thông tin dưới đây:

<table><thead><tr><th width="169">Trường</th><th>Mô tả</th></tr></thead><tbody><tr><td><strong>Remitting Bank Account</strong></td><td>Ngân hàng thực hiện hoàn học phí cho học viên/khách hàng, bao gồm:<br>- <em><strong>MB SAPP</strong></em>: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = B2B hoặc CGMA<br><br>- <em><strong>MB SAA</strong></em>: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = ACCA hoặc IFRS<br><br>- <em><strong>MB SCFA</strong></em>: trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = CFA<br><br>- <em><strong>MB SCMA:</strong></em> trong trường hợp khách hàng đã mua các sản phẩm thuộc Category = CMA hoặc Short courses</td></tr><tr><td><strong>Paid Date</strong></td><td>Ngày thực hiện hoàn học phí</td></tr><tr><td><strong>Upload chứng từ xác minh</strong></td><td>Cập nhật chứng từ xác minh đã thanh toán hoàn học phí cho học viên<br>File chứng từ ở định dạng: JPG, JPEG, PNG — tối đa 20MB/file</td></tr></tbody></table>
{% endstep %}

{% step %}
**Chọn&#x20;**<mark style="color:$primary;">**Confirm**</mark>**&#x20;để xác nhận giao dịch và Hoàn tất**

Sau khi user confirm giao dịch, hệ thống thực hiện:

* Gửi thông báo: **"Transaction confirmed successfully";**
* Chuyển trạng thái sang **Đã thanh toán;**
* Task KT01, KT03 được tick **done**; đồng bộ lên **\[FBP] Học phí hoàn trả** trên HubSpot.

<figure><img src="../../.gitbook/assets/image (1104).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ chỉnh sửa được giao dịch khi **Transaction Status = Chờ xác nhận**
2. **Paid Date** không được là ngày trong tương lai
3. Giao dịch **Hoàn học phí** do hệ thống tự tạo — Kế toán không tạo thủ công
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Chuẩn bị sẵn file chứng từ (JPG/JPEG/PNG, dưới 20MB) trước khi thao tác
2. Kế toán nên truy cập từ link trong task HubSpot để tìm đúng đơn hàng nhanh hơn
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                       | Nguyên nhân                                                        | Cách xử lý                                        |
| ------------------------------------------------------ | ------------------------------------------------------------------ | ------------------------------------------------- |
| _"This field is required"_                             | Chưa điền đủ trường bắt buộc                                       | Điền đầy đủ các trường có dấu ✅                   |
| _"Only supported these formats: JPG, JPEG, PNG"_       | Sai định dạng file                                                 | Chuyển file sang JPG, JPEG hoặc PNG               |
| _"Attachment exceeds the maximum size of 20MB"_        | File vượt 20MB                                                     | Nén file xuống dưới 20MB                          |
| Không thấy nút **Chỉnh sửa** / **Confirm Transaction** | Giao dịch đã **Đã thanh toán** hoặc tự động qua Chuyển khoản/VNPay | Kiểm tra trạng thái; liên hệ Admin nếu cần hỗ trợ |
| Không tìm thấy transaction cần xác nhận                | Nhầm đơn hàng                                                      | Truy cập lại từ link trong task HubSpot           |
