# Quản lý cơ sở học (Facility)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version | Effective Date |
| -------------- | ------------- | ----- | ------------------------------ | ------- | -------------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   | May 18, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, CX/Admin cơ sở

**Đường dẫn:** Department Operations → Share Services → Facility List
{% endhint %}

{% hint style="info" %}
**Phạm vi & Module liên quan**

* **Module chính:** Operation
* **Chức năng chính:** Facility
* **Module liên quan:** Classroom, Staff, Class, Calendar, Learning Schedule
{% endhint %}

{% hint style="warning" %}
**Điều kiện tiên quyết:**

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập menu **Facility**.
{% endhint %}

{% hint style="info" %}
Màn hình **Facility Detail** gồm các tab: **Overview, Classroom List, Staff List, Settings**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách cơ sở</summary>

{% stepper %}
{% step %}
**Mở màn hình Facility List**

Người dùng chọn **Facility List** tại submenu **Department Operations**.

<figure><img src="../../.gitbook/assets/image (461).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình danh sách cơ sở.

<figure><img src="../../.gitbook/assets/image (462).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin cơ sở**

Người dùng xem thông tin tại bảng **Facility List**: Code, Name, Address, Status, Area, Total Room và Date.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tìm kiếm/lọc cơ sở</summary>

{% stepper %}
{% step %}
**Nhập/chọn điều kiện tìm kiếm**

Người dùng nhập hoặc chọn điều kiện tại màn hình **Facility List** (tên/mã cơ sở, Province, Status hoặc khoảng thời gian tạo).

<figure><img src="../../.gitbook/assets/image (463).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search**. Hệ thống hiển thị danh sách cơ sở thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
**Chọn Reset**

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại danh sách cơ sở theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết cơ sở</summary>

{% stepper %}
{% step %}
**Mở Facility Detail**

Người dùng nhấp vào **tên cơ sở** tại màn hình **Facility List**.

<figure><img src="../../.gitbook/assets/image (464).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Facility Detail**.

<figure><img src="../../.gitbook/assets/image (465).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin cơ sở**

Người dùng xem thông tin tại màn hình **Facility Detail**: Name, Code, Status, Total Room, Province và Address.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem danh sách phòng học thuộc cơ sở</summary>

{% stepper %}
{% step %}
**Mở Facility Detail**

Người dùng mở màn hình **Facility Detail** của cơ sở cần xem.
{% endstep %}

{% step %}
**Chọn tab Classroom List**

Người dùng chọn tab **Classroom List** tại màn hình **Facility Detail**.

<figure><img src="../../.gitbook/assets/image (466).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách phòng học thuộc cơ sở.

<figure><img src="../../.gitbook/assets/image (467).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin phòng học**

Người dùng xem thông tin tại bảng **Classroom List**: Code, Name, Type, Capacity, Deferred Students, New Students, Status và Address.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới cơ sở</summary>

{% stepper %}
{% step %}
**Chọn Create Facility**

Người dùng chọn **Create Facility** tại màn hình **Facility List**.

<figure><img src="../../.gitbook/assets/image (468).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình tạo mới cơ sở.

<figure><img src="../../.gitbook/assets/image (469).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin cơ sở**

Người dùng nhập thông tin tại màn hình **Create Facility**: Name, Code, Province, District, Ward và Address detail.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save** tại màn hình **Create Facility**. Hệ thống lưu thông tin và tạo mới cơ sở.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa thông tin cơ sở</summary>

{% stepper %}
{% step %}
**Chọn Action → Edit**

Người dùng chọn **Action → Edit** tại cơ sở cần chỉnh sửa trên màn hình **Facility List**.

<figure><img src="../../.gitbook/assets/image (470).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình chỉnh sửa cơ sở.

<figure><img src="../../.gitbook/assets/image (471).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật thông tin**

Người dùng cập nhật thông tin cần chỉnh sửa tại màn hình **Edit Facility** theo quyền được cấp.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save** tại màn hình **Edit Facility**. Hệ thống lưu thông tin mới của cơ sở.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa cơ sở từ màn hình chi tiết</summary>

{% stepper %}
{% step %}
**Mở Facility Detail**

Người dùng mở màn hình **Facility Detail** của cơ sở cần chỉnh sửa.
{% endstep %}

{% step %}
**Chọn Edit Facility / tab Settings**

Người dùng chọn **Edit Facility** hoặc chuyển sang tab **Settings** tại màn hình **Facility Detail**.

<figure><img src="../../.gitbook/assets/image (472).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình chỉnh sửa thông tin cơ sở.
{% endstep %}

{% step %}
**Cập nhật thông tin và Save**

