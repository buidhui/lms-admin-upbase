# Quản lý nhân viên (Staff)

Tài liệu hướng dẫn quản lý toàn bộ tài khoản Nhân viên trong hệ thống OPS

## Record of Changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| 28 May 2026    | Lê Thị Huế    | M     | Chuẩn hóa nội dung lên Gitbook | 4.2.0   |

### Definitions and Acronyms

| # | Term       | Definition                                               |
| - | ---------- | -------------------------------------------------------- |
| 1 | OPS        | Operations — Hệ thống quản lý vận hành                   |
| 2 | LMS        | Learning Management System — Hệ thống quản lý học tập    |
| 3 | OTP        | One-Time Password — Mã xác thực một lần                  |
| 4 | Import Log | Lịch sử file đã import, hiển thị trạng thái từng bản ghi |

## I. Thông tin chung

**Dành cho:** Admin, Operator

**Đường dẫn:** User & Org Management → Staffs → Staff List

#### Phạm vi & Module liên quan

* **Module chính:** Staff Management (thuộc User Management)
* **Module liên quan:** Department, Title, Role Management

#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống OPS.
* Đã đăng nhập thành công vào hệ thống.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện (xem / tạo / chỉnh sửa / import).
* Đã nắm rõ cấu trúc Phòng ban (Department), Chức danh (Title), Cấp bậc (Level), Chương trình (Program) và Role hiện có trong hệ thống.

## II. Tổng Quan Giao Diện

Màn hình **Staff Management** bao gồm các khu vực chính:

* **Thanh điều hướng trái:** User & Org Management → Staffs → Staff List
* **Thanh tìm kiếm & bộ lọc:** Search (Họ tên / Username / Email / SĐT), Status, Role (đa lựa chọn), Sort by, Gender, From Date – To Date
* **Bảng danh sách:** Hiển thị danh sách nhân viên theo thời gian tạo giảm dần, kèm Phòng ban / Chức danh / Trạng thái
* **Nút thao tác (Action):** View Profile, Edit, Reset Password, Edit Email, Block
* **Nút chức năng chính:** Create (tạo mới), Import (nhập hàng loạt), Export (xuất Excel)

#### Đối tượng áp dụng

| Đối tượng | Vai trò            | Quyền hạn                                                                  |
| --------- | ------------------ | -------------------------------------------------------------------------- |
| Admin     | Quản trị hệ thống  | Toàn quyền — xem, tạo, chỉnh sửa, đổi trạng thái, import, export, gán Role |
| Operator  | Nhân viên vận hành | Tùy theo Role được cấp trong hệ thống (xem / tạo / chỉnh sửa / import)     |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Quản lý Phòng ban (Department)

Hệ thống tổ chức tài khoản nhân viên theo các cấp bậc phòng ban:

**Board > Block > Division > Department > Sub-department**

#### 3.1.1 Xem danh sách phòng ban

🎯 Mục tiêu: Xem toàn bộ danh sách phòng ban và số nhân viên thuộc phòng ban đó theo cấp bậc.

{% stepper %}
{% step %}
## Truy cập Department

Từ thanh điều hướng bên trái, chọn **User & Org Management** → chọn **Departments**. Danh sách bộ phận hiển thị dưới dạng cấp bậc phòng ban.

![](<.gitbook/assets/image (69)>)

Có thể rút gọn nếu không muốn xem chi tiết, chọn ![](<.gitbook/assets/image (70)>):

![](<.gitbook/assets/image (71)>)
{% endstep %}
{% endstepper %}

#### 3.1.2 Xem chi tiết phòng ban

🎯 Mục tiêu: Xem chi tiết thông tin của một phòng ban.

{% stepper %}
{% step %}
## Chọn tên phòng ban muốn xem chi tiết

Tại danh sách phòng ban, chọn tên phòng ban muốn xem chi tiết.

![](<.gitbook/assets/image (72)>)

✅ Kết quả: Thông tin chi tiết của phòng ban sẽ hiển thị. Người dùng có thể chỉnh sửa thông tin phòng ban đó.

![](<.gitbook/assets/image (73)>)
{% endstep %}
{% endstepper %}

#### 3.1.3 Chỉnh sửa thông tin phòng ban

🎯 Mục tiêu: Chỉnh sửa các thông tin chi tiết của một phòng ban cụ thể.

