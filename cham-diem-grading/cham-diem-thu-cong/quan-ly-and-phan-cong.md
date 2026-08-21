# Quản lý & phân công

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Mentor chính (giao người chấm), Mentor (xem bài được giao)

**Đường dẫn:** Class → Test/Quiz (Danh sách bài làm) / Class Detail → Mark / Class → Grading List
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* User đăng nhập thành công vào hệ thống.
* Học viên nộp bài thành công.
* Tài khoản có quyền xem bài làm của học viên.
* Người dùng được giao chấm bài làm của học viên.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>1. Giao người chấm bài (Assign Grader)</summary>

{% stepper %}
{% step %}
**Truy cập danh sách bài làm:** Mentor chính truy cập màn Danh sách bài làm của từng Test/Quiz.
{% endstep %}

{% step %}
**Chọn bài cần giao:** Tick checkbox ở đầu mỗi học viên (có thể chọn nhiều). Danh sách người chấm là danh sách Mentor của lớp.
{% endstep %}

{% step %}
**Chọn người chấm:** Chọn **Assign Grader** → chọn người chấm.
{% endstep %}

{% step %}
**Lưu:** Chọn **Save** để lưu thông tin. Ngay sau khi assign, hệ thống gửi thông báo cho mentor được giao chấm.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>2. Quản lý bài cần chấm theo Lớp (màn Mark)</summary>

**Truy cập:** Người dùng truy cập màn **Mark** tại Class Detail để xem danh sách bài cần chấm của mình. Giao diện gồm 2 phần: Filter và Danh sách bài chấm.

**Thông tin hiển thị:**

| **Cột**          | **Mô tả**                                  |
| ---------------- | ------------------------------------------ |
| Student name     | Tên học viên                               |
| Test/quiz        | Tên bài test/quiz                          |
| Status           | Trạng thái chấm điểm                       |
| Submission time  | Thời gian nộp bài                          |
| Grading attempts | Số lần chấm điểm                           |
| Final score      | Điểm cuối cùng                             |
| Grader           | Người chấm (chỉ hiển thị với Mentor chính) |
| Comment          | Bình luận                                  |

**Tìm kiếm & lọc:**

* Search by: Student name.
* Filter by: Status, Test/Quiz, Mentor (chỉ Mentor chính có filter này).

_Lưu ý: Mentor thường chỉ xem bài test/quiz bản thân được giao; Mentor chính xem được tất cả._

</details>

<details>

<summary>3. Quản lý bài cần chấm theo cá nhân (Grading List)</summary>

**Truy cập:** Người dùng truy cập màn **Grading List** tại sub-menu **Class** để xem danh sách bài cần chấm ở tất cả các lớp học. Giao diện gồm 2 phần: Filter và Danh sách bài chấm.

**Thông tin hiển thị:**

| **Cột**          | **Mô tả**            |
| ---------------- | -------------------- |
| Student name     | Tên học viên         |
| Test/quiz        | Tên bài test/quiz    |
| Status           | Trạng thái chấm điểm |
| Submission time  | Thời gian nộp bài    |
| Grading attempts | Số lần chấm điểm     |
| Final score      | Điểm cuối cùng       |
| Comment          | Bình luận            |

**Tìm kiếm & lọc:**

* Search by: Student name.
* Filter by: Status, Class, Test/Quiz.

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ Mentor chính mới có quyền giao người chấm (Assign Grader) và có filter Mentor tại màn Mark.
2. Grading List tổng hợp bài cần chấm ở **tất cả các lớp**, còn màn Mark chỉ theo **một lớp**.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống             | Nguyên nhân                         | Hướng dẫn khắc phục                                              |
| ---------------------------- | ----------------------------------- | ---------------------------------------------------------------- |
| Không thấy nút Assign Grader | Tài khoản không phải Mentor chính   | Chỉ Mentor chính mới giao được người chấm                        |
| Không thấy bài cần chấm      | Chưa được giao chấm hoặc sai bộ lọc | Kiểm tra lại filter Status/Class/Test-Quiz; liên hệ Mentor chính |
