# Xem danh sách khóa học (Course List)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn Admin cách sử dụng chức năng **Xem danh sách khóa học** trên hệ thống vận hành **OPS**.

Chức năng này cho phép Admin xem toàn bộ danh sách khóa học đã được tạo trên hệ thống, đồng thời hỗ trợ tìm kiếm, lọc và sắp xếp danh sách khóa học theo các tiêu chí như tên khóa học, chương trình, trạng thái, loại khóa học và khoảng thời gian tạo/cập nhật.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                     | Quyền hạn                                                                                                         |
| --------- | ------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành khóa học            | Có quyền xem danh sách, tìm kiếm/lọc và truy cập các thao tác quản lý khóa học theo phân quyền                    |
| SX        | Người phụ trách học thuật/nội dung khóa học | Có thể xem danh sách khóa học để kiểm tra thông tin chương trình, loại khóa học, trạng thái và thời gian cập nhật |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Course List
* **Module liên quan:**
  * Program Category
  * Subject Category
  * Class
  * Resources
  * Certificates
  * Learning Schedule

### 1.4 Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành OPS.
* Tài khoản người dùng có quyền truy cập nhóm chức năng **Course**.
* Tài khoản người dùng có quyền xem danh sách khóa học tại màn hình **Course 4 Level**.

## II. Tổng Quan Giao Diện

![](<.gitbook/assets/image (952)>)

Màn hình **Course 4 Level** hiển thị danh sách các khóa học đã được tạo trên hệ thống. Admin có thể sử dụng khu vực bộ lọc phía trên để tìm kiếm hoặc thu hẹp danh sách khóa học cần xem.

Người dùng truy cập chức năng theo đường dẫn:

**Academic Management → Course & Materials → Course 4 Level**

Tại màn hình này, Admin có thể:

* Xem danh sách khóa học.
* Tìm kiếm khóa học theo tên.
* Lọc khóa học theo Program, Status, Type và khoảng thời gian.
* Sắp xếp danh sách khóa học.
* Xem nhanh thông tin loại khóa học, chương trình, trạng thái và ngày tạo/cập nhật.
* Truy cập menu thao tác của từng khóa học.
* Chọn **Create Course** để bắt đầu tạo khóa học mới nếu có quyền.

### Các thành phần chính trên màn hình

| Khu vực / Thành phần        | Mô tả                                                                                       |
| --------------------------- | ------------------------------------------------------------------------------------------- |
| **Search course name**      | Cho phép Admin nhập từ khóa để tìm kiếm khóa học theo tên.                                  |
| **Program**                 | Cho phép lọc danh sách khóa học theo chương trình học.                                      |
| **Status**                  | Cho phép lọc danh sách khóa học theo trạng thái.                                            |
| **Type**                    | Cho phép lọc danh sách khóa học theo loại khóa học.                                         |
| **Sort by**                 | Cho phép sắp xếp danh sách khóa học theo tiêu chí được chọn.                                |
| **From date**               | Lọc danh sách khóa học từ ngày bắt đầu.                                                     |
| **To date**                 | Lọc danh sách khóa học đến ngày kết thúc.                                                   |
| **Reset**                   | Xóa toàn bộ điều kiện tìm kiếm/lọc đã nhập.                                                 |
| **Search**                  | Thực hiện tìm kiếm/lọc danh sách khóa học theo điều kiện đã nhập.                           |
| **Create Course**           | Tạo mới khóa học. Chức năng này chỉ hiển thị/thao tác được nếu Admin có quyền tạo khóa học. |
| **Bảng danh sách khóa học** | Hiển thị danh sách các khóa học thỏa mãn điều kiện tìm kiếm/lọc.                            |
| **Action/Menu ba chấm**     | Cho phép Admin mở danh sách thao tác với từng khóa học theo quyền được cấp.                 |
| **Phân trang**              | Cho phép chuyển trang và điều chỉnh số lượng bản ghi hiển thị trên mỗi trang.               |

### Ý nghĩa trạng thái khóa học

Theo user guide gốc, Admin có thể lọc khóa học theo các trạng thái: **Draft, Publish, Lock, Block**.

| Trạng thái  | Ý nghĩa                                                                                                             |
| ----------- | ------------------------------------------------------------------------------------------------------------------- |
| **Draft**   | Trạng thái nháp, đồng thời là trạng thái mặc định của khóa học sau khi được tạo.                                    |
| **Publish** | Trạng thái khóa học đã được Admin chuyển thủ công từ Draft sang Publish để sẵn sàng thêm vào lớp học.               |
| **Lock**    | Trạng thái được hệ thống tự động chuyển sang khi lớp học chứa khóa học đó đã có ít nhất một học viên tiến hành học. |
| **Block**   | Trạng thái khóa học không thể được thêm vào lớp học.                                                                |

### Ý nghĩa loại khóa học

Theo user guide gốc, danh sách loại khóa học gồm **Foundation Course, Trial Course, Practice Course, Normal Course**.

| Loại khóa học         | Ý nghĩa                                                                                                                        |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| **Foundation Course** | Khóa học nền tảng. Mỗi khóa học nền tảng được gắn tương ứng với level của học viên.                                            |
| **Trial Course**      | Khóa học thử.                                                                                                                  |
| **Practice Course**   | Khóa luyện tập.                                                                                                                |
| **Normal Course**     | Khóa học thường. Loại khóa học này có thể có yêu cầu tiên quyết là học viên cần hoàn thành một số khóa học nền tảng nhất định. |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Xem danh sách khóa học

