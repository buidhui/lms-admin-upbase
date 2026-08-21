# Quản lý nhân viên (Staffs)

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** LMS Operator

**Đường dẫn:** User Management → Staffs
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** User Management (Staffs)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống LMS Ops.
* Tài khoản có quyền tương ứng với từng chức năng cần thực hiện (crud).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Danh sách và chi tiết nhân sự vận hành LMS</summary>

{% stepper %}
{% step %}
**Truy cập Staff List**

Truy cập **User Management** → chọn **Students**.

Sử dụng các bộ lọc:

* **Search**: tìm theo Họ tên (Full name), Username, Email, Số điện thoại.
* **Status** (Trạng thái): chọn 1 trong các giá trị cho trước (Active/ Block).
* **Sort by**: sắp xếp theo Họ tên.
* **From Date - To Date**: lọc theo ngày cập nhật thông tin.
{% endstep %}

{% step %}
**Xem chi tiết thông tin nhân sự vận hành LMS**

Nhấn vào tên học viên hoặc nhấn **Action → View Profile**.


{% endstep %}

{% step %}
**Xuất danh sách ra Excel**

* Tại màn hình Staff List, chọn **Export** để hệ thống xuất danh sách nhân sự vận hành LMS (theo điều kiện tìm kiếm hiện tại) thành file Excel và tự động tải về thiết bị.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo tài khoản nhân sự vận hành LMS</summary>



</details>

<details>

<summary>Chỉnh sửa thông tin nhân sự vận hành LMS</summary>



</details>

<details>

<summary>Trạng thái nhân sự vận hành LMS</summary>

Học viên có 2 trạng thái:

| Trạng thái | Mô tả                                                       |
| ---------- | ----------------------------------------------------------- |
| Active     | Tài khoản đang được kích hoạt, có thể đăng nhập vào LMS Ops |
| Block      | Tài khoản bị khóa, không thể đăng nhập vào LMS Ops          |

Có 3 cách thay đổi trạng thái:

{% stepper %}
{% step %}
**Cách 1: Thay đổi qua nút Action**

Tại Staff List → **Action** → **Block** (áp dụng cho tài khoản đang Active) → Xác nhận thay đổi trạng thái.


{% endstep %}

{% step %}
**Cách 2: Thay đổi qua cột Status trong bảng danh sách**

Tại Staff List, nhấn chuyển **Status** tương ứng với nhân sự vận hành LMS cần đổi trạng thái tại cột thông tin Status → chọn **Block** (áp dụng cho tài khoản đang Active) / chọn **Active** (áp dụng cho tài khoản đang Block) → Xác nhận thay đổi trạng thái.


{% endstep %}

{% step %}
**Cách 3: Thay đổi qua trường Status trong Staff Profile**

Staff Profile → Setting → chọn giá trị mới (Active/ Block) để chuyển đổi trạng thái tài khoản nhân sự vận hành LMS đó.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Khi tài khoản nhân sự vận hành LMS bị **Block**, hệ thống LMS Ops sẽ tự động đăng xuất tất cả thiết bị đang đăng nhập của nhân sự đó.
{% endhint %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Username** và P**hone** KHÔNG được phép chỉnh sửa sau khi tạo tài khoản.
2. Tài khoản nhân viên bị **Block** sẽ không thể đăng nhập vào hệ thống LMS Ops.
3. Mỗi nhân viên có thể được gán nhiều **Role** cùng lúc.
4. File Import chỉ chấp nhận định dạng `.csv` hoặc `.xlsx,` mỗi lần chỉ import 1 file.
5. Các trường Username, Email, SĐT trong file import phải là duy nhất, không trùng dữ liệu đã có trong hệ thống.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Tải file mẫu (template) trước khi import để đảm bảo đúng định dạng cột và dữ liệu.
2. Dùng **View Log** sau import để kiểm tra chi tiết lỗi và sửa từng bản ghi lỗi trước khi import lại.
3. Kết hợp nhiều bộ lọc (Search + Status + Role + Gender + Date) để thu hẹp kết quả tìm kiếm nhanh hơn.
4. Gán **Role** ngay sau khi tạo tài khoản để nhân viên có thể truy cập các chức năng cần thiết.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                          | Nguyên nhân                                           | Cách xử lý                                                                                                                           |
| --------------------------------------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------ |
| Không tìm thấy nhân viên trong danh sách                  | Bộ lọc quá hẹp hoặc nhập sai từ khóa                  | Nhấn **Reset** để xóa toàn bộ bộ lọc, thử lại với từ khóa khác.                                                                      |
| Không thể lưu tài khoản mới                               | Thiếu trường bắt buộc (\*) hoặc dữ liệu không hợp lệ  | Kiểm tra các trường có dấu (\*), đảm bảo Username/ Email/ Phone chưa tồn tại trong hệ thống.                                         |
| File import bị lỗi một số dòng                            | Dữ liệu các cột không đúng định dạng yêu cầu          | Nhấn **View Log** để xem chi tiết dòng lỗi, sửa file theo hướng dẫn tại cột 'Errors' và import lại.                                  |
| Nhân viên đăng nhập được nhưng không thấy menu/chức năng  | Chưa được gán Role hoặc Role không có quyền tương ứng | Vào Staff Profile → Edit → gán Role phù hợp với phạm vi công việc của nhân sự đó.                                                    |
| Nhân sự bị Block có thể tự kích hoạt lại tài khoản không? |                                                       | Không. Chỉ tài khoản của nhân sự có quyền và còn có thể truy cập hệ thống LMS Ops mới có thể thay đổi trạng thái từ Block về Active. |
| Tại sao không thấy nút Create?                            |                                                       | Chưa được cấp quyền tạo mới staff. Liên hệ quản trị viên hệ thống để được cấp quyền.                                                 |
