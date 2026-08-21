# Import lớp học (Import Class)

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 25, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin, Ops User, Academic/CX User

**Đường dẫn:** Class → Class List → Import Class

#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Import Class
* **Module liên quan:** Class List, Course, Program, Subject, Facility, Exam, Class Owner / CX Admin, Import Log

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class**.
* Tài khoản có quyền import lớp học.

## II. Hướng dẫn chi tiết

### Import Class

{% stepper %}
{% step %}
## Chọn Import Class

Admin chọn **Import Class** tại màn hình **Class List**. Hệ thống hiển thị popup tải file import.

![](<../.gitbook/assets/image (211)>)
{% endstep %}

{% step %}
## Chọn Browse để chọn file

Admin chọn **Browse** tại popup **Import Class** để chọn file từ thiết bị. Hệ thống chỉ chấp nhận file định dạng **.csv** hoặc **.xlsx**.

![](<../.gitbook/assets/image (212)>)
{% endstep %}

{% step %}
## Chọn đúng file import

Admin chọn đúng file import cần tải lên. Mỗi lần import, hệ thống chỉ cho phép chọn **01 file**.

![](<../.gitbook/assets/image (213)>)
{% endstep %}

{% step %}
## Chọn Import

Admin chọn **Import** tại popup **Import Class**. Hệ thống tải file lên và bắt đầu xử lý dữ liệu lớp học trong file.

![](<../.gitbook/assets/image (214)>)
{% endstep %}

{% step %}
## Xem kết quả import

Hệ thống hiển thị hộp thoại kết quả import sau khi xử lý file: tên file, tổng số bản ghi, số lớp tạo thành công và số lớp tạo thất bại.
{% endstep %}

{% step %}
## Chọn View Log

Admin chọn **View Log** tại hộp thoại kết quả import để xem chi tiết trạng thái từng bản ghi. Hệ thống mở màn hình chi tiết log import.

![](<../.gitbook/assets/image (216)>)
{% endstep %}

{% step %}
## Kiểm tra các dòng lỗi

Admin kiểm tra các dòng lỗi tại màn hình **Import Detail**. Các trường dữ liệu không hợp lệ được bôi đỏ và lý do lỗi được hiển thị tại cột **Errors**.

![](<../.gitbook/assets/image (218)>)
{% endstep %}
{% endstepper %}

### Tải file mẫu import

{% stepper %}
{% step %}
## Chọn Import Class

Admin chọn **Import Class** tại màn hình **Class List**.
{% endstep %}

{% step %}
## Chọn Download Template / File mẫu

Admin chọn **Download Template / File mẫu** trong popup import. Hệ thống tải file mẫu về thiết bị.
{% endstep %}

{% step %}
## Nhập dữ liệu vào file mẫu

Admin nhập dữ liệu lớp học vào file mẫu theo đúng cấu trúc được hệ thống cung cấp.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chức năng **Import Class** dùng để tạo nhiều lớp học cùng lúc.
2. File import chỉ chấp nhận định dạng **.csv** hoặc **.xlsx**.
3. Mỗi lần import chỉ được chọn **01 file**.
4. Nên tải **file mẫu** trước khi nhập dữ liệu import; dữ liệu cần tuân thủ đúng cấu trúc và định dạng của template.
5. Các bản ghi hợp lệ sẽ được hệ thống tạo lớp thành công; các bản ghi không hợp lệ sẽ không được tạo lớp và được ghi nhận lỗi trong log.
6. Hệ thống hiển thị số lượng bản ghi thành công và thất bại sau khi import.
7. Các trường không hợp lệ trong file import được bôi đỏ tại màn hình chi tiết log; lý do lỗi hiển thị tại cột **Errors**.

### Mẹo sử dụng

1. Luôn tải file mẫu mới nhất từ popup import trước khi chuẩn bị dữ liệu để tránh lệch cấu trúc cột.
2. Trước khi import, nên rà soát các trường bắt buộc (Code, Construction Mode, Type, Course...) để giảm số bản ghi lỗi.
3. Sau khi import, nên mở **View Log** để xử lý các dòng bị bôi đỏ rồi import lại phần lỗi.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                     | Nguyên nhân                                    | Cách xử lý                                                           |
| ------------------------------------ | ---------------------------------------------- | -------------------------------------------------------------------- |
| Không chọn được file để import       | File sai định dạng (không phải .csv/.xlsx)     | Chuyển file về định dạng .csv hoặc .xlsx rồi chọn lại                |
| Không import được nhiều file một lúc | Mỗi lần import chỉ cho phép 01 file            | Chọn từng file một để import                                         |
| Một số bản ghi import thất bại       | Dữ liệu không đúng cấu trúc/định dạng template | Mở View Log, sửa các trường bị bôi đỏ theo cột Errors rồi import lại |
| Dữ liệu lệch cột sau khi import      | Dùng sai phiên bản file mẫu                    | Tải lại file mẫu mới nhất và nhập đúng cấu trúc                      |
| Không thực hiện được import          | Tài khoản chưa có quyền import lớp học         | Liên hệ quản trị để được cấp quyền import lớp học                    |