Người dùng cập nhật thông tin cần chỉnh sửa, sau đó chọn **Save** để lưu thông tin mới.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem danh sách nhân viên thuộc cơ sở</summary>

{% stepper %}
{% step %}
**Mở Facility Detail**

Người dùng mở màn hình **Facility Detail** của cơ sở cần xem.
{% endstep %}

{% step %}
**Chọn tab Staff List**

Người dùng chọn tab **Staff List** tại màn hình **Facility Detail**.

<figure><img src="../../.gitbook/assets/image (473).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách nhân viên thuộc cơ sở.

<figure><img src="../../.gitbook/assets/image (474).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin nhân viên**

Người dùng xem thông tin tại bảng **Staff List**: Code, Name, Phone number, Email, Facility manager và Job position.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tìm kiếm nhân viên thuộc cơ sở</summary>

{% stepper %}
{% step %}
**Nhập từ khóa tìm kiếm**

Người dùng nhập thông tin vào ô **Search staff** tại tab **Staff List** (Code, Name, Phone number hoặc Email).

<figure><img src="../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search**. Hệ thống hiển thị danh sách nhân viên thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
**Chọn Reset**

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại toàn bộ danh sách nhân viên thuộc cơ sở.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thêm nhân viên vào cơ sở</summary>

{% stepper %}
{% step %}
**Chọn tab Staff List**

Người dùng chọn tab **Staff List** tại màn hình **Facility Detail**.
{% endstep %}

{% step %}
**Chọn Add Staff**

Người dùng chọn **Add Staff** tại tab **Staff List**.

<figure><img src="../../.gitbook/assets/image (476).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Add Staff** và hiển thị danh sách nhân viên có thể thêm vào cơ sở.

<figure><img src="../../.gitbook/assets/image (477).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm nhân viên (nếu cần)**

Người dùng nhập hoặc chọn điều kiện tìm kiếm tại màn hình **Add Staff** (tên/mã/email/số điện thoại, Department, Staff position hoặc Program).

<figure><img src="../../.gitbook/assets/image (478).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search**. Hệ thống hiển thị danh sách nhân viên thỏa mãn điều kiện.
{% endstep %}

{% step %}
**Tick chọn nhân viên**

Người dùng tick chọn nhân viên cần thêm vào cơ sở.

<figure><img src="../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Add**

Người dùng chọn **Add** tại màn hình **Add Staff**. Hệ thống thêm các nhân viên đã chọn vào cơ sở. (Chọn **Cancel** nếu muốn dừng thao tác.)
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa một nhân viên khỏi cơ sở</summary>

{% stepper %}
{% step %}
**Chọn tab Staff List**

Người dùng chọn tab **Staff List** tại màn hình **Facility Detail**.
{% endstep %}

{% step %}
**Chọn Action → Delete**

Người dùng chọn **Action → Delete** tại dòng nhân viên cần xóa.

<figure><img src="../../.gitbook/assets/image (480).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup xác nhận xóa.

<figure><img src="../../.gitbook/assets/image (481).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận xóa**

Người dùng chọn **Yes** tại popup xác nhận. Hệ thống xóa nhân viên khỏi cơ sở nếu nhân viên đủ điều kiện xóa.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa nhiều nhân viên khỏi cơ sở</summary>

{% stepper %}
{% step %}
**Tick chọn các nhân viên cần xóa**

Người dùng tick chọn các nhân viên cần xóa tại tab **Staff List**.
{% endstep %}

{% step %}
**Chọn Delete Selected**

Người dùng chọn **Delete Selected** tại tab **Staff List**.

<figure><img src="../../.gitbook/assets/image (482).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup xác nhận xóa.

<figure><img src="../../.gitbook/assets/image (483).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận xóa**

Người dùng chọn **Yes** tại popup xác nhận. Hệ thống xóa các nhân viên đã chọn khỏi cơ sở nếu các nhân viên đủ điều kiện xóa.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần có quyền tương ứng để xem, tạo mới, chỉnh sửa hoặc xóa cơ sở.
2. Tên cơ sở mới không được trùng với tên của các cơ sở đã tồn tại trên hệ thống.
3. Cơ sở có trạng thái **Đang hoạt động** hoặc **Ngừng hoạt động**.
4. Những cơ sở đang được sử dụng (cơ sở có phòng học đã được đặt lịch) không được chuyển trạng thái từ **Đang hoạt động** sang **Ngừng hoạt động**.
{% endhint %}

### Quy tắc tạo/chỉnh sửa cơ sở

