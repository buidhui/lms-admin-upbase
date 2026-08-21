# Quản lý hồ sơ cá nhân (Profile)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| 26/05/2026     | Lê Thị Huế    | M     | Chuẩn hóa nội dung lên Gitbook | ….      |

### Definitions and Acronyms

| # | Term | Definition |
| - | ---- | ---------- |
| 1 | Ops  | Operations |

## I. Thông tin chung

**Dành cho:** Admin, Operator

**Đường dẫn:** https://ops.sapp.edu.vn/auth/login (truy cập hồ sơ qua avatar góc dưới bên trái → **My profile**)

### 1.1 Mục đích

Module **Hồ sơ cá nhân** cho phép người vận hành xem và chỉnh sửa thông tin chi tiết Hồ sơ cá nhân. Bao gồm: Thông tin Đăng nhập, Xem chi tiết hồ sơ cá nhân, Chỉnh sửa hồ sơ cá nhân, Thay đổi mật khẩu, Email.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò            | Quyền hạn                                     |
| --------- | ------------------ | --------------------------------------------- |
| Admin     | Quản trị hệ thống  | Toàn quyền — xem, tạo, chỉnh sửa, xóa, import |
| Operator  | Nhân viên vận hành | Tùy theo Role được cấp trong hệ thống         |

#### Phạm vi & Module liên quan

* **Module chính:** User Management (Students, Teachers, Staffs)
* **Module liên quan:** Course Management, Schedule Management, Import Report
* **Hệ thống tích hợp:** LMS Pro (giao diện học viên), HubSpot (Contact học viên)

#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống OPS.
* Đã đăng nhập thành công vào hệ thống.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện.

## II. Tổng Quan Giao Diện

Quản lý hồ sơ cá nhân bao gồm các khu vực chính:

* **Thanh điều hướng trái:** Truy cập các danh mục quản lý theo phân quyền.
* **Top main section:** Hiển thị thông tin cơ bản của người dùng: Tên, Trạng thái tài khoản, Số điện thoại, Email.
* **Body main section** gồm 3 tab:
  * **Overview:** Hiển thị các thông tin chi tiết của người dùng.
  * **Setting:** Nơi người dùng truy cập để chỉnh sửa các thông tin cá nhân bao gồm: Fullname và Avatar.
* **My role:** Nơi người dùng có thể truy cập để xem chi tiết các quyền.

## III. Hướng dẫn chi tiết

### Login

🎯 **Mục tiêu:** Đăng nhập thành công vào hệ thống OPS để thực hiện các thao tác quản lý.

{% stepper %}
{% step %}
## Truy cập hệ thống OPS

