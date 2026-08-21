# Lịch học tiêu chuẩn (Learning Schedule)

## Record of changes

_A - Add, M - Modify, D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin, SX

**Đường dẫn:** Academic Management → Course & Materials → Course 4 Level → Action → Learning Schedule

#### Phạm vi & Module liên quan

* **Module chính:** Operation
* **Chức năng chính:** Course 4 Level / Learning Schedule
* **Module liên quan:** Course, Course Content, Class, Calendar, Holiday Schedules, Teacher Schedule

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Course & Materials** và quyền xem/chỉnh sửa **Learning Schedule**.
* Khóa học đã được tạo trên hệ thống.
* Khóa học đã có **Course Content** nếu cần gắn nội dung học vào từng buổi.

**Learning Schedule** dùng để xác định nội dung cho từng buổi học của khóa học — là dữ liệu đầu vào để hệ thống tự động xếp lịch học cho lớp **Offline, Hybrid, Blended**.

## II. Hướng dẫn chi tiết

### Xem danh sách buổi học tiêu chuẩn

{% stepper %}
{% step %}
## Mở màn hình Learning Schedule

Người dùng chọn **Action → Learning Schedule** tại khóa học cần xem trên màn hình **Course 4 Level**. Hệ thống mở màn hình danh sách buổi học tiêu chuẩn.
{% endstep %}

{% step %}
## Xem danh sách buổi học

Người dùng xem danh sách buổi học tại màn hình **Learning Schedule**. Hệ thống hiển thị các buổi học đã được cấu hình cho khóa học.

![](<.gitbook/assets/image (576)>)

![](<.gitbook/assets/image (577)>)
{% endstep %}
{% endstepper %}

### Xem nhanh nội dung của buổi học

{% stepper %}
{% step %}
## Chọn biểu tượng Mở rộng

Người dùng chọn biểu tượng **Mở rộng** tại dòng buổi học cần xem trên màn hình **Learning Schedule**.

![](<.gitbook/assets/image (579)>)

Hệ thống hiển thị chi tiết nội dung học được gắn với buổi học đó.

![](<.gitbook/assets/image (581)>)
{% endstep %}
{% endstepper %}

### Xem chi tiết buổi học

{% stepper %}
{% step %}
## Chọn Action → View Detail

Người dùng chọn **Action → View Detail** tại buổi học cần xem trên màn hình **Learning Schedule**.

![](<.gitbook/assets/image (583)>)

Hệ thống mở màn hình thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
## Kiểm tra thông tin buổi học

Người dùng kiểm tra thông tin tại màn hình **Lesson Detail**.

![](<.gitbook/assets/image (585)>)

Hệ thống hiển thị tên buổi học, Study hour, Online LMS, View on LMS, Description và Course Content.
{% endstep %}
{% endstepper %}

### Xem lịch sử chỉnh sửa Learning Schedule

{% stepper %}
{% step %}
## Mở Version History

Người dùng chọn **Versions** tại màn hình danh sách buổi học.

![](<.gitbook/assets/image (587)>)

Hệ thống mở màn hình **Version History**.
{% endstep %}

{% step %}
## Xem danh sách phiên bản

Người dùng xem danh sách phiên bản tại màn hình **Version History**.

![](<.gitbook/assets/image (589)>)

Hệ thống hiển thị Version, Last updated và Changed by.
{% endstep %}

{% step %}
## Xem chi tiết một phiên bản

Người dùng nhấp vào tên **Version** cần xem chi tiết.

![](<.gitbook/assets/image (591)>)

Hệ thống hiển thị nội dung Learning Schedule tại phiên bản được chọn.

![](<.gitbook/assets/image (593)>)
{% endstep %}

{% step %}
## Chuyển qua phiên bản trước/sau

Người dùng chọn nút **<** hoặc **>** tại màn hình chi tiết Version nếu muốn chuyển qua phiên bản trước hoặc sau.

![](<.gitbook/assets/image (595)>)

