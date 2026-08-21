# Quản lý học viên (Student)

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Operator

**Đường dẫn:** User & Org Management → Students
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Student Management (thuộc User Management)
* **Hệ thống tích hợp:** LMS Pro (giao diện học viên), HubSpot (Contact, thông tin học viên)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống OPS.
* Đã đăng nhập thành công vào hệ thống.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện (xem / tạo / chỉnh sửa / import).
{% endhint %}

## II. Tổng quan giao diện

**Giao diện danh sách học viên**

Màn hình Danh sách học viên gồm các khu vực chính:

* Thanh điều hướng trái.
* Thanh tìm kiếm, bộ lọc: Search (Fullname, Username, Email, SĐT).
* Bảng danh sách: Hiển thị danh sách học viên với các trường thông tin: ID, User, Username, Phone, Additional Emails, Status, Type User, Date.
* Nút thao tác **Action** tại mỗi bản ghi học viên.
* Nút chức năng chính: **Create** (Tạo mới), **Import** (nhập hàng loạt), **Export** (xuất excel).

**Giao diện chi tiết học viên**

Màn hình Chi tiết học viên gồm:

* **Overview**: Chứa Personal Information, Account Information, Profile 1, Profile 2, Profile 3 (trong trường hợp học viên có nhiều email hoặc SĐT).
* **Setting**: Người dùng có thể truy cập để cập nhật các thông tin học viên tại tab này.
* **Class & Course**: Chi tiết thông tin học viên đó đã tham gia những lớp học nào và chi tiết của lớp học đó.
* **Security**: Quản lý trình duyệt và lịch sử đăng nhập.

## III. Các bước thực hiện chi tiết

<details>

<summary>3.1 Xem danh sách và chi tiết học viên</summary>

{% stepper %}
{% step %}
**Truy cập Student List**

Từ thanh điều hướng bên trái, truy cập **User & Org Management** → chọn **Students**. Danh sách học viên hiển thị theo thời gian tạo giảm dần.

<figure><img src="../.gitbook/assets/image (1202).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm và lọc**

Sử dụng các bộ lọc phía trên bảng danh sách:

* **Search**: tìm theo Họ tên (Full name), Username, Email, Số điện thoại.
* **Gender** (Giới tính): chọn 1 trong các giá trị cho trước.
* **Status** (Trạng thái): chọn 1 trong các giá trị cho trước (Active / Block).
* **Sort by**: sắp xếp theo Họ tên.
* **From Date – To Date**: lọc theo ngày cập nhật thông tin.

Nhấn **Search** để hiển thị kết quả. Nhấn **Reset** để xóa toàn bộ bộ lọc.

<figure><img src="../.gitbook/assets/image (1203).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin chi tiết học viên**

Nhấn vào tên tài khoản học viên hoặc nhấn **Action → View Profile**.

<figure><img src="../.gitbook/assets/image (1204).png" alt=""><figcaption></figcaption></figure>

Màn hình Student Profile hiển thị các tab:

* _**Overview**_: Hiển thị Personal Information (các thông tin cá nhân của học viên), Account Information (Account type, HubSpot Contact ID, Username, Status, Test Account) và các Profile học viên.

<figure><img src="../.gitbook/assets/image (1205).png" alt=""><figcaption></figcaption></figure>

*   _**Setting**_: Hiển thị các thông tin:

    * **General Information**: Full name, Email, Phone number, CCCD, Major, University, Field of Work, Avatar, Account Type.
    * **CFA Information**: Các thông tin liên quan đến Level kiểm tra tiếng Anh đầu vào, lịch đăng ký thi, kết quả bài thi CFA.
    * **ACCA Information**: Các thông tin liên quan đến Level kiểm tra tiếng Anh đầu vào, lịch đăng ký thi, kết quả bài thi ACCA.
    * **CMA Information**: Các thông tin liên quan đến Level kiểm tra tiếng Anh đầu vào, lịch đăng ký thi, kết quả bài thi CMA.

    <figure><img src="../.gitbook/assets/image (1206).png" alt=""><figcaption></figcaption></figure>
* _**Class and Course**_: Danh sách lớp và khóa học học viên đã đăng ký. Có thể tìm kiếm lớp học theo Code, Course (Khóa học), Program (Chương trình học), Status (Trạng thái học tập).

