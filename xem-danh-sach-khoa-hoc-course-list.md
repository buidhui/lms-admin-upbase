# Xem danh sách khóa học (Course List)

Kết quả đạt được: Người dùng có thể xem, lọc danh sách khóa học trong hệ thống

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

**Dành cho:** Admin, SX

**Đường dẫn:** [https://ops.sapp.edu.vn/courses?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/courses?page_index=1\&page_size=10)

#### Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Course List
* **Module liên quan:**
  * Program Category
  * Subject Category
  * Class
  * Resources
  * Certificates
  * Learning Schedule

#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành OPS.
* Tài khoản người dùng có quyền truy cập nhóm chức năng **Course**.

## II. Hướng dẫn chi tiết

### Xem danh sách khóa học

{% stepper %}
{% step %}
## Truy cập màn hình Course 4 Level

Admin truy cập theo đường dẫn:

**Academic Management → Course & Materials → Course 4 Level**

Hệ thống hiển thị màn hình danh sách khóa học.

![](<.gitbook/assets/image (457)>)
{% endstep %}

{% step %}
## Xem thông tin khóa học trên danh sách

![](<.gitbook/assets/image (458)>)

Admin xem thông tin tổng quan của từng khóa học tại bảng danh sách, bao gồm:

* Course name
* Type
* Program
* Status
* Created date
* Updated date
{% endstep %}

{% step %}
## Chuyển trang nếu danh sách có nhiều khóa học

![](<.gitbook/assets/image (459)>)

Nếu danh sách có nhiều khóa học, Admin sử dụng khu vực phân trang ở cuối bảng để:

* Chuyển sang trang tiếp theo.
* Quay lại trang trước.
* Chọn số lượng khóa học hiển thị trên mỗi trang.
{% endstep %}
{% endstepper %}

### Tìm kiếm khóa học theo tên

{% stepper %}
{% step %}
## Nhập từ khóa

![](<.gitbook/assets/image (460)>)

Tại ô **Search course name**, Admin nhập từ hoặc cụm từ mà tên khóa học cần tìm có chứa.
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học có tên phù hợp với từ khóa đã nhập.

![](<.gitbook/assets/image (461)>)
{% endstep %}
{% endstepper %}

### Lọc khóa học theo Program

{% stepper %}
{% step %}
## Chọn Program

![](<.gitbook/assets/image (462)>)

Tại trường **Program**, Admin chọn một giá trị trong danh sách Program có sẵn.
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học thuộc Program đã chọn.

![](<.gitbook/assets/image (463)>)
{% endstep %}
{% endstepper %}

### Lọc khóa học theo Status

{% stepper %}
{% step %}
## Chọn Status

![](<.gitbook/assets/image (464)>)

Tại trường **Status**, Admin chọn một trong các trạng thái:

* Draft
* Publish
* Lock
* Block
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học tương ứng với trạng thái đã chọn.

![](<.gitbook/assets/image (465)>)
{% endstep %}
{% endstepper %}

### Lọc khóa học theo Type

{% stepper %}
{% step %}
## Chọn Type

![](<.gitbook/assets/image (466)>)

Tại trường **Type**, Admin chọn loại khóa học cần lọc:

* Foundation Course
* Trial Course
* Practice Course
* Normal Course
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học thuộc loại đã chọn.

![](<.gitbook/assets/image (467)>)
{% endstep %}
{% endstepper %}

### Lọc khóa học theo khoảng thời gian

{% stepper %}
{% step %}
## Nhập khoảng thời gian

![](<.gitbook/assets/image (468)>)

Admin nhập hoặc chọn khoảng thời gian tại các trường:

| Trường        | Mô tả              |
| ------------- | ------------------ |
| **From date** | Ngày bắt đầu lọc.  |
| **To date**   | Ngày kết thúc lọc. |
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học trong khoảng thời gian đã nhập.

![](<.gitbook/assets/image (469)>)
{% endstep %}
{% endstepper %}

### Sắp xếp danh sách khóa học

{% stepper %}
{% step %}
## Chọn Sort by

![](<.gitbook/assets/image (470)>)

Tại trường **Sort by**, Admin chọn một trong các kiểu sắp xếp:

| Giá trị    | Mô tả                                           |
| ---------- | ----------------------------------------------- |
| **A - Z**  | Sắp xếp danh sách theo tên khóa học từ A đến Z. |
| **Z - A**  | Sắp xếp danh sách theo tên khóa học từ Z đến A. |
| **Latest** | Sắp xếp theo ngày cập nhật mới nhất trước.      |
| **Oldest** | Sắp xếp theo ngày cập nhật cũ nhất trước.       |
{% endstep %}

{% step %}
## Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học theo tiêu chí sắp xếp đã chọn.

![](<.gitbook/assets/image (471)>)
{% endstep %}
{% endstepper %}

### Xóa điều kiện tìm kiếm/lọc

{% stepper %}
{% step %}
## Chọn Reset

![](<.gitbook/assets/image (472)>)

Admin chọn **Reset** tại khu vực tìm kiếm.
{% endstep %}

{% step %}
## Hệ thống xóa bộ lọc

Hệ thống xóa toàn bộ điều kiện đã nhập/chọn tại các trường tìm kiếm và hiển thị lại danh sách khóa học theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Admin cần có quyền truy cập màn hình **Course 4 Level** để xem danh sách khóa học.
2. Khóa học ở trạng thái **Block** không thể được thêm vào lớp học.
3. Khóa học ở trạng thái **Lock** là khóa học đã có ít nhất một học viên tiến hành học trong lớp chứa khóa học đó.
4. Các thao tác trong menu **Action** phụ thuộc vào quyền tài khoản và trạng thái hiện tại của khóa học.

### Mẹo sử dụng

1. Khi cần tìm nhanh một khóa học cụ thể, nên nhập một phần tên khóa học vào ô **Search course name** thay vì nhập đầy đủ tên.
2. Khi danh sách có nhiều khóa học, nên kết hợp nhiều điều kiện như **Program + Status + Type** để thu hẹp kết quả.
3. Nên dùng bộ lọc **Status = Draft** để kiểm tra các khóa học đang tạo dở/chưa publish.
4. Nên dùng bộ lọc **Status = Publish** để kiểm tra các khóa học đã sẵn sàng thêm vào lớp học.
5. Nên dùng bộ lọc **Status = Block** để kiểm tra các khóa học đang bị chặn, không thể thêm vào lớp học.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                    | Nguyên nhân                                                              | Cách xử lý                                                           |
| ----------------------------------- | ------------------------------------------------------------------------ | -------------------------------------------------------------------- |
| Không thấy menu Course 4 Level      | Tài khoản chưa được cấp quyền truy cập chức năng                         | Liên hệ Admin hệ thống để kiểm tra phân quyền                        |
| Không tìm thấy khóa học             | Từ khóa hoặc điều kiện lọc chưa đúng                                     | Kiểm tra lại tên khóa học, Program, Status, Type hoặc chọn **Reset** |
| Không thấy khóa học vừa tạo         | Danh sách đang bị lọc bởi điều kiện cũ                                   | Chọn **Reset** hoặc kiểm tra lại bộ lọc                              |
| Không lọc được theo ngày            | From date/To date chưa đúng hoặc khoảng thời gian không có dữ liệu       | Kiểm tra lại khoảng thời gian và chọn **Search**                     |
| Không thấy nút Create Course        | Tài khoản chưa có quyền tạo khóa học                                     | Liên hệ Admin để kiểm tra phân quyền                                 |
| Không thao tác được tại menu Action | Tài khoản chưa có quyền hoặc trạng thái khóa học không cho phép thao tác | Kiểm tra quyền tài khoản và trạng thái khóa học                      |
| Khóa học không thêm được vào lớp    | Khóa học đang ở trạng thái Block hoặc chưa đủ điều kiện sử dụng          | Kiểm tra trạng thái khóa học trước khi thêm vào lớp                  |
