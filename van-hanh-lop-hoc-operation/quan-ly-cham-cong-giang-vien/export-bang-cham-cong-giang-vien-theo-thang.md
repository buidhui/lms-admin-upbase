# Export bảng chấm công giảng viên theo tháng

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version |
| -------------- | --------------- | ----- | ------------------ | ------- |
| Jul 16, 2026   | Nguyễn Duy Hiếu | A     |                    | 1.0.0   |

## I. Giới Thiệu Chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Đường dẫn:** [https://ops.sapp.edu.vn/](https://ops.sapp.edu.vn/)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chấm công Giảng viên (Teacher Attendance) – Export
* **Chức năng chính:** Export danh sách chấm công của giảng viên theo bộ lọc ra file Excel
* **Mục đích:** Xuất bảng công theo template để import lên phần mềm nhân sự (Base)
* **Module liên quan:**
  * Teacher (Quản lý giảng viên)
  * Operations – Customer Experience
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* User đã đăng nhập thành công vào hệ thống OPS.
* User có quyền xem bảng chấm công.
* User có quyền export danh sách chấm công.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Export bảng chấm công giảng viên</summary>

> 🎯 _Mục tiêu: Xuất danh sách chấm công của giảng viên theo bộ lọc ra file Excel theo template để import lên phần mềm nhân sự (Base)._

{% stepper %}
{% step %}
**Đăng nhập hệ thống OPS**
{% endstep %}

{% step %}
**Chọn Department → Operations**
{% endstep %}

{% step %}
**Chọn Customer Experience**
{% endstep %}

{% step %}
**Chọn Teacher**
{% endstep %}

{% step %}
**Chọn tab Attendance**
{% endstep %}

{% step %}
**Thiết lập bộ lọc để khoanh vùng dữ liệu cần xuất**

Chọn tháng (Date Filter, mặc định tháng hiện tại) và các bộ lọc khác như mã/tên giảng viên, Class, Program… File Export sẽ xuất đúng theo bộ lọc đang chọn.

<figure><img src="../../.gitbook/assets/image (1430).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Ấn nút "Export"**

<figure><img src="../../.gitbook/assets/image (1429).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Bộ lọc trên màn Attendance</summary>

| Trường                    | Loại   | Mô tả                                                                    |
| ------------------------- | ------ | ------------------------------------------------------------------------ |
| Search teacher code, name | Label  | Tìm kiếm theo mã, tên giảng viên                                         |
| Gender                    | List   | Tìm kiếm theo giới tính                                                  |
| Class                     | List   | Tìm kiếm theo lớp giảng dạy                                              |
| Teaching Status           | List   | Tìm kiếm theo tình trạng giảng dạy                                       |
| Program                   | List   | Tìm kiếm theo chương trình học. Flow filter: Program » Subject » Section |
| Subject                   | List   | Tìm kiếm theo môn học                                                    |
| Section                   | List   | Tìm kiếm theo section trong môn học                                      |
| Person in Charge          | List   | Tìm kiếm theo người phụ trách                                            |
| Date Filter               | Date   | Lọc theo tháng. Mặc định tháng hiện tại                                  |
| Export                    | Button | Xuất thông tin bảng công của giảng viên theo bộ lọc đang chọn            |

</details>

<details>

<summary>Thông tin hiển thị trên màn Attendance</summary>

| Cột                 | Loại   | Mô tả                                                                                                                 |
| ------------------- | ------ | --------------------------------------------------------------------------------------------------------------------- |
| Code                | Label  | Mã giảng viên                                                                                                         |
| Teacher Name        | Label  | Tên giảng viên                                                                                                        |
| Attendance          | Number | Công giảng viên trong tháng. Định dạng: **Thời gian chấm công thực tế / Công chuẩn**                                  |
| Late Count          | Number | Số lần đi muộn/về sớm trong tháng. Đi muộn: check-in muộn hơn giờ vào lớp; Về sớm: check-out sớm hơn giờ kết thúc lớp |
| Late Minutes        | Number | Số phút đi muộn/về sớm                                                                                                |
| Thời gian chấm công | Number | Hiển thị theo cột tất cả các ngày trong tháng — số công thực tế của giảng viên theo từng ngày                         |

</details>

<details>

<summary>Nội dung &#x26; định dạng file Export</summary>

Khi click nút **Export**, hệ thống xuất file Excel theo [template](https://docs.google.com/spreadsheets/d/1dqXXl6vFJt3Qvw8_y-RCu9W5XuXEJd0C0xgBQQaJid8/edit) với các quy định:

| Nội dung          | Quy định                                                                                                |
| ----------------- | ------------------------------------------------------------------------------------------------------- |
| Tên file          | `teacher_attendance_[tháng]_[năm]` — VD: `teacher_attendance_04_2026`                                   |
| Phạm vi dữ liệu   | Xuất theo đúng bộ lọc đang chọn                                                                         |
| Employee ID       | Mã giảng viên (Mapping: **Code**)                                                                       |
| Name              | Tên giảng viên (Mapping: **Teacher name**)                                                              |
| Dữ liệu chấm công | Thời gian check-in, check-out thực tế của **tất cả các ngày trong tháng** (theo filter tháng đang chọn) |

<figure><img src="../../.gitbook/assets/image (1431).png" alt=""><figcaption></figcaption></figure>

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Dữ liệu Export xuất theo **đúng bộ lọc** đang chọn tại màn Attendance.
2. Date Filter mặc định là **tháng hiện tại**; file xuất theo dữ liệu check-in/check-out của tất cả các ngày trong tháng được chọn.
3. Tên file tuân theo định dạng `teacher_attendance_[tháng]_[năm]`.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Chọn tháng và các bộ lọc phù hợp trước khi Export để file kết quả gọn, đúng phạm vi cần dùng.
2. Sử dụng đúng template để thuận tiện import lên phần mềm nhân sự (Base).
{% endhint %}
