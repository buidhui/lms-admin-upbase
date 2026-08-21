# Quản lý hồ sơ cá nhân (Profile)

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Operator

**Đường dẫn:** [https://ops.sapp.edu.vn/auth/login](https://ops.sapp.edu.vn/auth/login) (truy cập hồ sơ qua avatar góc dưới bên trái → **My profile**)
{% endhint %}

### 1.1 Mục đích

Module **Hồ sơ cá nhân** cho phép người vận hành xem và chỉnh sửa thông tin chi tiết Hồ sơ cá nhân. Bao gồm: Thông tin Đăng nhập, Xem chi tiết hồ sơ cá nhân, Chỉnh sửa hồ sơ cá nhân, Thay đổi mật khẩu, Email.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò            | Quyền hạn                                     |
| --------- | ------------------ | --------------------------------------------- |
| Admin     | Quản trị hệ thống  | Toàn quyền — xem, tạo, chỉnh sửa, xóa, import |
| Operator  | Nhân viên vận hành | Tùy theo Role được cấp trong hệ thống         |

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** User Management (Students, Teachers, Staffs)
* **Module liên quan:** Course Management, Schedule Management, Import Report
* **Hệ thống tích hợp:** LMS Pro (giao diện học viên), HubSpot (Contact học viên)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống OPS.
* Đã đăng nhập thành công vào hệ thống.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện.
{% endhint %}

## II. Tổng quan giao diện

Quản lý hồ sơ cá nhân bao gồm các khu vực chính:

* **Thanh điều hướng trái:** Truy cập các danh mục quản lý theo phân quyền.
* **Top main section:** Hiển thị thông tin cơ bản của người dùng: Tên, Trạng thái tài khoản, Số điện thoại, Email.
* **Body main section** gồm 3 tab:
  * **Overview:** Hiển thị các thông tin chi tiết của người dùng.
  * **Setting:** Nơi người dùng truy cập để chỉnh sửa các thông tin cá nhân bao gồm: Fullname và Avatar.
* **My role:** Nơi người dùng có thể truy cập để xem chi tiết các quyền.

## III. Hướng dẫn chi tiết

<details>

<summary>Login</summary>

🎯 **Mục tiêu:** Đăng nhập thành công vào hệ thống OPS để thực hiện các thao tác quản lý.

{% stepper %}
{% step %}
**Truy cập hệ thống OPS**

Mở trình duyệt và truy cập đường dẫn hệ thống OPS [tại đây](https://ops.sapp.edu.vn/auth/login).
{% endstep %}

{% step %}
**Nhập thông tin đăng nhập**

Nhập Username và Password vào ô tương ứng trên màn hình đăng nhập.

<figure><img src="../.gitbook/assets/image (1106).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận đăng nhập**

Nhấn nút Sign in. Hệ thống xác thực thông tin và chuyển hướng đến màn hình chính.

<figure><img src="../.gitbook/assets/image (1107).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Hệ thống hiển thị thông báo "Login Successfull".
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>View Profile Details</summary>

🎯 **Mục tiêu:** Xem toàn bộ thông tin chi tiết của tài khoản đang đăng nhập.

{% stepper %}
{% step %}
**Truy cập My Profile**

Tại góc dưới bên trái màn hình, hover chuột vào avatar và chọn "**My profile**".

<figure><img src="../.gitbook/assets/image (1108).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin chung — Truy cập tab Overview**

Hệ thống hiển thị Overview thông tin chi tiết của tài khoản, bao gồm: Mã code, Fullname, Username, Email, Số điện thoại, Role, Trạng thái, Thời gian cập nhật.

<figure><img src="../.gitbook/assets/image (1109).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình Profile hiển thị đầy đủ thông tin cá nhân của tài khoản.
{% endstep %}

{% step %}
**Xem quyền chi tiết — Truy cập tab My role**

Truy cập tab **My role**, click vào từng dòng để xem chi tiết nhóm quyền.

<figure><img src="../.gitbook/assets/image (1110).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình Profile hiển thị đầy đủ thông tin quyền của người dùng.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Reset Password</summary>

🎯 **Mục tiêu:** Thay đổi mật khẩu đăng nhập của tài khoản.

**Cách 1: Truy cập User Management (Áp dụng cho người dùng có quyền edit thông tin Staffs)**

{% stepper %}
{% step %}
**Truy cập danh sách Staffs**

Truy cập **User Management** > Chọn **Staffs**.

<figure><img src="../.gitbook/assets/image (1111).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình hiển thị danh sách Staffs.
{% endstep %}

{% step %}
**Chọn Reset password**

Tìm tài khoản cần Thay đổi mật khẩu > Chọn **Action** > **Reset password**.

<figure><img src="../.gitbook/assets/image (1113).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận Reset**

<figure><img src="../.gitbook/assets/image (1114).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình sẽ hiển thị mật khẩu mới. Pop-up này sẽ được đóng khi người dùng chọn "Hoàn tất".

<figure><img src="../.gitbook/assets/image (1115).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

**Cách 2: Sử dụng tính năng Quên mật khẩu (Áp dụng cho người dùng KHÔNG có quyền edit thông tin Staffs)**

{% stepper %}
{% step %}
**Chọn Forgot Password**

Tại màn hình Đăng nhập chọn Forgot Password.

<figure><img src="../.gitbook/assets/image (1116).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập email đăng ký**

Nhập thông tin email đăng ký tài khoản và nhấn "**Send**".

<figure><img src="../.gitbook/assets/image (1117).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình sẽ hiển thị box nhập mã code.

<figure><img src="../.gitbook/assets/image (1118).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác thực mã code**

Truy cập email nhận thông tin mã code và chọn **Verify**.
{% endstep %}

{% step %}
**Nhập mật khẩu mới**

Nhập mật khẩu cũ, mật khẩu mới và chọn **Submit**.

<figure><img src="../.gitbook/assets/image (1119).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Hệ thống hiển thị màn hình Đổi mật khẩu thành công như sau.

<figure><img src="../.gitbook/assets/image (1120).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Edit Email</summary>

🎯 **Mục tiêu:** Cập nhật địa chỉ email của tài khoản. Áp dụng cho tài khoản có quyền Edit Staff.

{% stepper %}
{% step %}
**Truy cập danh sách Staff**

Truy cập **User & Org Management** và chọn **Staff**.

<figure><img src="../.gitbook/assets/image (1121).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Màn hình hiển thị danh sách Staffs.
{% endstep %}

{% step %}
**Chọn Edit Email**

Tìm tài khoản cần Thay đổi Email > Chọn **Action > Edit Email**.

<figure><img src="../.gitbook/assets/image (1122).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Hệ thống sẽ gửi mã OTP xác nhận edit email về email gốc của người dùng.
{% endstep %}

{% step %}
**Nhập Email mới và OTP**

Nhập Email mới và OTP được gửi từ Bước 2 sau đó chọn **Save**.

<figure><img src="../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>

✅ **Kết quả:** Email được cập nhật thành công.
{% endstep %}
{% endstepper %}

</details>
