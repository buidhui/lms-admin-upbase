# Quản lý giảng viên (Teacher)

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| 28/05/2026     | Lê Thị Huế    | M     | Chuẩn hóa nội dung lên GitBook | 4.2.0   |

## Definitions and Acronyms

| # | Term             | Definition                                            |
| - | ---------------- | ----------------------------------------------------- |
| 1 | LMS Admin        | Hệ thống quản lý vận hành                |
| 2 | LMS              | Learning Management System — Hệ thống quản lý học tập |
| 3 | Person in charge | Nhân viên UpBase phụ trách giảng viên                   |
| 4 | Facility         | Cơ sở giảng dạy của giảng viên                        |
| 5 | DOB              | Date of Birth — Ngày sinh                             |
| 6 | OTP              | One-Time Password — Mã xác thực một lần               |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Operator

**Đường dẫn:** User Management → Teachers → Teacher List
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Teacher Management (thuộc User Management)
* **Module liên quan:** Teaching Program, LMS Pro
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống LMS Admin.
* Đã đăng nhập thành công vào hệ thống.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện (xem / tạo / chỉnh sửa / import).
* Đã nắm danh sách Chương trình (Program) và các môn học (Subject) hiện có trong hệ thống.
{% endhint %}

## II. Tổng quan giao diện

Màn hình **Teacher Management** bao gồm các khu vực chính:

* **Thanh điều hướng trái:** User Management → Teachers
* **Thanh tìm kiếm & bộ lọc:** Search (Họ tên / Username / Email / SĐT), Gender, Status, From Date – To Date, Teaching Status, Program, Subject, Section, Person in Charge
* **Bảng danh sách:** Hiển thị danh sách giảng viên theo thời gian tạo giảm dần
* **Nút thao tác (Action):** View Profile, Edit, Reset Password, Edit Email, Block
* **Nút chức năng chính:** Create (tạo mới), Import (nhập hàng loạt), Export (xuất Excel)

#### Đối tượng áp dụng

| Đối tượng | Vai trò            | Quyền hạn                                                              |
| --------- | ------------------ | ---------------------------------------------------------------------- |
| Admin     | Quản trị hệ thống  | Toàn quyền — xem, tạo, chỉnh sửa, đổi trạng thái, import, export       |
| Operator  | Nhân viên vận hành | Tùy theo Role được cấp trong hệ thống (xem / tạo / chỉnh sửa / import) |

## III. Các bước thực hiện chi tiết

<details>

<summary>3.1 Xem danh sách và truy cập chi tiết giảng viên</summary>

{% stepper %}
{% step %}
**Truy cập Teacher List**

Từ thanh điều hướng bên trái, nhấn vào **Teachers** → chọn **Teacher List**. Danh sách giảng viên hiển thị theo thời gian tạo giảm dần.

<figure><img src="../.gitbook/assets/image (1228).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm và lọc giảng viên**

<figure><img src="../.gitbook/assets/image (1229).png" alt=""><figcaption></figcaption></figure>

Sử dụng các bộ lọc phía trên bảng danh sách:

* **Search:** tìm theo Họ tên (Full name), Username, Email, Số điện thoại — cần nhập đủ từ.
* **Gender** (Giới tính): chọn 1 trong các giá trị cho trước.
* **Status** (Trạng thái): chọn 1 trong các giá trị cho trước (Active / Block).
* **From Date – To Date:** lọc theo ngày cập nhật thông tin.
* **Teaching Status:** trạng thái giảng dạy, chọn 1 trong các giá trị cho trước.
* **Program:** chương trình giảng dạy, chọn 1 trong các giá trị cho trước.
* **Subject:** môn giảng dạy, chọn 1 trong các giá trị cho trước.
* **Section:** section giảng dạy, chọn 1 trong các giá trị cho trước.
* **Person in Charge:** người chịu trách nhiệm, chọn 1 trong các giá trị cho trước.

Nhấn **Search** để hiển thị kết quả. Nhấn **Reset** để xóa toàn bộ bộ lọc.
{% endstep %}

{% step %}
**Xem thông tin chi tiết giảng viên**

<figure><img src="../.gitbook/assets/image (1230).png" alt=""><figcaption></figcaption></figure>

Nhấn vào tên giảng viên hoặc nhấn **Action → View Profile**. Màn hình Teacher Profile hiển thị các tab:

* **Overview:** Code, Full Name, Username, Email, Address, Phone Number, Account Status, Test Account, Teaching Status, Person in Charge, Gender, Job Title, D.O.B, Facility, Current Company, Facebook, Youtube, LinkedIn, Certificate File, Updated At, Description.