Hệ thống hiển thị thông tin của phiên bản tương ứng.
{% endstep %}
{% endstepper %}

### Tạo mới buổi học

{% stepper %}
{% step %}
## Chọn New Lesson

Người dùng chọn **New Lesson** tại màn hình **Learning Schedule**.

![](<.gitbook/assets/image (597)>)

Hệ thống mở màn hình tạo mới buổi học.
{% endstep %}

{% step %}
## Nhập Lesson Name và Study hour

Người dùng nhập **Lesson Name** và **Study hour** (các trường bắt buộc) tại màn hình tạo mới buổi học.

![](<.gitbook/assets/image (599)>)
{% endstep %}

{% step %}
## Tick Online LMS (nếu có)

Người dùng tick **Online LMS** nếu buổi học là buổi học online trên LMS. Nếu không tick, buổi học được hiểu là buổi Offline/không phải Online LMS.
{% endstep %}

{% step %}
## Tick/bỏ tick View on LMS (với buổi Offline)

Nếu tick **View on LMS**, học viên được phép xem lại nội dung buổi học trên LMS; nếu không tick, học viên không được xem lại.
{% endstep %}

{% step %}
## Nhập Description (nếu cần)

Người dùng nhập **Description** nếu cần mô tả thêm cho buổi học.
{% endstep %}

{% step %}
## Chọn Course content

Người dùng chọn **Course content** cần gắn với buổi học. Hệ thống chỉ hiển thị các cấu phần học chưa được thêm vào buổi học nào.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình tạo mới buổi học. Hệ thống lưu thông tin và tạo mới buổi học thành công.