Mở trình duyệt và truy cập đường dẫn hệ thống OPS [tại đây](https://ops.sapp.edu.vn/auth/login).
{% endstep %}

{% step %}
## Nhập thông tin đăng nhập

Nhập Username và Password vào ô tương ứng trên màn hình đăng nhập.

![](<../.gitbook/assets/image (2)>)
{% endstep %}

{% step %}
## Xác nhận đăng nhập

Nhấn nút Sign in. Hệ thống xác thực thông tin và chuyển hướng đến màn hình chính.

![](<../.gitbook/assets/image (3)>)

✅ **Kết quả:** Hệ thống hiển thị thông báo "Login Successfull".
{% endstep %}
{% endstepper %}

### View Profile Details

🎯 **Mục tiêu:** Xem toàn bộ thông tin chi tiết của tài khoản đang đăng nhập.

{% stepper %}
{% step %}
## Truy cập My Profile

Tại góc dưới bên trái màn hình, hover chuột vào avatar và chọn "**My profile**".

![](<../.gitbook/assets/image (4)>)
{% endstep %}

{% step %}
## Xem thông tin chung — Truy cập tab Overview

Hệ thống hiển thị Overview thông tin chi tiết của tài khoản, bao gồm: Mã code, Fullname, Username, Email, Số điện thoại, Role, Trạng thái, Thời gian cập nhật.

![](<../.gitbook/assets/image (5)>)

✅ **Kết quả:** Màn hình Profile hiển thị đầy đủ thông tin cá nhân của tài khoản.
{% endstep %}

{% step %}
## Xem quyền chi tiết — Truy cập tab My role

Truy cập tab **My role**, click vào từng dòng để xem chi tiết nhóm quyền.

![](<../.gitbook/assets/image (6)>)

✅ **Kết quả:** Màn hình Profile hiển thị đầy đủ thông tin quyền của người dùng.
{% endstep %}
{% endstepper %}

### Reset Password

🎯 **Mục tiêu:** Thay đổi mật khẩu đăng nhập của tài khoản.

#### Cách 1: Truy cập User Management (Áp dụng cho người dùng có quyền edit thông tin Staffs)

{% stepper %}
{% step %}
## Truy cập danh sách Staffs

Truy cập **User Management** > Chọn **Staffs**.

![](<../.gitbook/assets/image (7)>)

✅ **Kết quả:** Màn hình hiển thị danh sách Staffs.
{% endstep %}

{% step %}
## Chọn Reset password

Tìm tài khoản cần Thay đổi mật khẩu > Chọn **Action** > **Reset password**.

![](<../.gitbook/assets/image (8)>)
{% endstep %}

{% step %}
## Xác nhận Reset

![](<../.gitbook/assets/image (9)>)

✅ **Kết quả:** Màn hình sẽ hiển thị mật khẩu mới. Pop-up này sẽ được đóng khi người dùng chọn "Hoàn tất".

![](<../.gitbook/assets/image (10)>)
{% endstep %}
{% endstepper %}

#### Cách 2: Sử dụng tính năng Quên mật khẩu (Áp dụng cho người dùng KHÔNG có quyền edit thông tin Staffs)

{% stepper %}
{% step %}
## Chọn Forgot Password

Tại màn hình Đăng nhập chọn Forgot Password.

![](<../.gitbook/assets/image (11)>)
{% endstep %}

{% step %}
## Nhập email đăng ký

Nhập thông tin email đăng ký tài khoản và nhấn "**Send**".

![](<../.gitbook/assets/image (12)>)

✅ **Kết quả:** Màn hình sẽ hiển thị box nhập mã code.

![](<../.gitbook/assets/image (13)>)
{% endstep %}

{% step %}
## Xác thực mã code

Truy cập email nhận thông tin mã code và chọn **Verify**.
{% endstep %}

{% step %}
## Nhập mật khẩu mới

Nhập mật khẩu cũ, mật khẩu mới và chọn **Submit**.

![](<../.gitbook/assets/image (14)>)

✅ **Kết quả:** Hệ thống hiển thị màn hình Đổi mật khẩu thành công như sau.

![](<../.gitbook/assets/image (15)>)
{% endstep %}
{% endstepper %}

### Edit Email

🎯 **Mục tiêu:** Cập nhật địa chỉ email của tài khoản. Áp dụng cho tài khoản có quyền Edit Staff.

{% stepper %}
{% step %}
## Truy cập danh sách Staff

Truy cập **User & Org Management** và chọn **Staff**.

![](<../.gitbook/assets/image (16)>)

✅ **Kết quả:** Màn hình hiển thị danh sách Staffs.
{% endstep %}

{% step %}
## Chọn Edit Email

Tìm tài khoản cần Thay đổi Email > Chọn **Action > Edit Email**.

![](<../.gitbook/assets/image (17)>)

✅ **Kết quả:** Hệ thống sẽ gửi mã OTP xác nhận edit email về email gốc của người dùng.
{% endstep %}

{% step %}
## Nhập Email mới và OTP

Nhập Email mới và OTP được gửi từ Bước 2 sau đó chọn **Save**.

![](<../.gitbook/assets/image (18)>)

✅ **Kết quả:** Email được cập nhật thành công.
{% endstep %}
{% endstepper %}