<figure><img src="../.gitbook/assets/image (1231).png" alt=""><figcaption></figcaption></figure>

* **Setting:** Cho phép cập nhật các thông tin: Code, Full Name, Address, Phone, Status, File chứng chỉ đi kèm, Job Title, Teaching Status, Person in Charge, Facebook, Youtube, LinkedIn, Description.

<figure><img src="../.gitbook/assets/image (1232).png" alt=""><figcaption></figcaption></figure>

* **Teaching Program:** Nội dung giảng dạy theo từng chương trình (CFA/ACCA/CMA), danh sách môn và mức độ ưu tiên.

<figure><img src="../.gitbook/assets/image (1233).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xuất danh sách ra Excel**

<figure><img src="../.gitbook/assets/image (1234).png" alt=""><figcaption></figcaption></figure>

Tại màn hình Teacher List, nhấn **Export**. Hệ thống xuất danh sách giảng viên (theo điều kiện tìm kiếm hiện tại) thành file Excel và tự động tải về thiết bị.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.2 Tạo tài khoản giảng viên</summary>

{% stepper %}
{% step %}
**Truy cập màn hình tạo tài khoản**

<figure><img src="../.gitbook/assets/image (1236).png" alt=""><figcaption></figcaption></figure>

Tại màn hình Teacher List, nhấn nút **Create** để chuyển đến màn hình Create Teacher.
{% endstep %}

{% step %}
**Điền thông tin giảng viên**

<figure><img src="../.gitbook/assets/image (1237).png" alt=""><figcaption></figcaption></figure>

Điền các trường thông tin. Các trường có dấu **(\*)** là bắt buộc:

**Thông tin cá nhân:**

* **Avatar:** tải ảnh đại diện từ thiết bị.
* **Code:** mã giảng viên, nhập theo quy định nội bộ.
* **Full Name (\*):** tối đa 100 ký tự.
* **Username (\*):** 6–40 ký tự, không trùng.
* **Email (\*):** đúng định dạng, không trùng email đã tồn tại.
* **Password & Confirm Password (\*):** theo điều kiện hệ thống.
* **Phone number (\*):** 10–11 số, bắt đầu bằng 0, không trùng SĐT đã tồn tại.
* **Address:** nhập dạng text địa chỉ.
* **Gender (\*):** chọn 1 giá trị.
* **DOB:** ngày sinh.

**Thông tin giảng dạy:**

* **Facility (\*):** cơ sở giảng dạy.
* **Job Title:** chức vụ.
* **Teaching Status (\*):** trạng thái giảng dạy tại UpBase.
* **Person in Charge (\*):** nhân viên UpBase phụ trách.

**Liên kết mạng xã hội (tùy chọn):** Facebook, LinkedIn, Youtube.

**Description:** ghi chú về giảng viên.

**File chứng chỉ:**

* Định dạng cho phép: pdf, docx, doc, xls, xlsx, csv, txt, ppt, pptx, zip.
* Dung lượng tối đa: 500 MB/file.

**Teaching Program (\*):**

* **Primary Responsibility (\*):** chọn 1 chương trình chính (CFA / ACCA / CMA).
* **Các nội dung có thể giảng dạy:** tick chọn nhiều môn học.
* **Mức độ ưu tiên theo từng môn:** Ưu tiên 1 > Ưu tiên 2 > Không ưu tiên (= Chưa có giáo án).
{% endstep %}

{% step %}
**Lưu tài khoản**

<figure><img src="../.gitbook/assets/image (1238).png" alt=""><figcaption></figcaption></figure>

Nhấn **Save** → chọn **Yes** khi hộp thoại xác nhận hiển thị. Tài khoản mới xuất hiện ở đầu danh sách Teacher List.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.3 Chỉnh sửa thông tin giảng viên</summary>

{% stepper %}
{% step %}
**Truy cập màn hình chỉnh sửa**

Có 3 cách truy cập màn hình chỉnh sửa thông tin giảng viên:

* **Cách 1:** Tại Teacher List → nhấn **Action** → chọn **Edit**.

<figure><img src="../.gitbook/assets/image (1239).png" alt=""><figcaption></figcaption></figure>

* **Cách 2:** Nhấn vào tên giảng viên → chọn **Edit Profile**.

<figure><img src="../.gitbook/assets/image (1240).png" alt=""><figcaption></figcaption></figure>

* **Cách 3:** Nhấn vào tên giảng viên → chọn tab **Setting**.