<figure><img src="../.gitbook/assets/image (1207).png" alt=""><figcaption></figcaption></figure>

* _**Security**_: Quản lý trình duyệt đã đăng nhập (tối đa 3 trình duyệt), lịch sử đăng nhập gần đây.

<figure><img src="../.gitbook/assets/image (1208).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xuất danh sách ra Excel (nếu cần)**

Tại màn hình Student List, nhấn **Export**. Hệ thống xuất danh sách học viên (theo điều kiện tìm kiếm hiện tại) thành file Excel và tự động tải về thiết bị.

<figure><img src="../.gitbook/assets/image (1209).png" alt=""><figcaption></figcaption></figure>

Các trường thông tin được trích xuất ra file Excel bao gồm: ID, Full name, Username, Email, Phone, Type User, Status.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.2 Tạo tài khoản học viên</summary>

{% stepper %}
{% step %}
**Truy cập màn hình tạo tài khoản**

Truy cập **User & Org Management**. Tại màn hình Student List, nhấn nút **Create** để chuyển đến màn hình **Create Student**.

<figure><img src="../.gitbook/assets/image (1210).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền thông tin học viên**

<figure><img src="../.gitbook/assets/image (1211).png" alt=""><figcaption></figcaption></figure>

Điền các trường thông tin. Các trường có dấu **(\*)** là bắt buộc:

* **Avatar**: tải ảnh đại diện từ thiết bị.
* **Account Type**:
  * _Employee Account_: Dành cho nhân viên nội bộ SAPP. Code = mã nhân viên. Dùng để xem trước dữ liệu khóa học, bài test mà không ảnh hưởng dữ liệu.
  * _Student Account_: Dành cho học viên đăng ký khóa học tại SAPP. Code = Record ID Contract trên HubSpot.
* **Full Name (\*)**: tối đa 100 ký tự.
* **Code**: mã nhân viên (với Employee Account) hoặc Record ID HubSpot (với Student Account).
* **Username (\*)**: 6–40 ký tự, không chứa khoảng trắng, không ký tự tiếng Việt có dấu và ký tự đặc biệt, không trùng.
* **Email (\*)**: đúng định dạng, không trùng email đã tồn tại.
* **Password / Confirm Password (\*)**: theo điều kiện hệ thống.
* **Phone number (\*)**: 10–11 số, bắt đầu bằng 0, không trùng SĐT đã tồn tại.
* **Gender**: chọn 1 giá trị.
* **Entrance Level**: chọn 1 giá trị (cấp độ đầu vào).
* **Test Account**: Yes (tài khoản test cho nhân viên SAPP) / No (học viên bình thường).
* **CFA Level**: Level test đầu vào tiếng Anh của chương trình CFA.
* **CMA Level**: Level test đầu vào tiếng Anh của chương trình CMA.
* **ACCA Level**: Level test đầu vào tiếng Anh của chương trình ACCA.
{% endstep %}

{% step %}
**Lưu tài khoản**

Nhấn ![](<../.gitbook/assets/image (1212).png>) để lưu thông tin.
{% endstep %}

{% step %}
**Xác nhận**

<figure><img src="../.gitbook/assets/image (1213).png" alt=""><figcaption></figcaption></figure>

Khi hộp thoại xác nhận hiển thị, chọn **Yes** để đồng ý. Hệ thống chuyển về Student List, tài khoản mới xuất hiện ở đầu danh sách.

✅ Kết quả: Tài khoản học viên được tạo thành công.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.3 Chỉnh sửa thông tin học viên (Edit Student)</summary>

{% stepper %}
{% step %}
**Truy cập màn hình chỉnh sửa**

Có 3 cách truy cập màn hình chỉnh sửa thông tin học viên:

* **Cách 1**: Tại Student List → nhấn **Action** → chọn **Edit**.

<figure><img src="../.gitbook/assets/image (1214).png" alt=""><figcaption></figcaption></figure>

* **Cách 2**: Nhấn vào tên học viên → chọn **Edit Profile**.

<figure><img src="../.gitbook/assets/image (1215).png" alt=""><figcaption></figcaption></figure>

* **Cách 3**: Nhấn vào tên học viên → chọn tab **Setting**.

<figure><img src="../.gitbook/assets/image (1216).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin**

**📑 Chỉnh sửa thông tin General Information**

