# Xem danh sách lịch trực (Receptionist Shift)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Facility Manager, Receptionist Full-time, Receptionist Part-time

**Đường dẫn:** Department Operations → Customer Experience → Receptionist → Receptionist Shift
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Shift
* **Module liên quan:** Facility, Classroom, Class Calendar, Classroom Calendar, Receptionist Shift Management
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập menu **Receptionist Shift**.
* Tài khoản có quyền xem lịch trực của Lễ tân.
{% endhint %}

{% hint style="info" %}
Chức năng này chỉ để xem danh sách lịch trực; không bao gồm đăng ký ca trực hoặc chỉnh sửa thông tin lịch trực.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách lịch trực</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Receptionist Shift**

Người dùng truy cập **Department Operations → Customer Experience → Receptionist → Receptionist Shift** trên thanh menu.

<figure><img src="../../.gitbook/assets/image (533).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình danh sách lịch trực của Lễ tân.

<figure><img src="../../.gitbook/assets/image (534).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Facility**

Người dùng chọn **Facility** tại vùng bộ lọc (trường bắt buộc). Nếu người dùng có gắn cơ sở, hệ thống mặc định hiển thị cơ sở đầu tiên của nhân viên.
{% endstep %}

{% step %}
**Chọn On-call person (nếu cần)**

Người dùng chọn **On-call person** nếu cần lọc theo người trực cụ thể (trường không bắt buộc).
{% endstep %}

{% step %}
**Chọn Start date - End date**

Người dùng chọn **Start date - End date** tại vùng bộ lọc (trường bắt buộc) để xác định khoảng thời gian cần xem lịch trực.
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search**. Hệ thống hiển thị danh sách lịch trực thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
**Xem thông tin lịch trực**

Người dùng xem thông tin tại bảng danh sách: Date, Shift, On-call person, Room holder, Section, Teacher, Classroom, Attendant và Note.
{% endstep %}

{% step %}
**Chọn Reset (nếu cần)**

Người dùng chọn **Reset** nếu muốn làm mới bộ lọc. Hệ thống xóa các điều kiện tìm kiếm đã nhập và đưa bộ lọc về trạng thái mặc định.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Facility** và **Start date - End date** là các trường bắt buộc.
2. **Facility** có thể được hệ thống mặc định theo cơ sở đầu tiên của nhân viên nếu nhân viên có gắn cơ sở.
3. Kết quả lịch trực của tháng tiếp theo được hệ thống cập nhật vào ngày **21 hàng tháng**.
4. Cột **On-call person** hiển thị tên người trực đã có trong ca; nếu ca chưa đủ người trực, hệ thống hiển thị "-------------" với số lượng tương ứng số người còn thiếu.
5. Cột **Attendant** và **Note** được cập nhật tại chức năng chỉnh sửa lịch trực, không chỉnh sửa trực tiếp tại màn hình danh sách.
6. Nút **Reset** chỉ làm mới điều kiện tìm kiếm, không xóa dữ liệu lịch trực.
{% endhint %}

### Quy tắc hiển thị ca trực theo loại Lễ tân

| Loại tài khoản         | Quy tắc hiển thị                                                                                      |
| ---------------------- | ----------------------------------------------------------------------------------------------------- |
| Receptionist Part-time | Thứ hai đến thứ sáu: chỉ hiển thị ca tối.                                                             |
| Receptionist Part-time | Thứ bảy, Chủ nhật: hiển thị cả ba ca sáng, chiều, tối.                                                |
| Receptionist Part-time | Ca sáng và ca chiều từ thứ hai đến thứ sáu chỉ hiển thị nếu Lễ tân Part-time được gắn với ca trực đó. |
| Receptionist Full-time | Hiển thị toàn bộ ca sáng, chiều, tối từ thứ hai đến Chủ nhật.                                         |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                      | Nguyên nhân                                              | Cách xử lý                                               |
| ----------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------- |
| Không hiển thị được danh sách lịch trực               | Chưa chọn Facility hoặc Start date - End date (bắt buộc) | Chọn đầy đủ Facility và khoảng thời gian rồi bấm Search  |
| Ca trực hiển thị "------------"                       | Ca trực chưa đủ người trực                               | Đây là biểu thị số người còn thiếu, không phải lỗi       |
| Không thấy lịch trực tháng tiếp theo                  | Lịch tháng sau được cập nhật vào ngày 21 hàng tháng      | Xem lại sau ngày 21 hàng tháng                           |
| Lễ tân Part-time không thấy ca sáng/chiều ngày thường | Part-time chỉ thấy ca tối T2–T6 (trừ khi được gắn ca)    | Đây là quy tắc hiển thị theo loại Lễ tân, không phải lỗi |
| Không cập nhật được Attendant/Note                    | Hai cột này không sửa trực tiếp tại màn hình danh sách   | Cập nhật tại chức năng chỉnh sửa lịch trực               |
| Không truy cập được Receptionist Shift                | Tài khoản chưa có quyền xem lịch trực                    | Liên hệ quản trị để được cấp quyền                       |