![](<.gitbook/assets/image (601)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa buổi học

{% stepper %}
{% step %}
## Chọn Action → Edit

Người dùng chọn **Action → Edit** tại buổi học cần chỉnh sửa trên màn hình **Learning Schedule**.

![](<.gitbook/assets/image (602)>)

Hệ thống mở màn hình chỉnh sửa buổi học.
{% endstep %}

{% step %}
## Cập nhật thông tin buổi học

Người dùng cập nhật thông tin tại màn hình chỉnh sửa.

![](<.gitbook/assets/image (603)>)

Có thể sửa Lesson Name, Study hour, Online LMS, View on LMS, Description và Course content.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình chỉnh sửa buổi học. Hệ thống lưu thông tin mới của buổi học.
{% endstep %}
{% endstepper %}

### Xóa buổi học

{% stepper %}
{% step %}
## Chọn Action → Delete

Người dùng chọn **Action → Delete** tại buổi học cần xóa trên màn hình **Learning Schedule**.

![](<.gitbook/assets/image (604)>)

Hệ thống hiển thị popup xác nhận xóa.
{% endstep %}

{% step %}
## Xác nhận xóa

Người dùng chọn **Yes** tại popup xác nhận. Hệ thống xóa buổi học khỏi Learning Schedule.
{% endstep %}
{% endstepper %}

### Khôi phục Learning Schedule từ phiên bản cũ

{% stepper %}
{% step %}
## Cách 1 — Khôi phục từ màn hình Version History

Người dùng chọn **Versions** tại màn hình **Learning Schedule** → tại màn hình **Version History**, chọn **Restore** tại phiên bản cần khôi phục.

![](<.gitbook/assets/image (605)>)

Hệ thống khôi phục Learning Schedule theo dữ liệu của phiên bản được chọn.
{% endstep %}

{% step %}
## Cách 2 — Khôi phục từ màn hình chi tiết Version

Người dùng chọn tên **Version** cần xem tại màn hình **Version History** → tại màn hình chi tiết của phiên bản, chọn **Restore**.

![](<.gitbook/assets/image (606)>)

Hệ thống khôi phục Learning Schedule theo dữ liệu của phiên bản đang xem.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Learning Schedule là dữ liệu đầu vào để hệ thống xếp lịch học tự động cho lớp **Offline, Hybrid, Blended**.
2. Các trường bắt buộc khi tạo/chỉnh sửa buổi học: **Lesson Name, Study hour, Course content**.
3. Checkbox **Online LMS** dùng để đánh dấu buổi học là buổi học Online trên LMS.
4. Trường **View on LMS** chỉ áp dụng với buổi học Offline (không tick Online LMS): tick → học viên xem lại được nội dung trên LMS; không tick → không xem lại được.
5. Trường **Course content** chỉ hiển thị các cấu phần học chưa được thêm vào buổi học nào; khi đã gắn vào một buổi, cấu phần đó không còn hiển thị để chọn ở buổi khác.
6. Mỗi lần thay đổi Learning Schedule có thể tạo ra một phiên bản lịch sử để xem lại hoặc khôi phục; phiên bản hiện tại được đánh dấu là **Current**.
7. Khi khôi phục phiên bản cũ, Learning Schedule hiện tại sẽ được thay thế bằng nội dung của phiên bản được khôi phục.

### Quy tắc trường thông tin buổi học

| Trường thông tin | Bắt buộc | Quy tắc                                                                                   |
| ---------------- | -------- | ----------------------------------------------------------------------------------------- |
| Lesson Name      | Có       | Tên buổi học, hiển thị trên danh sách Learning Schedule và lịch học.                      |
| Study hour       | Có       | Số giờ học dự kiến của buổi học.                                                          |
| Online LMS       | Không    | Tick nếu buổi học là buổi học Online trên LMS.                                            |
| View on LMS      | Không    | Chỉ áp dụng với buổi Offline. Cho phép/không cho phép học viên xem lại nội dung trên LMS. |
| Description      | Không    | Mô tả bổ sung cho buổi học.                                                               |
| Course content   | Có       | Nội dung học gắn với buổi học. Chỉ hiển thị cấu phần học chưa được gắn vào buổi nào khác. |

### Quy tắc Version History

| Quy tắc             | Mô tả                                                                                          |
| ------------------- | ---------------------------------------------------------------------------------------------- |
| Version             | Mỗi phiên bản thể hiện một lần thay đổi Learning Schedule.                                     |
| Current             | Phiên bản hiện tại được đánh dấu là Current.                                                   |
| Last updated        | Ghi nhận thời điểm phiên bản được tạo/cập nhật.                                                |
| Changed by          | Ghi nhận người thực hiện thay đổi.                                                             |
| View version detail | Người dùng có thể mở từng version để xem chi tiết nội dung Learning Schedule tại thời điểm đó. |
| Restore             | Người dùng có thể khôi phục Learning Schedule từ phiên bản cũ nếu có quyền.                    |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                           | Nguyên nhân                                                            | Cách xử lý                                                           |
| ------------------------------------------ | ---------------------------------------------------------------------- | -------------------------------------------------------------------- |
| Không lưu được buổi học                    | Chưa nhập đủ trường bắt buộc (Lesson Name, Study hour, Course content) | Nhập đầy đủ các trường bắt buộc rồi bấm Save                         |
| Không thấy Course content cần gắn          | Cấu phần học đã được gắn vào buổi học khác                             | Mỗi cấu phần chỉ gắn được 1 buổi; gỡ khỏi buổi cũ nếu cần đổi        |
| Không thấy/không tick được View on LMS     | Buổi học đang được tick **Online LMS**                                 | View on LMS chỉ áp dụng cho buổi Offline (không tick Online LMS)     |
| Lịch học tự động chưa đúng                 | Learning Schedule chưa cấu hình đầy đủ buổi/nội dung                   | Rà soát lại các buổi học và Course content trong Learning Schedule   |
| Khôi phục nhầm phiên bản                   | Chọn sai Version khi Restore                                           | Mở Version History, xem chi tiết và Restore đúng phiên bản mong muốn |
| Không thực hiện được tạo/sửa/xóa/khôi phục | Tài khoản chưa có quyền tương ứng                                      | Liên hệ quản trị để được cấp quyền với Learning Schedule             |