<figure><img src="../.gitbook/assets/image (1217).png" alt=""><figcaption></figcaption></figure>

Các trường **có thể** chỉnh sửa:

* **Avatar**: Upload/chỉnh sửa ảnh đại diện tài khoản.
* **Gender**: Chọn 1 giá trị từ danh sách hệ thống cung cấp.
* **Date of Birth**: Chọn ngày từ date picker, theo định dạng ngày của hệ thống.
* **CCCD/CMND**: Upload hình ảnh CCCD/CMND mặt trước và mặt sau. Hỗ trợ thay đổi/cập nhật ảnh.
* **Major**: Chọn 1 giá trị từ danh sách định nghĩa sẵn.
* **University**: Chọn 1 giá trị từ danh sách định nghĩa sẵn.
* **Address**: Nhập text tự do theo nhu cầu nghiệp vụ.
* **Field of Work**: Chọn 1 giá trị từ danh sách định nghĩa sẵn.
* **Account Type**: Chọn Employee Account hoặc Student Account.
* **Employee Code**: Nhập mã nhân viên theo chuẩn nội bộ doanh nghiệp.
* **HubSpot Contact ID**: Không cập nhật thủ công. Giá trị được đồng bộ từ HubSpot. Nhấn nút để cập nhật HubSpot ID.
* **Status**: Chọn Active (tài khoản hoạt động) hoặc Block (tài khoản bị khóa, không thể đăng nhập).
* **Test Account**: Chọn Yes (tài khoản nhân viên SAPP/test account) hoặc No (tài khoản học viên thông thường).

Các trường **KHÔNG** được phép chỉnh sửa:

* **Fullname (\*)**: định danh duy nhất, không thay đổi sau khi tạo.
* **Phone (\*)**: định danh duy nhất, không thay đổi sau khi tạo.

Các trường có **quy trình riêng**:

* **Email (\*)**: Người dùng không thể tự chỉnh sửa email tại Setting profile. Để edit email, người dùng cần có quyền Edit student. Xem hướng dẫn chỉnh sửa email [tại đây](https://sapp-academy.gitbook.io/sapp-academy/~/revisions/jJXeizmPeI0YOMZR7XZI/nguoi-dung-user-management/pages/kilkVFJKJHZcpGjzHenO#id-3.4-edit-email).

**📑 Chỉnh sửa thông tin liên quan Chương trình học**

<figure><img src="../.gitbook/assets/image (900).png" alt=""><figcaption></figcaption></figure>

Các thông tin **có thể** chỉnh sửa:

* Account ID.
* \[Chương trình] Level: Chọn từ dropdown.
* \[Môn học] Exam: Chọn lịch thi từ dropdown.

Các thông tin **KHÔNG** được chỉnh sửa:

* \[Môn học] Result: Kết quả thi.
{% endstep %}

{% step %}
**Lưu thay đổi**

<figure><img src="../.gitbook/assets/image (1219).png" alt=""><figcaption></figcaption></figure>

Nhấn **Save Changes** → chọn **Yes, save** khi hộp thoại xác nhận hiển thị.

✅ Kết quả: Thông tin học viên được cập nhật thành công.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.4 Trạng thái học viên</summary>

Hệ thống hỗ trợ 2 trạng thái tài khoản học viên:

| Trạng thái | Mô tả                                                           |
| ---------- | --------------------------------------------------------------- |
| Active     | Tài khoản đang được kích hoạt, có thể đăng nhập vào LMS Student |
| Block      | Tài khoản bị khóa, không thể đăng nhập vào LMS Student          |

Có 3 cách thay đổi trạng thái:

{% stepper %}
{% step %}
**Cách 1 – Thay đổi qua nút Action**

Tại Student List, nhấn **Action** tương ứng với học viên cần đổi trạng thái → chọn **Block** (áp dụng cho tài khoản đang Active) → Xác nhận thay đổi trạng thái.

<figure><img src="../.gitbook/assets/image (1220).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cách 2 – Thay đổi qua cột Status trong bảng danh sách**

Tại Student List, nhấn chuyển **Status** tương ứng với học viên cần đổi trạng thái tại cột thông tin Status → chọn **Block** (áp dụng cho tài khoản đang Active) / chọn **Active** (áp dụng cho tài khoản đang Block) → Xác nhận thay đổi trạng thái.

<figure><img src="../.gitbook/assets/image (1221).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cách 3 – Thay đổi qua trường Status trong Student Profile**

Nhấn trực tiếp vào giá trị trường **Status** trên trang Student Profile → Setting → chọn giá trị mới (Active / Block) để chuyển đổi trạng thái.

<figure><img src="../.gitbook/assets/image (1222).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Khi học viên bị **Block**, hệ thống sẽ tự động đăng xuất tất cả thiết bị đang đăng nhập của học viên đó.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3.5 Import hàng loạt học viên</summary>

{% stepper %}
{% step %}
**Truy cập Student List và mở hộp thoại Import**

Tại Student List, nhấn nút **Import** để hiển thị hộp thoại tải file.

<figure><img src="../.gitbook/assets/image (1223).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn file và kiểm tra định dạng**

Chọn **Browse** để chọn file từ thiết bị (chỉ chấp nhận **.csv** hoặc **.xlsx**). Mỗi lần chỉ được chọn 1 file.

<figure><img src="../.gitbook/assets/image (910).png" alt=""><figcaption></figcaption></figure>

Người dùng có thể tải file mẫu về để tham khảo cách điền các thông tin hợp lệ. Các trường bắt buộc trong file bao gồm:

| Trường        | Điều kiện                                                                                                                                      |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Username      | 6–40 ký tự, không chứa khoảng trắng, không chứa ký tự tiếng Việt có dấu và ký tự đặc biệt (ngoại trừ . - \_), không trùng username đã tồn tại. |
| Email         | Đúng định dạng abc@abc.abc, không trùng email đã tồn tại.                                                                                      |
| Phone         | 10–11 ký tự số, bắt đầu bằng 0, không trùng SĐT đã tồn tại.                                                                                    |
| Full Name     | Họ và tên đầy đủ của học viên.                                                                                                                 |
| Status        | Active hoặc Block.                                                                                                                             |
| Testing Staff | Yes hoặc No — xác định tài khoản test của nội bộ.                                                                                              |
| Type User     | Employee hoặc Student — xác định loại User.                                                                                                    |
{% endstep %}

{% step %}
**Click "Import" để tải file lên hệ thống**

<figure><img src="../.gitbook/assets/image (911).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Kiểm tra kết quả Import qua hộp thoại thông báo**

Hộp thoại hiển thị trạng thái tạo tài khoản:

* **Source**: tên file đã tải lên.
* **Data**: số lượng bản ghi trong file.
* **Successfully**: số tài khoản học viên được tạo thành công.
* **Error**: số tài khoản học viên tạo thất bại.

Nhấp vào **View Log** để xem chi tiết tình trạng tạo tài khoản. Những trường không hợp lệ sẽ được bôi đỏ, kèm lỗi cụ thể tại cột **Errors**.

<figure><img src="../.gitbook/assets/image (912).png" alt=""><figcaption></figcaption></figure>

View log sẽ hiển thị như sau:

<figure><img src="../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

## IV. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Fullname KHÔNG được phép chỉnh sửa** sau khi tạo tài khoản.
2. Người có quyền Edit thông tin Students/Teachers/Staffs có quyền **Thay đổi Email** — yêu cầu xác thực OTP gửi về email cũ, cần đảm bảo email cũ còn hoạt động.
3. Tài khoản học viên bị **Block** sẽ không thể đăng nhập vào LMS Student.
4. Mỗi học viên chỉ được phép đăng nhập tối đa **3 thiết bị**. Nếu vượt quá, học viên cần liên hệ Ops để xóa thiết bị tại tab Security.
5. File Import chỉ chấp nhận định dạng **.csv** hoặc **.xlsx**; mỗi lần chỉ import 1 file.
6. Các trường Username, Email, SĐT trong file import phải là duy nhất, không trùng dữ liệu đã có trong hệ thống.
7. Học viên thuộc Account Type **Student Account** cần có Record ID HubSpot để đồng bộ Contact.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Tải file mẫu (template) trước khi import để đảm bảo đúng định dạng cột và dữ liệu.
2. Dùng **View Log** sau import để kiểm tra chi tiết lỗi và sửa từng bản ghi lỗi trước khi import lại.
3. Kết hợp nhiều bộ lọc (Search + Status + Gender + Date) để thu hẹp kết quả tìm kiếm nhanh hơn.
4. Sắp xếp danh sách theo cột Họ tên (Sort by) khi cần tìm kiếm thủ công.
5. Trước khi tạo tài khoản mới, dùng Search để kiểm tra học viên đã tồn tại hay chưa, tránh trùng dữ liệu.
{% endhint %}

## V. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                           | Nguyên nhân                                            | Cách xử lý                                                                                                |
| ------------------------------------------ | ------------------------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| Không tìm thấy học viên trong danh sách    | Bộ lọc quá chặt hoặc nhập sai từ khóa                  | Nhấn **Reset** để xóa toàn bộ bộ lọc, thử lại với từ khóa khác.                                           |
| Không thể lưu tài khoản mới                | Thiếu trường bắt buộc (\*) hoặc dữ liệu không hợp lệ   | Kiểm tra các trường có dấu (\*), đảm bảo Username/Email/SĐT chưa tồn tại trong hệ thống.                  |
| Username/Email/SĐT đã tồn tại              | Trùng dữ liệu với tài khoản đã có                      | Search trước để xác nhận tài khoản đã có hay chưa. Nếu cần, dùng giá trị khác hoặc xử lý tài khoản trùng. |
| File import bị lỗi một số dòng             | Dữ liệu các cột không đúng định dạng yêu cầu           | Nhấn **View Log** để xem chi tiết dòng lỗi, sửa file theo hướng dẫn tại cột **Errors** và import lại.     |
| File import không tải được                 | Định dạng file không phải .csv/.xlsx hoặc file quá lớn | Kiểm tra lại định dạng file. Tách nhỏ file nếu quá lớn và import từng lần.                                |
| Học viên không đăng nhập được thiết bị mới | Đã đăng nhập đủ 3 thiết bị                             | Vào Student Profile → tab **Security** → xóa bớt thiết bị cũ.                                             |
| Học viên bị Block báo không đăng nhập được | Tài khoản đã bị khóa trên hệ thống OPS                 | Vào Student Profile, đổi trạng thái về **Active** (nếu được phép) hoặc xác nhận với Admin lý do Block.    |
| Danh sách không tải được                   | Mất kết nối hoặc lỗi server                            | Tải lại trang (F5). Nếu vẫn lỗi, liên hệ IT để hỗ trợ.                                                    |

## VI. Câu hỏi thường gặp

<details>

<summary>Q: Tôi không thấy tài khoản học viên cần tìm dù đã tìm kiếm?</summary>

A: Kiểm tra lại bộ lọc đang áp dụng — nhấn **Reset** để xóa tất cả bộ lọc và tìm lại. Lưu ý ô Search cần nhập đủ từ. Nếu vẫn không thấy, tài khoản có thể không thuộc phạm vi quyền xem của bạn — liên hệ Admin.

</details>

<details>

<summary>Q: Tại sao tôi không chỉnh sửa được Fullname và Email của học viên?</summary>

A: Đây là quy tắc nghiệp vụ để đảm bảo tính nhất quán dữ liệu. Để chỉnh sửa Email, có thể liên hệ tới Admin.

</details>

<details>

<summary>Q: File import của tôi có nhiều dòng lỗi, tôi cần làm gì?</summary>

A: Sau khi import, nhấn **View Log** để xem chi tiết các dòng lỗi. Mở lại file gốc, sửa các dòng bị bôi đỏ theo hướng dẫn tại cột **Errors**, sau đó import lại file đã sửa.

</details>

<details>

<summary>Q: Học viên bị Block có thể tự kích hoạt lại tài khoản không?</summary>

A: Không. Chỉ người dùng có quyền trên hệ thống OPS (Admin / Operator có quyền) mới có thể thay đổi trạng thái từ Block về Active.

</details>

<details>

<summary>Q: Sự khác biệt giữa Employee Account và Student Account là gì?</summary>

A: Employee Account dùng cho nhân viên nội bộ SAPP (cần điền mã nhân viên ở trường Code). Student Account dùng cho học viên đăng ký khóa học thực tế (cần điền Record ID HubSpot để đồng bộ Contact).

</details>

<details>

<summary>Q: Học viên đăng nhập tối đa bao nhiêu thiết bị?</summary>

A: Tối đa 3 thiết bị. Khi vượt quá, học viên cần liên hệ Ops để xóa bớt thiết bị tại tab Security trong Student Profile.

</details>