<figure><img src="../.gitbook/assets/image (1241).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin cơ bản**

<figure><img src="../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>

**Các trường có thể chỉnh sửa:** Avatar, Full Name (\*), Gender (\*), DOB, Facility (\*), Job Title, Teaching Status (\*), Person in Charge (\*), Facebook, LinkedIn, Youtube, Description, File chứng chỉ.

**Các trường KHÔNG được phép chỉnh sửa:**

* **Username (\*)** — định danh duy nhất, không thay đổi sau khi tạo.
* **Phone (\*)** — định danh duy nhất, không thay đổi sau khi tạo.

**Các trường có quy trình riêng:**

* **Email (\*):** thay đổi qua tính năng Edit Email — [xem hướng dẫn tại đây](https://sapp-academy.gitbook.io/sapp-academy/~/revisions/jJXeizmPeI0YOMZR7XZI/nguoi-dung-user-management/pages/kilkVFJKJHZcpGjzHenO#id-3.4-edit-email).
* **Môn học giảng dạy:** thay đổi qua bước tiếp theo (tab Teaching Program).

Nhấn **Save** để lưu thay đổi.
{% endstep %}

{% step %}
**Thay đổi môn học giảng dạy (Teaching Program)**

<figure><img src="../.gitbook/assets/image (1243).png" alt=""><figcaption></figcaption></figure>

Tại trang chi tiết giảng viên, chọn tab **Teaching Program** → chọn chương trình muốn chỉnh sửa → nhấn **Edit Subjects**. Tại đây có thể:

* Thay đổi **Primary Responsibility** (chương trình giảng dạy chính).
* Tick / untick các môn học mà giảng viên có thể giảng dạy.
* Chỉnh mức độ ưu tiên: Ưu tiên 1 > Ưu tiên 2 > Không ưu tiên.

Nhấn **Save** → chọn **Yes** khi hộp thoại xác nhận hiển thị.

<figure><img src="../.gitbook/assets/image (1244).png" alt=""><figcaption></figcaption></figure>

✅ Kết quả: Thông tin giảng viên được cập nhật thành công.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.4 Thay đổi trạng thái giảng viên</summary>

Hệ thống hỗ trợ 2 trạng thái tài khoản giảng viên:

| Trạng thái | Mô tả                                                                    |
| ---------- | ------------------------------------------------------------------------ |
| Active     | Tài khoản đang được kích hoạt, có thể đăng nhập vào LMS Pro để giảng dạy |
| Block      | Tài khoản bị khóa, không thể đăng nhập vào LMS Pro                       |

{% stepper %}
{% step %}
**Cách 1 — Thay đổi qua nút Action**

Tại Teacher List, nhấn **Action** tương ứng với giảng viên cần đổi trạng thái → chọn **Block** (áp dụng cho tài khoản đang Active).

<figure><img src="../.gitbook/assets/image (1248).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cách 2 — Thay đổi qua trường Status**

Nhấn trực tiếp vào giá trị trường **Status** trong bảng danh sách hoặc trên trang Teacher Profile → chọn giá trị mới (Active / Block) để chuyển đổi trạng thái.

<figure><img src="../.gitbook/assets/image (1246).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận thay đổi trạng thái**

<figure><img src="../.gitbook/assets/image (1247).png" alt=""><figcaption></figcaption></figure>

Xác nhận khi hộp thoại hiển thị.

{% hint style="warning" %}
Khi giảng viên bị **Block**, các lớp/khóa học đã được phân công cho giảng viên này vẫn giữ nguyên — cần điều chuyển sang giảng viên khác nếu cần thiết.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.5 Import hàng loạt giảng viên</summary>

{% stepper %}
{% step %}
**Mở hộp thoại Import**

Tại màn hình Teacher List, nhấn nút **Import** để hiển thị hộp thoại tải file.

<figure><img src="../.gitbook/assets/image (1175).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn file và kiểm tra định dạng**

Chọn **Browse** để chọn file từ thiết bị. Lưu ý:

* Chỉ chấp nhận định dạng **.csv** hoặc **.xlsx**.
* Mỗi lần chỉ được chọn 1 file.
* Người dùng có thể tải **file mẫu (template)** về để tham khảo cách điền thông tin hợp lệ.

<figure><img src="../.gitbook/assets/image (910).png" alt=""><figcaption></figcaption></figure>

Các trường bắt buộc trong file import:

| Trường        | Điều kiện                                                                                                                                      |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Username      | 6–40 ký tự, không chứa khoảng trắng, không chứa ký tự tiếng Việt có dấu và ký tự đặc biệt (ngoại trừ . - \_), không trùng username đã tồn tại. |
| Email         | Đúng định dạng abc@abc.abc, không trùng email đã tồn tại.                                                                                      |
| Phone         | 10–11 ký tự số, bắt đầu bằng 0, không trùng SĐT đã tồn tại.                                                                                    |
| Full Name     | Họ và tên đầy đủ của giảng viên.                                                                                                               |
| Status        | Active hoặc Block.                                                                                                                             |
| Testing Staff | Yes hoặc No — xác định tài khoản test nội bộ.                                                                                                  |
| Type User     | Employee hoặc Student — xác định loại User.                                                                                                    |
{% endstep %}

{% step %}
**Click "Import" để tải file lên hệ thống**

Nhấn **Import** để bắt đầu xử lý file.

<figure><img src="../.gitbook/assets/image (911).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Kiểm tra kết quả và xem log lỗi**

Hộp thoại kết quả hiển thị các thông tin:

* **Source:** tên file đã tải lên.
* **Data:** số lượng bản ghi trong file.
* **Successfully:** số tài khoản được tạo thành công.
* **Error:** số tài khoản tạo thất bại.

<figure><img src="../.gitbook/assets/image (912).png" alt=""><figcaption></figcaption></figure>

Nhấp vào **View Log** để xem chi tiết tình trạng tạo tài khoản. Những trường không hợp lệ sẽ được bôi đỏ, kèm lỗi cụ thể tại cột **Errors**.

<figure><img src="../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Sau khi import, các thông tin về **Teaching Program** (Primary Responsibility, môn học, mức độ ưu tiên) cần được bổ sung thủ công cho từng giảng viên qua màn hình Edit.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

## IV. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Username** và **Số điện thoại** KHÔNG được phép chỉnh sửa sau khi tạo tài khoản — đây là định danh duy nhất của giảng viên.
2. Thay đổi **Email** yêu cầu xác thực OTP gửi về Email cũ — cần đảm bảo Email cũ còn hoạt động. Chỉ user có quyền Edit tài khoản Teacher mới được thực hiện.
3. Tài khoản giảng viên bị **Block** sẽ không thể đăng nhập vào LMS Pro để giảng dạy.
4. Mỗi giảng viên chỉ có **1 Primary Responsibility** (chương trình giảng dạy chính).
5. Mức độ ưu tiên **"Không ưu tiên"** đồng nghĩa với việc giảng viên chưa có giáo án cho môn học đó.
6. File chứng chỉ có dung lượng tối đa **500 MB/file**, hỗ trợ nhiều định dạng: pdf, docx, doc, xls, xlsx, csv, txt, ppt, pptx, zip.
7. File Import chỉ chấp nhận định dạng **.csv** hoặc **.xlsx**; mỗi lần chỉ import 1 file.
8. Các trường **Username, Email, SĐT** trong file import phải là duy nhất, không trùng dữ liệu đã có trong hệ thống.
9. Thông tin **Teaching Program** không được nhập qua Import — phải bổ sung thủ công sau khi tạo tài khoản.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Tải **file mẫu (template)** trước khi import để đảm bảo đúng định dạng cột và dữ liệu.
2. Dùng **View Log** sau import để kiểm tra chi tiết lỗi và sửa từng bản ghi lỗi trước khi import lại.
3. Kết hợp nhiều bộ lọc (Search + Status + Gender + Date) để thu hẹp kết quả tìm kiếm nhanh hơn.
4. Cập nhật đầy đủ **Teaching Program** và mức độ ưu tiên ngay sau khi tạo tài khoản để hệ thống phân lớp/khóa được chính xác.
5. Sử dụng tab **Teaching Program** để xem nhanh năng lực giảng dạy của giảng viên trước khi phân công lớp.
{% endhint %}

## V. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                     | Nguyên nhân                                                                | Cách xử lý                                                                                                            |
| ---------------------------------------------------- | -------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Không tìm thấy giảng viên trong danh sách            | Bộ lọc quá chặt hoặc nhập sai từ khóa                                      | Nhấn **Reset** để xóa toàn bộ bộ lọc, thử lại với từ khóa khác. Đảm bảo nhập đủ từ khi search.                        |
| Không thể lưu tài khoản mới                          | Thiếu trường bắt buộc (\*) hoặc dữ liệu không hợp lệ                       | Kiểm tra các trường có dấu (\*), đảm bảo Username / Email / SĐT chưa tồn tại trong hệ thống.                          |
| Không upload được file chứng chỉ                     | File quá lớn (>500MB) hoặc sai định dạng                                   | Kiểm tra dung lượng và đảm bảo file thuộc định dạng được hỗ trợ: pdf, docx, doc, xls, xlsx, csv, txt, ppt, pptx, zip. |
| Không chọn được môn học cho giảng viên               | Chưa chọn Primary Responsibility hoặc môn không thuộc chương trình đã chọn | Vào tab **Teaching Program**, chọn **Primary Responsibility** trước, sau đó tick chọn các môn học tương ứng.          |
| File import bị lỗi một số dòng                       | Dữ liệu các cột không đúng định dạng yêu cầu                               | Nhấn **View Log** để xem chi tiết dòng lỗi, sửa file theo hướng dẫn tại cột **Errors** và import lại.                 |
| File import không tải được                           | Định dạng file không phải .csv / .xlsx hoặc file quá lớn                   | Kiểm tra lại định dạng file. Tách nhỏ file nếu quá lớn và import từng lần.                                            |
| Giảng viên bị Block báo không đăng nhập được LMS Pro | Tài khoản đã bị khóa trên hệ thống LMS Admin                                     | Vào Teacher Profile, đổi trạng thái về **Active** (nếu được phép) hoặc xác nhận với Admin lý do block.                |
| Danh sách không tải được                             | Mất kết nối hoặc lỗi server                                                | Tải lại trang (F5). Nếu vẫn lỗi, liên hệ IT để hỗ trợ.                                                                |

## VI. Câu hỏi thường gặp (FAQ)

<details>

<summary>Tôi không thấy tài khoản giảng viên cần tìm dù đã tìm kiếm?</summary>

Kiểm tra lại bộ lọc đang áp dụng — nhấn **Reset** để xóa tất cả bộ lọc và tìm lại. Lưu ý ô Search cần nhập đủ từ. Nếu vẫn không thấy, tài khoản có thể không thuộc phạm vi quyền xem của bạn — liên hệ Admin.

</details>

<details>

<summary>Tại sao tôi không chỉnh sửa được Username và Số điện thoại của giảng viên?</summary>

Đây là quy tắc nghiệp vụ để đảm bảo tính nhất quán dữ liệu. Username và SĐT là định danh duy nhất của tài khoản, không được phép thay đổi sau khi tạo. Nếu cần sửa, phải tạo tài khoản mới.

</details>

<details>

<summary>Một giảng viên có thể giảng dạy nhiều chương trình không?</summary>

Có. Giảng viên có thể tick chọn nhiều môn học thuộc nhiều chương trình khác nhau. Tuy nhiên, mỗi giảng viên chỉ có 1 **Primary Responsibility** (chương trình giảng dạy chính).

</details>

<details>

<summary>Mức độ ưu tiên môn học hoạt động như thế nào?</summary>

Hệ thống ưu tiên phân lớp/khóa theo thứ tự: Ưu tiên 1 > Ưu tiên 2 > Không ưu tiên. Giảng viên ở mức "Không ưu tiên" được hiểu là chưa có giáo án cho môn đó và sẽ ít được ưu tiên phân công.

</details>

<details>

<summary>File import của tôi có nhiều dòng lỗi, tôi cần làm gì?</summary>

Sau khi import, nhấn **View Log** để xem chi tiết các dòng lỗi. Mở lại file gốc, sửa các dòng bị bôi đỏ theo hướng dẫn tại cột **Errors**, sau đó import lại file đã sửa. Bạn cũng có thể vào **Teachers → Import Report** để xem lại lịch sử import.

</details>

<details>

<summary>Sau khi import, tại sao giảng viên chưa có Teaching Program?</summary>

Import chỉ tạo các thông tin tài khoản cơ bản (Username, Email, Phone, Full Name, Status). Các thông tin về Teaching Program (Primary Responsibility, môn học, mức ưu tiên) cần được bổ sung thủ công qua màn hình Edit của từng giảng viên.

</details>

<details>

<summary>Giảng viên bị Block có thể tự kích hoạt lại tài khoản không?</summary>

Không. Chỉ người dùng có quyền trên hệ thống LMS Admin (Admin / Operator có quyền) mới có thể thay đổi trạng thái từ Block về Active.

</details>

<details>

<summary>Có thể upload nhiều file chứng chỉ cho 1 giảng viên không?</summary>

Có. Mỗi giảng viên có thể có nhiều file chứng chỉ. Mỗi file có dung lượng tối đa 500 MB và phải thuộc các định dạng được hỗ trợ: pdf, docx, doc, xls, xlsx, csv, txt, ppt, pptx, zip.

</details>