| Quy tắc                 | Mô tả                                                             |
| ----------------------- | ----------------------------------------------------------------- |
| Name                    | Tên cơ sở không được trùng với cơ sở đã tồn tại.                  |
| Code                    | Mã cơ sở dùng để định danh cơ sở trên hệ thống.                   |
| Province/District/Ward  | Dùng để xác định khu vực của cơ sở.                               |
| Address detail          | Dùng để nhập địa chỉ chi tiết như số nhà, tên đường.              |
| Status                  | Có thể là Đang hoạt động hoặc Ngừng hoạt động.                    |
| Cơ sở đang được sử dụng | Không được đổi trạng thái từ Đang hoạt động sang Ngừng hoạt động. |

### Quy tắc Facility Manager

| Quy tắc                                     | Mô tả                                                                                        |
| ------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Facility Manager                            | Là nhân viên được tick tại cột Facility manager trong Staff List.                            |
| Số lượng Facility Manager                   | Mỗi cơ sở có duy nhất **01 Facility Manager**.                                               |
| Receptionist Part-time                      | Nhân viên có Job position = Receptionist Part-time không thể được chọn làm Facility Manager. |
| Nhân viên không phải Receptionist Part-time | Có thể là Facility Manager của nhiều hơn một cơ sở.                                          |
| Xóa Facility Manager                        | Không được xóa nhân viên đang là Facility Manager của cơ sở.                                 |
| Thông báo lỗi khi xóa Facility Manager      | Hệ thống hiển thị "Facility Manager can not be deleted".                                     |

### Quy tắc thêm nhân viên vào cơ sở

| Quy tắc                                                    | Mô tả                                                                                              |
| ---------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| Danh sách Add Staff                                        | Hiển thị danh sách nhân viên thuộc phòng ban Customer Experience theo điều kiện lọc.               |
| Nhân viên đã thuộc cơ sở hiện tại                          | Không hiển thị trong danh sách Add Staff.                                                          |
| Receptionist Part-time đã thuộc cơ sở khác                 | Không hiển thị trong danh sách Add Staff.                                                          |
| Nhân viên có Status = Block                                | Không hiển thị trong danh sách Add Staff.                                                          |
| Cơ sở chưa có nhân viên                                    | Nhân viên được thêm sớm nhất sẽ tự động là Facility Manager nếu không phải Receptionist Part-time. |
| Cơ sở chưa có nhân viên và chỉ chọn Receptionist Part-time | Hệ thống hiển thị lỗi và không cho phép thêm nhân viên vào cơ sở.                                  |

### Quy tắc xóa nhân viên khỏi cơ sở

| Quy tắc             | Mô tả                                                                            |
| ------------------- | -------------------------------------------------------------------------------- |
| Xóa một nhân viên   | Người dùng chọn Action → Delete tại nhân viên cần xóa.                           |
| Xóa nhiều nhân viên | Người dùng tick chọn nhân viên và chọn Delete Selected.                          |
| Facility Manager    | Không thể chọn checkbox để xóa hàng loạt nếu nhân viên đang là Facility Manager. |
| Xác nhận xóa        | Hệ thống hiển thị popup xác nhận trước khi xóa.                                  |
| Chọn Yes            | Hệ thống xóa nhân viên khỏi cơ sở nếu hợp lệ.                                    |
| Chọn No             | Hệ thống hủy thao tác xóa và giữ nguyên danh sách nhân viên.                     |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                               | Nguyên nhân                                                            | Cách xử lý                                                        |
| ---------------------------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------- |
| Không tạo/lưu được cơ sở                       | Tên cơ sở bị trùng hoặc thiếu thông tin bắt buộc                       | Đặt tên không trùng, nhập đủ thông tin rồi Save                   |
| Không đổi được trạng thái sang Ngừng hoạt động | Cơ sở đang được sử dụng (có phòng học đã đặt lịch)                     | Không thể đổi trạng thái khi cơ sở đang được sử dụng              |
| Không tìm thấy cơ sở/nhân viên                 | Sai điều kiện tìm kiếm/lọc                                             | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định        |
| Không thấy nhân viên trong danh sách Add Staff | Nhân viên đã thuộc cơ sở, Block, hoặc Receptionist PT thuộc cơ sở khác | Đối chiếu quy tắc thêm nhân viên; chọn nhân viên hợp lệ           |
| Không thêm được nhân viên vào cơ sở mới        | Cơ sở chưa có nhân viên mà chỉ chọn Receptionist Part-time             | Thêm ít nhất 1 nhân viên không phải Receptionist Part-time làm FM |
| Lỗi "Facility Manager can not be deleted"      | Đang xóa nhân viên là Facility Manager của cơ sở                       | Chỉ định Facility Manager khác trước khi xóa nhân viên này        |