{% stepper %}
{% step %}
## Truy cập trang Edit Department

Có 3 cách truy cập chỉnh sửa phòng ban:

**Cách 1:** Tại Department List chọn **Action** → **Edit** phòng ban cần chỉnh sửa:

![](<.gitbook/assets/image (74)>)

**Cách 2:** Truy cập Department Detail → chọn **Edit Department**:

![](<.gitbook/assets/image (75)>)

**Cách 3:** Truy cập Department Detail → chọn **Setting**:

![](<.gitbook/assets/image (76)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin Department

Cho phép chỉnh sửa các thông tin sau (\*: trường bắt buộc):

* **Department Name** (\*): Tên bộ phận
* **Department Short Name** (\*): Tên rút gọn
* **Department Level:** Cấp bậc — Board > Block > Division > Department > Sub-department
* **Department Parent** (\*): Phòng ban cha của nó
* **Unit** (\*): Đơn vị kinh doanh
* **Description:** Mô tả phòng ban

![](<.gitbook/assets/image (77)>)
{% endstep %}

{% step %}
## Nhấn lưu và xác nhận thông tin

Nhấn ![](<.gitbook/assets/image (78)>) và xác nhận lưu thông tin.

![](<.gitbook/assets/image (79)>)

✅ Kết quả: Thông tin phòng ban được cập nhật thành công.
{% endstep %}
{% endstepper %}

#### 3.1.5 Tạo mới phòng ban

🎯 Mục tiêu: Tạo mới phòng ban trên hệ thống.

{% stepper %}
{% step %}
## Truy cập Create Department

Truy cập danh mục **Department**, tại Department List chọn **Create Department**.

![](<.gitbook/assets/image (80)>)
{% endstep %}

{% step %}
## Nhập thông tin phòng ban

* **Department Name** (\*): nhập tên đầy đủ
* **Department Short Name:** nhập tên rút gọn (tùy chọn)
* **Department Level** (\*): chọn cấp bậc từ dropdown
* **Department Parent** (\*): chọn phòng ban cấp trên từ dropdown
* **Unit** (\*): chọn đơn vị kinh doanh từ dropdown
* **Description:** nhập mô tả (tùy chọn)

![](<.gitbook/assets/image (81)>)
{% endstep %}

{% step %}
## Nhấn Submit và xác nhận để lưu thông tin

Người dùng chọn ![](<.gitbook/assets/image (82)>) để hoàn tất lưu thông tin.

✅ Kết quả: Thông tin phòng ban mới sẽ được tạo, hệ thống hiển thị thông báo

![](<.gitbook/assets/image (83)>)
{% endstep %}
{% endstepper %}

#### 3.1.6 Xóa phòng ban

Cho phép xóa phòng ban khi không có phòng ban con nào thuộc nó và không có staff, role nào gắn với phòng ban đó.

{% stepper %}
{% step %}
## Truy cập Department List → chọn Action → Delete

![](<.gitbook/assets/image (84)>)
{% endstep %}

{% step %}
## Xác nhận xóa

![](<.gitbook/assets/image (85)>)

✅ Kết quả: Hệ thống xóa thành công phòng ban và hiển thị
{% endstep %}
{% endstepper %}

### 3.2 Quản lý Chức danh (Title)

#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống Ops.
* Người dùng được cấp quyền tương ứng (xem / tạo / chỉnh sửa chức danh).

#### 3.2.1 Xem danh sách chức danh (Title List)

🎯 Mục tiêu: Truy cập và xem toàn bộ danh sách chức danh hiện có trong hệ thống.

{% stepper %}
{% step %}
## Truy cập màn hình Title List

Từ menu điều hướng bên trái, chọn: **User & Org Management** → **Title List**.

![](<.gitbook/assets/image (86)>)

Màn hình Title List gồm các khu vực chính:

* **Thanh tìm kiếm:** Tìm theo Name hoặc Code.
* **Bộ lọc (Filter):** Department Level, Department, Status, From Date – To Date.
* **Nút Create:** Mở màn hình tạo mới chức danh.
* **Nút Import:** Nhập danh sách chức danh từ file.
* **Bảng danh sách:** Hiển thị danh sách chức danh với các cột #, Name, Code, Department, Status, Description, Date, Action.

Các trường thông tin trong danh sách:

| Trường      | Kiểu dữ liệu      | Mô tả                                   |
| ----------- | ----------------- | --------------------------------------- |
| Name        | Text              | Tên chức danh                           |
| Code        | Text              | Mã chức danh                            |
| Department  | Label             | Phòng ban sử dụng chức danh             |
| Status      | Label             | Trạng thái hoạt động: Active / Inactive |
| Description | Text Area         | Mô tả chức danh                         |
| Date        | Date (DD/MM/YYYY) | Ngày tạo và ngày chỉnh sửa gần nhất     |
{% endstep %}

{% step %}
## Tìm kiếm chức danh (nếu cần)

* Nhập từ khoá vào ô **Search** để tìm theo Name hoặc Code.
* Sử dụng bộ lọc **Filter** để thu hẹp kết quả theo Department Level, Department, Status hoặc khoảng thời gian From Date – To Date.
* Nhấn **Search** để áp dụng điều kiện lọc. Nhấn **Reset** để xóa bộ lọc.

![](<.gitbook/assets/image (87)>)

✅ Kết quả:

Danh sách chức danh hiển thị theo bảng với các thông tin: Name, Code, Department, Status, Description, Date.

Click trực tiếp vào Name để mở màn hình chỉnh sửa, hoặc chọn icon Action (⋮) ở cuối dòng để xem thêm thao tác.
{% endstep %}
{% endstepper %}

#### 3.2.2 Tạo mới chức danh (Create Title)

🎯 Mục tiêu: Thêm một chức danh mới vào hệ thống.

{% stepper %}
{% step %}
## Truy cập màn hình tạo mới

Tại màn hình Title List, nhấn nút **Create** (góc phải phía trên).

![](<.gitbook/assets/image (88)>)
{% endstep %}

{% step %}
## Nhập thông tin chức danh

![](<.gitbook/assets/image (89)>)

Điền đầy đủ các trường thông tin:

| Trường      | Kiểu dữ liệu | Bắt buộc | Mô tả                                                                            |
| ----------- | ------------ | -------- | -------------------------------------------------------------------------------- |
| Name        | Text         | Có       | Tên chức danh. Cho phép chữ hoa, thường, số và ký tự đặc biệt, tối đa 100 ký tự. |
| Code        | Text         | Có       | Mã chức danh.                                                                    |
| Department  | Combo box    | Có       | Chọn phòng ban áp dụng chức danh. Có thể chọn nhiều phòng ban.                   |
| Description | Text Area    | Không    | Mô tả chi tiết về chức danh.                                                     |
{% endstep %}

{% step %}
## Chọn hành động lưu

* **Save:** Lưu chức danh vừa tạo và quay về danh sách.
* **Save & New:** Lưu và mở form tạo mới tiếp theo.
* **Cancel:** Hủy thao tác. Hệ thống hiển thị popup xác nhận.

✅ Kết quả: Sau khi tạo thành công, chức danh mới có Status mặc định là **Active**.
{% endstep %}
{% endstepper %}

#### 3.2.3 Chỉnh sửa chức danh (Edit Title)

🎯 Mục tiêu: Cập nhật thông tin chức danh đã có trong hệ thống.

{% stepper %}
{% step %}
## Truy cập màn hình chỉnh sửa

**Cách 1:** Tại màn hình Title List, click trực tiếp vào **Name** của chức danh cần chỉnh sửa.

![](<.gitbook/assets/image (90)>)

**Cách 2:** Tại dòng chức danh, chọn icon **Action (⋮)** → **Edit**.

![](<.gitbook/assets/image (91)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin

![](<.gitbook/assets/image (92)>)

Cập nhật các trường thông tin theo nhu cầu:

| Trường      | Bắt buộc | Mô tả                                                               |
| ----------- | -------- | ------------------------------------------------------------------- |
| Name        | Có       | Tên chức danh.                                                      |
| Code        | Có       | Mã chức danh. Bị khóa nếu Title đã được gán cho Staff.              |
| Department  | Có       | Có thể chọn nhiều phòng ban. Các department đã có staff sẽ bị khóa. |
| Status      | Có       | Active / Inactive.                                                  |
| Description | Không    | Mô tả chi tiết.                                                     |
{% endstep %}

{% step %}
## Lưu chỉnh sửa

Nhấn nút **Save** để lưu thay đổi vào hệ thống.

✅ Kết quả: Thay đổi thông tin Title thành công.
{% endstep %}
{% endstepper %}

#### 3.2.4 Thay đổi trạng thái chức danh (Status)

Người dùng có thể thay đổi trạng thái chức danh trực tiếp từ màn hình Edit hoặc từ danh sách:

* **Active → Inactive:** Vô hiệu hóa chức danh. Chức danh sẽ không xuất hiện trong các lựa chọn mới.
* **Inactive → Active:** Kích hoạt lại chức danh.

{% stepper %}
{% step %}
## Truy cập Title List, cập nhật thông tin tại cột Status

![](<.gitbook/assets/image (93)>)
{% endstep %}

{% step %}
## Xác nhận thay đổi trạng thái

![](<.gitbook/assets/image (94)>)

✅ Kết quả: Hệ thống cập nhật thành công trạng thái của chức danh.
{% endstep %}
{% endstepper %}

### 3.3 Quản lý Nhân viên (Staff)

#### 3.3.1 Xem danh sách nhân viên

🎯 Mục tiêu: Xem toàn bộ danh sách tài khoản nhân viên vận hành trong hệ thống và tìm kiếm thông tin nhân viên cụ thể.

{% stepper %}
{% step %}
## Truy cập Staff List

Từ thanh điều hướng bên trái, nhấn **User & Org Management** → chọn **Staff**. Danh sách nhân viên hiển thị theo thời gian tạo giảm dần.

![](<.gitbook/assets/image (95)>)
{% endstep %}

{% step %}
## Tìm kiếm và lọc

![](<.gitbook/assets/image (96)>)

Sử dụng các bộ lọc phía trên bảng danh sách:

* **Search:** tìm theo Họ tên (Full name), Username, Email, Số điện thoại — cần nhập đủ từ.
* **Status:** chọn Active / Block.
* **Role:** chọn nhóm vai trò.
* **Sort by:** sắp xếp theo Họ tên.
* **Gender:** chọn giới tính.
* **From Date – To Date:** lọc theo ngày cập nhật thông tin.

Nhấn ![](<.gitbook/assets/image (97)>) để áp dụng. Nhấn ![](<.gitbook/assets/image (98)>) để xóa toàn bộ bộ lọc.
{% endstep %}

{% step %}
## Xem thông tin chi tiết nhân viên

Có 2 cách truy cập thông tin chi tiết nhân viên:

**Cách 1:** Từ **List Staffs** chọn **Action** → **View Profile**:

![](<.gitbook/assets/image (99)>)

**Cách 2:** Nhấn trực tiếp vào tên Staff:

![](<.gitbook/assets/image (100)>)

Màn hình **Staff Profile** hiển thị các thông tin Overview:

* Mã nhân viên, Hubspot ID, Họ tên, Username, Email, Số điện thoại,
* Phòng ban, Chức vụ
* Chương trình
* Role
* Trạng thái, Giới tính
* Thời gian cập nhật.

![](<.gitbook/assets/image (101)>)
{% endstep %}

{% step %}
## Xuất danh sách ra Excel

![](<.gitbook/assets/image (102)>)

Tại Staff List, nhấn **Export**. Hệ thống xuất danh sách nhân viên (theo điều kiện tìm kiếm hiện tại) thành file Excel và tự động tải về thiết bị.

✅ Kết quả: Danh sách nhân viên hiển thị đúng theo điều kiện tìm kiếm. Người dùng có thể xem chi tiết, chỉnh sửa hoặc xuất dữ liệu.
{% endstep %}
{% endstepper %}

#### 3.3.2 Tạo tài khoản nhân viên

🎯 Mục tiêu: Tạo mới một tài khoản nhân viên vận hành trong hệ thống OPS.

{% stepper %}
{% step %}
## Truy cập màn hình tạo tài khoản

Tại Staff List, nhấn nút **Create** để mở màn hình Create Staff.

![](<.gitbook/assets/image (103)>)
{% endstep %}

{% step %}
## Điền thông tin nhân viên

![](<.gitbook/assets/image (104)>)

Điền các trường thông tin. Các trường có dấu **(\*)** là bắt buộc:

* **Avatar:** tải ảnh đại diện từ thiết bị.
* **Full Name** (\*): tối đa 100 ký tự.
* **Username** (\*): 6–40 ký tự, không trùng.
* **Email** (\*): đúng định dạng, không trùng email đã tồn tại.
* **Hubspot contact ID:** Thông tin ID contact được đồng bộ với Hubspot.
* **Password / Confirm Password** (\*): theo điều kiện hệ thống.
* **Phone number** (\*): nhập theo điều kiện trên màn hình, không trùng SĐT đã tồn tại.
* **Department:** chọn 1 giá trị trong các phòng ban được cấu hình.
* **Program:** chọn chương trình phụ trách — bắt buộc nếu phòng ban khác 'HO', không bắt buộc nếu phòng ban là 'HO'.
* **Role:** được phép chọn nhiều quyền cho cùng 1 nhân viên.
* **Gender** (\*): chọn 1 giá trị.
{% endstep %}

{% step %}
## Lưu tài khoản

Nhấn **Save** tại góc phải màn hình → chọn **Yes** khi hộp thoại xác nhận hiển thị.

![](<.gitbook/assets/image (105)>)

✅ Kết quả: Tài khoản nhân viên được tạo thành công và xuất hiện ở đầu danh sách Staff List.
{% endstep %}
{% endstepper %}

#### 3.3.3 Chỉnh sửa thông tin nhân viên

🎯 Mục tiêu: Cập nhật thông tin cơ bản, tổ chức và phân quyền của tài khoản nhân viên đã có.

{% stepper %}
{% step %}
## Truy cập màn hình chỉnh sửa

Có 3 cách truy cập màn hình chỉnh sửa thông tin nhân viên:

**Cách 1:** Tại Staff List → nhấn **Action** → chọn **Edit**:

![](<.gitbook/assets/image (106)>)

**Cách 2:** Nhấn vào tên nhân viên → chọn **Edit Profile**:

![](<.gitbook/assets/image (107)>)

**Cách 3:** Nhấn vào tên nhân viên → chọn tab **Setting**:

![](<.gitbook/assets/image (108)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin

![](<.gitbook/assets/image (109)>)

**Các trường có thể chỉnh sửa:** Avatar, Full Name (\*), Gender (\*), Department, Job Position (Title & Level — tối đa 2 vị trí), Program, Role, Status.

**Các trường KHÔNG được phép chỉnh sửa:**

* **Username** (\*) — định danh duy nhất, không thay đổi sau khi tạo.
* **Phone** (\*) — định danh duy nhất, không thay đổi sau khi tạo.

**Thay đổi Email** (có quy trình riêng — cần xác thực OTP):

Tại trang edit profile nhấn ![](<.gitbook/assets/image (110)>), hệ thống sẽ gửi OTP xác nhận đổi email vào tài khoản email gốc.

![](<.gitbook/assets/image (111)>)

Nhập tài khoản email mới và mã OTP (có hiệu lực trong 15 giây) được gửi về email gốc:

![](<.gitbook/assets/image (112)>)

Nhấn **Save** để hoàn tất chỉnh sửa email.

**Lưu ý khi chỉnh sửa Job Position:**

* Mỗi nhân viên tối thiểu 1, tối đa 2 Job Position.
* Dùng nút **Add job position** để thêm vị trí:

![](<.gitbook/assets/image (113)>)

* Dùng nút **Delete** để xóa bớt vị trí (chỉ xóa được khi còn nhiều hơn 1 Job Position):

![](<.gitbook/assets/image (114)>)
{% endstep %}

{% step %}
## Lưu thay đổi

Nhấn **Save Changes** để lưu thay đổi.

✅ Kết quả: Thông tin nhân viên được cập nhật thành công.

![](<.gitbook/assets/image (115)>)
{% endstep %}
{% endstepper %}

#### 3.3.4 Thay đổi trạng thái nhân viên

🎯 Mục tiêu: Thay đổi trạng thái hoạt động của tài khoản nhân viên (kích hoạt hoặc khóa tài khoản).

**Cách 1: Thay đổi từ màn hình List Staffs**

{% stepper %}
{% step %}
## Truy cập List Staffs

Tại Staff List, nhấn **Action** tương ứng với nhân viên cần đổi trạng thái → chọn **Block** (áp dụng cho tài khoản đang Active) hoặc **Active** (áp dụng cho tài khoản đang Block).

![](<.gitbook/assets/image (116)>)
{% endstep %}

{% step %}
## Xác nhận thay đổi trạng thái

Chọn **Yes** để cập nhật trạng thái thành công.

![](<.gitbook/assets/image (117)>)
{% endstep %}
{% endstepper %}

**Cách 2: Thay đổi qua Staff Profile**

{% stepper %}
{% step %}
## Truy cập Staff Profile

Nhấn trực tiếp vào giá trị trường **Status** trong bảng danh sách hoặc trên trang Staff Profile → chọn giá trị mới (Active / Block) để chuyển đổi trạng thái.

![](<.gitbook/assets/image (118)>)
{% endstep %}

{% step %}
## Nhấn "Save changes" để lưu trạng thái tài khoản

{% hint style="warning" %}
Khi nhân viên bị Block, các Role đã gán vẫn được giữ nguyên nhưng nhân viên không thể đăng nhập. Khi chuyển về Active, nhân viên có thể đăng nhập lại với các Role hiện có.
{% endhint %}

✅ Kết quả: Trạng thái tài khoản nhân viên được cập nhật thành công.
{% endstep %}
{% endstepper %}

#### 3.3.5 Import hàng loạt nhân viên

🎯 Mục tiêu: Tạo nhiều tài khoản nhân viên cùng lúc bằng cách tải lên file Excel/CSV.

{% stepper %}
{% step %}
## Mở hộp thoại Import

Tại màn hình Staff List, nhấn nút **Import** để hiển thị hộp thoại tải file.

![](<.gitbook/assets/image (119)>)
{% endstep %}

{% step %}
## Chọn file từ thiết bị

Chọn **Browse** để chọn file từ thiết bị (chỉ chấp nhận `.csv` hoặc `.xlsx`; mỗi lần chỉ được chọn 1 file). Người dùng có thể tải file mẫu về để tham khảo cách điền các thông tin hợp lệ.

![](<.gitbook/assets/image (120)>)

Các trường bắt buộc trong file Import:

| Trường        | Điều kiện                                                                                                                                      |
| ------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| Username      | 6–40 ký tự, không chứa khoảng trắng, không chứa ký tự tiếng Việt có dấu và ký tự đặc biệt (ngoại trừ . - \_), không trùng username đã tồn tại. |
| Email         | Đúng định dạng abc@abc.abc, không trùng email đã tồn tại.                                                                                      |
| Phone         | 10–11 ký tự số, bắt đầu bằng 0, không trùng SĐT đã tồn tại.                                                                                    |
| Full Name     | Họ và tên đầy đủ của nhân viên.                                                                                                                |
| Status        | Active hoặc Block.                                                                                                                             |
| Testing Staff | Xác định tài khoản test nội bộ: Yes hoặc No.                                                                                                   |
| Type User     | Xác định loại User: Employee hoặc Student.                                                                                                     |
{% endstep %}

{% step %}
## Click "Import" để tải file lên hệ thống

![](<.gitbook/assets/image (121)>)
{% endstep %}

{% step %}
## Kiểm tra kết quả Import

Hộp thoại hiển thị trạng thái tạo tài khoản:

* **Source:** tên file đã tải lên.
* **Data:** số lượng bản ghi trong file.
* **Successfully:** số tài khoản được tạo thành công.
* **Error:** số tài khoản tạo thất bại.

Nhấp vào **View Log** để xem chi tiết tình trạng tạo tài khoản. Những trường không hợp lệ sẽ được bôi đỏ, kèm lỗi cụ thể tại cột **'Errors'**.

![](<.gitbook/assets/image (122)>)

View log sẽ hiển thị như sau:

![](<.gitbook/assets/image (123)>)

✅ Kết quả: Tài khoản nhân viên hợp lệ được tạo thành công. Tài khoản lỗi được ghi nhận trong log để người dùng kiểm tra, sửa và import lại.

{% hint style="warning" %}
Sau khi import, các trường liên quan đến nội dung giảng dạy (Teaching Program, Primary Responsibility, Mức độ ưu tiên môn học) cần được bổ sung thủ công cho từng giảng viên qua màn hình Edit.
{% endhint %}
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. **Username** và **Số điện thoại** KHÔNG được phép chỉnh sửa sau khi tạo tài khoản — đây là định danh duy nhất của nhân viên.
2. Thay đổi **Email** yêu cầu xác thực OTP gửi về Email cũ — cần đảm bảo Email cũ còn hoạt động.
3. Tài khoản nhân viên bị **Block** sẽ không thể đăng nhập vào hệ thống OPS.
4. Mỗi nhân viên có tối thiểu **1**, tối đa **2 Job Position** (tổ hợp Title + Level).
5. Phòng ban khác **'HO'** BẮT BUỘC phải chọn Chương trình (Program); phòng ban 'HO' thì không bắt buộc.
6. Danh sách Title (chức danh) hiển thị phụ thuộc vào Department đã chọn — chọn Department trước, rồi mới chọn Title.
7. Mỗi nhân viên có thể được gán **nhiều Role** cùng lúc — Role quyết định quyền thao tác trong hệ thống.
8. File Import chỉ chấp nhận định dạng `.csv` hoặc `.xlsx`; mỗi lần chỉ import 1 file.
9. Các trường Username, Email, SĐT trong file import phải là duy nhất, không trùng dữ liệu đã có trong hệ thống.
10. Thông tin Department / Job Position / Program / Role không được nhập qua Import — phải bổ sung thủ công sau khi tạo tài khoản.

### Mẹo sử dụng

1. Tải file mẫu (template) trước khi import để đảm bảo đúng định dạng cột và dữ liệu.
2. Dùng **View Log** sau import để kiểm tra chi tiết lỗi và sửa từng bản ghi lỗi trước khi import lại.
3. Kết hợp nhiều bộ lọc (Search + Status + Role + Gender + Date) để thu hẹp kết quả tìm kiếm nhanh hơn.
4. Gán **Role** ngay sau khi tạo tài khoản để nhân viên có thể truy cập các chức năng cần thiết.
5. Khi cần điều chuyển nội bộ, dùng tính năng **Edit Job Position** thay vì tạo tài khoản mới.

## V. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                         | Nguyên nhân                                           | Cách xử lý                                                                                          |
| -------------------------------------------------------- | ----------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Không tìm thấy nhân viên trong danh sách                 | Bộ lọc quá chặt hoặc nhập sai từ khóa                 | Nhấn **Reset** để xóa toàn bộ bộ lọc, thử lại với từ khóa khác. Đảm bảo nhập đủ từ khi search.      |
| Không thể lưu tài khoản mới                              | Thiếu trường bắt buộc (\*) hoặc dữ liệu không hợp lệ  | Kiểm tra các trường có dấu (\*), đảm bảo Username/Email/SĐT chưa tồn tại trong hệ thống.            |
| Không chọn được Chức danh (Title)                        | Chưa chọn Phòng ban (Department)                      | Chọn Department trước, danh sách Title sẽ hiển thị tương ứng với phòng ban đã chọn.                 |
| Không lưu được tài khoản dù đã điền đủ thông tin         | Phòng ban khác 'HO' nhưng chưa chọn Chương trình      | Kiểm tra trường Program — nếu Department khác 'HO' thì bắt buộc phải chọn Chương trình.             |
| Không thêm được Job Position thứ 3                       | Vượt quá giới hạn                                     | Mỗi nhân viên tối đa 2 Job Position. Xóa bớt 1 vị trí trước khi thêm vị trí mới.                    |
| Không xóa được Job Position                              | Chỉ còn 1 Job Position duy nhất                       | Mỗi nhân viên phải có tối thiểu 1 Job Position. Thêm vị trí mới trước khi xóa vị trí cũ.            |
| File import bị lỗi một số dòng                           | Dữ liệu các cột không đúng định dạng yêu cầu          | Nhấn **View Log** để xem chi tiết dòng lỗi, sửa file theo hướng dẫn tại cột 'Errors' và import lại. |
| Nhân viên đăng nhập được nhưng không thấy menu/chức năng | Chưa được gán Role hoặc Role không có quyền tương ứng | Vào Staff Profile → Edit → gán Role phù hợp với công việc của nhân viên.                            |
| Nhân viên bị Block báo không đăng nhập được              | Tài khoản đã bị khóa trên hệ thống OPS                | Vào Staff Profile, đổi trạng thái về Active (nếu được phép) hoặc xác nhận với Admin lý do block.    |
| Danh sách không tải được                                 | Mất kết nối hoặc lỗi server                           | Tải lại trang (F5). Nếu vẫn lỗi, liên hệ IT để hỗ trợ.                                              |

## VI. Câu Hỏi Thường Gặp (FAQ)

<details>

<summary>Tôi không thấy tài khoản nhân viên cần tìm dù đã tìm kiếm?</summary>

Kiểm tra lại bộ lọc đang áp dụng — nhấn **Reset** để xóa tất cả bộ lọc và tìm lại. Lưu ý ô Search cần nhập đủ từ. Nếu vẫn không thấy, tài khoản có thể không thuộc phạm vi quyền xem của bạn — liên hệ Admin.

</details>

<details>

<summary>Tại sao tôi không chỉnh sửa được Username và Số điện thoại của nhân viên?</summary>

Đây là quy tắc nghiệp vụ để đảm bảo tính nhất quán dữ liệu. Username và SĐT là định danh duy nhất của tài khoản, không được phép thay đổi sau khi tạo. Nếu cần sửa, phải tạo tài khoản mới.

</details>

<details>

<summary>Một nhân viên có thể có mấy Job Position?</summary>

Tối thiểu 1 và tối đa 2 Job Position. Dùng nút **Add job position** để thêm vị trí và nút **Delete** để xóa bớt (chỉ xóa được khi còn nhiều hơn 1 vị trí).

</details>

<details>

<summary>Khi nào bắt buộc phải chọn Chương trình (Program)?</summary>

Khi Phòng ban (Department) khác 'HO' thì bắt buộc phải chọn Chương trình. Riêng phòng ban HO thì Chương trình là tùy chọn, không bắt buộc.

</details>

<details>

<summary>Một nhân viên có thể có mấy Role?</summary>

Không giới hạn. Một nhân viên có thể được gán nhiều Role cùng lúc tùy theo nhu cầu công việc. Hệ thống sẽ tổng hợp quyền từ tất cả Role được gán.

</details>

<details>

<summary>Tại sao danh sách Title thay đổi khi tôi chọn Department khác?</summary>

Vì Title (chức danh) được cấu hình theo từng Phòng ban. Mỗi phòng ban có một bộ chức danh riêng. Khi đổi Department, hệ thống tự động cập nhật lại danh sách Title tương ứng.

</details>

<details>

<summary>File import của tôi có nhiều dòng lỗi, tôi cần làm gì?</summary>

Sau khi import, nhấn **View Log** để xem chi tiết các dòng lỗi. Mở lại file gốc, sửa các dòng bị bôi đỏ theo hướng dẫn tại cột 'Errors', sau đó import lại file đã sửa. Bạn cũng có thể truy cập Staffs → Import Report để xem lại lịch sử.

</details>

<details>

<summary>Sau khi import, tại sao nhân viên không truy cập được hệ thống?</summary>

Import chỉ tạo thông tin tài khoản cơ bản (Username, Email, Phone, Full Name, Status). Các thông tin về Department, Job Position, Program và đặc biệt là **Role** cần được bổ sung thủ công qua màn hình Edit. Nhân viên chưa có Role sẽ không thấy được menu/chức năng trong OPS.

</details>

<details>

<summary>Nhân viên bị Block có thể tự kích hoạt lại tài khoản không?</summary>

Không. Chỉ người dùng có quyền trên hệ thống OPS (Admin / Operator có quyền) mới có thể thay đổi trạng thái từ Block về Active.

</details>

<details>

<summary>Tôi có thể xóa một chức danh không?</summary>

Hệ thống hiện không hỗ trợ xóa chức danh. Để vô hiệu hóa, hãy chuyển Status sang **Inactive**.

</details>

<details>

<summary>Tại sao tôi không thấy nút Create?</summary>

Bạn chưa được cấp quyền tạo mới chức danh. Liên hệ quản trị viên hệ thống để được cấp quyền.

</details>

<details>

<summary>Có thể gán một chức danh cho nhiều phòng ban không?</summary>

Có. Tại màn hình Edit, trường Department hỗ trợ **Multiple select** — bạn có thể chọn nhiều phòng ban cùng lúc.

</details>

<details>

<summary>Sau khi tạo mới, chức danh có trạng thái gì?</summary>

Sau khi tạo thành công, Status mặc định của chức danh là **Active**.

</details>
