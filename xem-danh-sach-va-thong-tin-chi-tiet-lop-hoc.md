# xem danh sach va thong tin chi tiet lop hoc

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 25, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Ops User, CX User

**Đường dẫn:** Academic Management → Class → Class List
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Class List / Class Detail
* **Module liên quan:** Course, Student, Mentor, Teacher, Test/Quiz, Resources, Examination, Marks
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class**.
* Tài khoản có quyền xem danh sách lớp học.
* Tài khoản có quyền xem thông tin chi tiết lớp học.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách lớp học</summary>

{% stepper %}
{% step %}
## Chọn Class List tại menu Class

Người dùng chọn **Class List** tại menu **Class**. Hệ thống hiển thị màn hình **Class List**.

<figure><img src="https://sapp-academy.gitbook.io/files/dCKTKeWGavTzMu1joieo" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Xem danh sách lớp học

Người dùng xem danh sách lớp học tại bảng dữ liệu trên màn hình **Class List**. Hệ thống hiển thị danh sách theo thời gian tạo giảm dần.

Các cột thông tin trong bảng danh sách:

| Cột thông tin           | Mô tả                                                            |
| ----------------------- | ---------------------------------------------------------------- |
| **#**                   | Số thứ tự của lớp học trên danh sách.                            |
| **Class**               | Tên lớp học. Người dùng có thể nhấp vào tên lớp để xem chi tiết. |
| **Code**                | Mã lớp học.                                                      |
| **Construction Mode**   | Hình thức học của lớp.                                           |
| **Number Of Students**  | Số lượng học viên hiện có trong lớp.                             |
| **Status**              | Trạng thái hiện tại của lớp học.                                 |
| **Class Foundation**    | Hiển thị lớp Foundation liên quan nếu lớp có gắn Foundation.     |
| **Action/Menu ba chấm** | Cho phép thao tác với lớp học tương ứng.                         |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tìm kiếm/lọc lớp học</summary>

