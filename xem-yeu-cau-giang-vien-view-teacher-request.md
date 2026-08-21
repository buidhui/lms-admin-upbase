# Xem yêu cầu giảng viên (View Teacher Request)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin, CX Admin

**Đường dẫn:** Customer Experience → Teacher → List Request

#### Phạm vi & Module liên quan

* **Module chính:** Teacher Request Management
* **Chức năng chính:** List Request / View Request Detail
* **Module liên quan:** Teacher, Class, Calendar, Teacher Calendar, Weekly Norm, Timeoff Request

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **OPS/LMS Operations**.
* Tài khoản có quyền truy cập chức năng **List Request**.
* Tài khoản có quyền xem danh sách và thông tin chi tiết yêu cầu giảng viên.

Teacher Request gồm 2 tab chính: **Personal Schedule Request** (Busy Schedule, Weekly Norm) và **Timeoff Request** (Timeoff, Teaching Mode Change). Trạng thái yêu cầu: **Pending, Approved, Rejected, Cancelled**.

## II. Hướng dẫn chi tiết

### Xem danh sách Personal Schedule Request

{% stepper %}
{% step %}
## Truy cập màn hình List Request

Người dùng chọn **Customer Experience > Teacher** trên hệ thống OPS/LMS Operations.

![](<.gitbook/assets/image (630)>)

Hệ thống mở màn hình danh sách yêu cầu và mặc định hiển thị tab **Personal Schedule Request**.
{% endstep %}

{% step %}
## Xem danh sách yêu cầu

Người dùng xem danh sách tại tab **Personal Schedule Request**. Hệ thống hiển thị các yêu cầu Busy Schedule và Weekly Norm theo thời gian tạo mới nhất đến cũ nhất.
{% endstep %}

{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng nhập hoặc chọn điều kiện tại vùng bộ lọc nếu cần (Request name, Request type, Status, Start date - End date).
{% endstep %}

{% step %}
## Chọn Search / Reset

Chọn **Search** để áp dụng điều kiện tìm kiếm; chọn **Reset** để xóa toàn bộ điều kiện và hiển thị lại danh sách theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết Personal Schedule Request

{% stepper %}
{% step %}
## Mở chi tiết từ Request name

Người dùng nhấp vào **Request name** tại tab **Personal Schedule Request**.

![](<.gitbook/assets/image (631)>)

Hệ thống mở màn hình **Request Detail**.
{% endstep %}

{% step %}
## Hoặc chọn Action → View

Người dùng chọn **Action → View** tại dòng yêu cầu nếu muốn mở chi tiết từ menu thao tác.

![](<.gitbook/assets/image (632)>)

Hệ thống mở màn hình **Request Detail** của yêu cầu được chọn.
{% endstep %}

{% step %}
## Kiểm tra thông tin chi tiết

Người dùng kiểm tra thông tin tại màn hình **Request Detail**: tên yêu cầu, thời hạn duyệt, trạng thái, người tạo, người duyệt, thời gian đề xuất và lý do/ghi chú liên quan.

![](<.gitbook/assets/image (633)>)
{% endstep %}
{% endstepper %}

### Xem danh sách Timeoff Request

{% stepper %}
{% step %}
## Truy cập màn hình List Request

Người dùng chọn **Customer Experience > Teacher** trên hệ thống OPS/LMS Operations. Hệ thống mở màn hình danh sách yêu cầu.
{% endstep %}

{% step %}
## Chọn tab Timeoff Request

Người dùng chọn tab **Timeoff Request**.

![](<.gitbook/assets/image (634)>)

Hệ thống hiển thị danh sách yêu cầu Timeoff và Teaching Mode Change.
{% endstep %}

{% step %}
## Xem danh sách yêu cầu

Người dùng xem danh sách tại tab **Timeoff Request**. Hệ thống hiển thị các yêu cầu theo thời gian tạo mới nhất đến cũ nhất.
{% endstep %}

{% step %}
## Tìm kiếm và lọc

Người dùng nhập/chọn điều kiện tại vùng bộ lọc (Request name, Request type, Status, Start date - End date), chọn **Search** để áp dụng hoặc **Reset** để xóa điều kiện.
{% endstep %}
{% endstepper %}

### Xem chi tiết Timeoff Request

{% stepper %}
{% step %}
## Mở chi tiết từ Request name

Người dùng nhấp vào **Request name** tại tab **Timeoff Request**.

![](<.gitbook/assets/image (635)>)

Hệ thống mở màn hình **Request Detail**.
{% endstep %}

{% step %}
## Hoặc chọn Action → View

Người dùng chọn **Action → View** tại dòng yêu cầu nếu muốn mở chi tiết từ menu thao tác.

![](<.gitbook/assets/image (636)>)

Hệ thống mở màn hình **Request Detail** của yêu cầu được chọn.
{% endstep %}

{% step %}
## Kiểm tra thông tin chi tiết

Người dùng kiểm tra thông tin tại màn hình **Request Detail**: tên yêu cầu, thời hạn duyệt, trạng thái, lớp liên quan, lịch buổi học, người tạo, người duyệt và lý do yêu cầu.

![](<.gitbook/assets/image (637)>)
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền xem hoặc duyệt yêu cầu để truy cập danh sách Teacher Request.
2. Màn hình **List Request** mặc định hiển thị tab **Personal Schedule Request**.
3. Tab **Personal Schedule Request** bao gồm yêu cầu **Busy Schedule** và **Weekly Norm**.
4. Tab **Timeoff Request** bao gồm yêu cầu **Timeoff** và **Teaching Mode Change**.
5. Danh sách yêu cầu được sắp xếp theo thời gian tạo từ mới nhất đến cũ nhất.
6. Chức năng này chỉ để xem; không bao gồm tạo mới, chỉnh sửa, duyệt, từ chối, hủy hoặc xóa yêu cầu.

### Quy tắc hiển thị theo loại yêu cầu

| Loại yêu cầu         | Thông tin đặc thù                                                         |
| -------------------- | ------------------------------------------------------------------------- |
| Busy Schedule        | Hiển thị thời gian lịch bận và lý do đăng ký lịch bận.                    |
| Weekly Norm          | Hiển thị thời gian đăng ký định mức, số lượng định mức và ghi chú nếu có. |
| Timeoff              | Hiển thị lớp, buổi học xin nghỉ và lý do xin nghỉ.                        |
| Teaching Mode Change | Hiển thị lớp, buổi học xin đổi hình thức dạy và lý do thay đổi.           |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                      | Nguyên nhân                                    | Cách xử lý                                                 |
| ------------------------------------- | ---------------------------------------------- | ---------------------------------------------------------- |
| Không truy cập được List Request      | Tài khoản chưa có quyền xem yêu cầu giảng viên | Liên hệ quản trị để được cấp quyền xem Teacher Request     |
| Không tìm thấy yêu cầu                | Sai điều kiện tìm kiếm/lọc                     | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định |
| Không thấy yêu cầu cần tìm trong tab  | Yêu cầu thuộc nhóm tab khác (Personal/Timeoff) | Chuyển sang đúng tab tương ứng với loại yêu cầu            |
| Không mở được chi tiết yêu cầu (View) | Tài khoản chưa có quyền xem chi tiết           | Liên hệ quản trị để được cấp quyền xem chi tiết yêu cầu    |