{% stepper %}
{% step %}
#### Truy cập màn hình Course 4 Level

Admin truy cập theo đường dẫn:

**Academic Management → Course & Materials → Course 4 Level**

Hệ thống hiển thị màn hình danh sách khóa học.

![](<.gitbook/assets/image (457)>)
{% endstep %}

{% step %}
#### Xem thông tin khóa học trên danh sách

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
#### Chuyển trang nếu danh sách có nhiều khóa học

![](<.gitbook/assets/image (459)>)

Nếu danh sách có nhiều khóa học, Admin sử dụng khu vực phân trang ở cuối bảng để:

* Chuyển sang trang tiếp theo.
* Quay lại trang trước.
* Chọn số lượng khóa học hiển thị trên mỗi trang.
{% endstep %}
{% endstepper %}

### 3.2 Tìm kiếm khóa học theo tên

{% stepper %}
{% step %}
#### Nhập từ khóa

![](<.gitbook/assets/image (460)>)

Tại ô **Search course name**, Admin nhập từ hoặc cụm từ mà tên khóa học cần tìm có chứa.
{% endstep %}

{% step %}
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học có tên phù hợp với từ khóa đã nhập.

![](<.gitbook/assets/image (461)>)
{% endstep %}
{% endstepper %}

### 3.3 Lọc khóa học theo Program

{% stepper %}
{% step %}
#### Chọn Program

![](<.gitbook/assets/image (462)>)

Tại trường **Program**, Admin chọn một giá trị trong danh sách Program có sẵn.
{% endstep %}

{% step %}
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học thuộc Program đã chọn.

![](<.gitbook/assets/image (463)>)
{% endstep %}
{% endstepper %}

### 3.4 Lọc khóa học theo Status

{% stepper %}
{% step %}
#### Chọn Status

![](<.gitbook/assets/image (464)>)

Tại trường **Status**, Admin chọn một trong các trạng thái:

* Draft
* Publish
* Lock
* Block
{% endstep %}

{% step %}
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học tương ứng với trạng thái đã chọn.

![](<.gitbook/assets/image (465)>)
{% endstep %}
{% endstepper %}

### 3.5 Lọc khóa học theo Type

{% stepper %}
{% step %}
#### Chọn Type

![](<.gitbook/assets/image (466)>)

Tại trường **Type**, Admin chọn loại khóa học cần lọc:

* Foundation Course
* Trial Course
* Practice Course
* Normal Course
{% endstep %}

{% step %}
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học thuộc loại đã chọn.

![](<.gitbook/assets/image (467)>)
{% endstep %}
{% endstepper %}

### 3.6 Lọc khóa học theo khoảng thời gian

{% stepper %}
{% step %}
#### Nhập khoảng thời gian

![](<.gitbook/assets/image (468)>)

Admin nhập hoặc chọn khoảng thời gian tại các trường:

| Trường        | Mô tả              |
| ------------- | ------------------ |
| **From date** | Ngày bắt đầu lọc.  |
| **To date**   | Ngày kết thúc lọc. |
{% endstep %}

{% step %}
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học trong khoảng thời gian đã nhập.

![](<.gitbook/assets/image (469)>)
{% endstep %}
{% endstepper %}

### 3.7 Sắp xếp danh sách khóa học

{% stepper %}
{% step %}
#### Chọn Sort by

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
#### Chọn Search

Admin chọn **Search**.

Hệ thống hiển thị danh sách khóa học theo tiêu chí sắp xếp đã chọn.

![](<.gitbook/assets/image (471)>)
{% endstep %}
{% endstepper %}

### 3.8 Xóa điều kiện tìm kiếm/lọc

{% stepper %}
{% step %}
#### Chọn Reset

![](<.gitbook/assets/image (472)>)

Admin chọn **Reset** tại khu vực tìm kiếm.
{% endstep %}

{% step %}
#### Hệ thống xóa bộ lọc

Hệ thống xóa toàn bộ điều kiện đã nhập/chọn tại các trường tìm kiếm và hiển thị lại danh sách khóa học theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

* Admin cần có quyền truy cập màn hình **Course 4 Level** để xem danh sách khóa học.
* Khóa học ở trạng thái **Block** không thể được thêm vào lớp học.
* Khóa học ở trạng thái **Lock** là khóa học đã có ít nhất một học viên tiến hành học trong lớp chứa khóa học đó.
* Các thao tác trong menu **Action** phụ thuộc vào quyền tài khoản và trạng thái hiện tại của khóa học.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

* Khi cần tìm nhanh một khóa học cụ thể, nên nhập một phần tên khóa học vào ô **Search course name** thay vì nhập đầy đủ tên.
* Khi danh sách có nhiều khóa học, nên kết hợp nhiều điều kiện như **Program + Status + Type** để thu hẹp kết quả.
* Nên dùng bộ lọc **Status = Draft** để kiểm tra các khóa học đang tạo dở/chưa publish.
* Nên dùng bộ lọc **Status = Publish** để kiểm tra các khóa học đã sẵn sàng thêm vào lớp học.
* Nên dùng bộ lọc **Status = Block** để kiểm tra các khóa học đang bị chặn, không thể thêm vào lớp học.
{% endhint %}