{% stepper %}
{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng nhập hoặc chọn điều kiện tìm kiếm tại vùng bộ lọc của màn hình **Class List**.

<figure><img src="https://sapp-academy.gitbook.io/files/wfSGL2SwwTMXVKYqiQME" alt=""><figcaption></figcaption></figure>

Có thể lọc theo các trường: tên/mã lớp (Search by name and code), Code, Program, Subject, Status, Facility, Construction Mode (Blended, Hybrid, Online, Recorded Online...), Type, Class Owner, CX Admin, Sort by hoặc khoảng thời gian (From date - To date).
{% endstep %}

{% step %}
## Chọn Search để áp dụng

Người dùng chọn **Search** để áp dụng điều kiện. Hệ thống hiển thị danh sách lớp học thỏa mãn điều kiện đã nhập.
{% endstep %}

{% step %}
## Chọn Reset để xóa điều kiện

Người dùng chọn **Reset** để xóa toàn bộ điều kiện tìm kiếm. Hệ thống hiển thị lại danh sách lớp học theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem thông tin chi tiết lớp học</summary>

{% stepper %}
{% step %}
## Mở màn hình Class Detail

Người dùng nhấp vào **tên lớp học** tại màn hình **Class List**. Hệ thống mở màn hình **Class Detail** của lớp được chọn.

<figure><img src="https://sapp-academy.gitbook.io/files/FI5WQrZNcRFVBFQ5Ycfy" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tab Overview — thông tin tổng quan

<figure><img src="https://sapp-academy.gitbook.io/files/i1WqfD6DBaulbyGPhWhQ" alt=""><figcaption></figcaption></figure>

Người dùng chọn tab **Overview** để xem thông tin tổng quan của lớp học.

| Thông tin                   | Mô tả                                                   |
| --------------------------- | ------------------------------------------------------- |
| **Name**                    | Tên lớp học.                                            |
| **Code**                    | Mã lớp học.                                             |
| **Status**                  | Trạng thái lớp học.                                     |
| **Construction Mode**       | Hình thức học của lớp.                                  |
| **Facility**                | Cơ sở của lớp học.                                      |
| **Type**                    | Loại lớp học.                                           |
| **No. of Students**         | Số lượng học viên hiện tại / số lượng học viên tối đa.  |
| **Opening at**              | Ngày mở khóa học online.                                |
| **Start Date**              | Ngày bắt đầu lớp học.                                   |
| **End Date**                | Ngày kết thúc lớp học.                                  |
| **Expire Date**             | Ngày hết hạn truy cập lớp học.                          |
| **Number of Extended Days** | Số ngày gia hạn thêm cho học viên sau khi lớp kết thúc. |
| **Reason For Extension**    | Lý do gia hạn.                                          |
| **Standard Schedule**       | Lịch học cố định của lớp.                               |
| **Classroom name**          | Tên phòng học.                                          |
| **Course**                  | Khóa học được gắn với lớp.                              |
| **Exam**                    | Kỳ thi được gắn với lớp.                                |
| **Class Owner**             | Người phụ trách lớp.                                    |
| **CX Admin**                | Người phụ trách CX Admin của lớp.                       |
| **Description**             | Mô tả lớp học.                                          |
{% endstep %}

{% step %}
## Tab Calendar — lịch học của lớp

Người dùng chọn tab **Calendar** để xem lịch học theo dạng Calendar. (Chỉ hiển thị với lớp có Construction Mode = Offline, Blended, Live\_Online, Hybrid)

<figure><img src="https://sapp-academy.gitbook.io/files/oBwt0YfiXAmENvyzliCl" alt=""><figcaption></figcaption></figure>

| Thành phần              | Mô tả                                            |
| ----------------------- | ------------------------------------------------ |
| **Generate Schedule**   | Tạo lịch học tự động cho lớp nếu có quyền.       |
| **Add Lesson**          | Thêm buổi học mới vào lịch.                      |
| **Bộ điều hướng tháng** | Chuyển sang tháng trước hoặc tháng sau.          |
| **Today**               | Quay về ngày hiện tại.                           |
| **Month view**          | Hiển thị lịch theo tháng.                        |
| **Legend**              | Chú thích màu/biểu tượng của từng loại buổi học. |

Ý nghĩa chú thích trên Calendar:

| Chú thích       | Ý nghĩa                                 |
| --------------- | --------------------------------------- |
| **Online**      | Buổi học online.                        |
| **Live Online** | Buổi học live online.                   |
| **Offline**     | Buổi học offline.                       |
| **Cancelled**   | Buổi học đã bị hủy.                     |
| **Holiday**     | Ngày nghỉ/lịch nghỉ lễ.                 |
| **Case Study**  | Buổi học hoặc nội dung có Case Study.   |
| **Test**        | Buổi học hoặc nội dung có bài kiểm tra. |
| **Key Content** | Nội dung học trọng tâm.                 |
{% endstep %}

{% step %}
## Tab Progress — tiến độ học tập

Người dùng chọn tab **Progress** để xem tiến độ học tập của lớp. Hệ thống hiển thị thông tin tiến độ giảng dạy theo dữ liệu giảng viên đã khai báo.

<figure><img src="https://sapp-academy.gitbook.io/files/YS8MqsZwnckKpuO2mLSS" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tab Students — danh sách học viên

Người dùng chọn tab **Students** để xem danh sách học viên đang thuộc lớp học.

<figure><img src="https://sapp-academy.gitbook.io/files/3keMilXJGvC8cQ7aXUNp" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tab Mentors — danh sách trợ giảng

Người dùng chọn tab **Mentors** để xem danh sách trợ giảng đang được gắn với lớp học.

<figure><img src="https://sapp-academy.gitbook.io/files/U7mkltDbHUqoSABLF1gF" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tab Teachers — danh sách giảng viên

Người dùng chọn tab **Teachers** để xem danh sách giảng viên đang được gắn với lớp học.

<figure><img src="https://sapp-academy.gitbook.io/files/M9hyWxNO6OrAuoXZ3jvu" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tab Test/Quiz — danh sách bài kiểm tra

Người dùng chọn tab **Test/Quiz** để xem danh sách bài kiểm tra trong khóa học gắn với lớp (nếu khóa học có cấu hình Test/Quiz).

<figure><img src="https://sapp-academy.gitbook.io/files/gba1ru76fixiduBPu1NE" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần có quyền xem danh sách lớp học để truy cập màn hình **Class List**.
2. Người dùng cần có quyền xem chi tiết lớp học để mở màn hình **Class Detail**.
3. Danh sách lớp học mặc định hiển thị theo thời gian tạo giảm dần.
4. Có thể tìm kiếm/lọc lớp học theo nhiều điều kiện: tên/mã lớp, Program, Subject, Status, Facility, Construction Mode, Type, Class Owner, CX Admin và khoảng thời gian.
5. Khi nhấp vào tên lớp học, hệ thống mở màn hình chi tiết lớp học.
6. Tab **Calendar** chỉ hiển thị với lớp có Construction Mode = Offline, Blended, Live\_Online, Hybrid.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Khi cần tìm nhanh một lớp cụ thể, nên nhập một phần tên lớp hoặc mã lớp vào ô **Search by name and code**.
2. Khi có nhiều lớp cùng chương trình, nên kết hợp bộ lọc **Program + Subject** để thu hẹp kết quả.
3. Nên dùng **Construction Mode** để phân biệt nhanh lớp Blended, Hybrid, Online hoặc Offline.
4. Có thể kiểm tra cột **Class Foundation** để biết lớp có liên quan đến lớp Foundation hay không.
5. Khi cần kiểm tra lịch học, nên vào tab **Calendar** thay vì chỉ xem ngày bắt đầu/kết thúc ở Overview.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                        | Nguyên nhân                                                              | Cách xử lý                                                  |
| --------------------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Không tìm thấy lớp học                  | Điều kiện tìm kiếm/lọc chưa đúng hoặc quá hẹp                            | Kiểm tra lại bộ lọc, bấm Reset để về danh sách mặc định     |
| Danh sách không hiển thị dữ liệu mới    | Danh sách đang bị lọc theo điều kiện trước đó                            | Chọn Reset để xóa bộ lọc                                    |
| Không mở được màn hình Class Detail     | Tài khoản chưa có quyền xem chi tiết lớp học                             | Liên hệ quản trị để được cấp quyền xem chi tiết lớp học     |
| Không thấy tab Calendar                 | Lớp có Construction Mode không thuộc Offline/Blended/Live\_Online/Hybrid | Tab Calendar chỉ áp dụng cho các Construction Mode nói trên |
| Không truy cập được màn hình Class List | Tài khoản chưa có quyền xem danh sách lớp học                            | Liên hệ quản trị để được cấp quyền truy cập module Class    |
