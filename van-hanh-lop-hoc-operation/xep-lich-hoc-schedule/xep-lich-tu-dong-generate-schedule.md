# Xếp lịch tự động (Generate Schedule)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, CX

**Đường dẫn:** Class → Class List → Class Detail → Calendar
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Class Calendar / Generate Schedule
* **Module liên quan:** Class List, Class Detail, Calendar, Course, Learning Schedule, Course Content, Classroom, Teacher, Holiday Schedules, Student Calendar, Teacher Calendar, Receptionist Schedule
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class** và quyền thao tác trên **Class Calendar**.
* Lớp học có **Type = Lesson**.
* Lớp học có **Construction Mode = Offline, Blended hoặc Live Online**.
* Lớp học có **Status = Draft hoặc Public**.
* Course của lớp đã được cấu hình **Learning Schedule**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Tạo lịch học tự động</summary>

{% stepper %}
{% step %}
**Truy cập Class Calendar**

Người dùng truy cập **Class List → Class Detail → Calendar** tại lớp cần xếp lịch. Hệ thống hiển thị màn hình **Class Calendar**.
{% endstep %}

{% step %}
**Chọn Generate Schedule**

Người dùng chọn **Generate Schedule** tại màn hình **Calendar**.

<figure><img src="../../.gitbook/assets/image (818).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Generate Schedule** để kiểm tra thông tin trước khi tạo lịch.

<figure><img src="../../.gitbook/assets/image (820).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Kiểm tra/điều chỉnh Start Date**

Người dùng kiểm tra hoặc điều chỉnh **Start Date**. Start Date không được là ngày trong quá khứ và không được trùng ngày nghỉ lễ năm.
{% endstep %}

{% step %}
**Kiểm tra/điều chỉnh Standard Schedule**

Người dùng kiểm tra hoặc điều chỉnh **Standard Schedule**. Có thể thêm tối đa 3 lịch học tiêu chuẩn hoặc xóa lịch học tiêu chuẩn không cần dùng.
{% endstep %}

{% step %}
**Chọn Generate**

Người dùng chọn **Generate**. Hệ thống tạo lịch học tự động cho lớp theo Learning Schedule, Start Date, Standard Schedule và lịch nghỉ lễ.
{% endstep %}

{% step %}
**Hủy thao tác (nếu cần)**

Người dùng chọn **Cancel** hoặc biểu tượng đóng nếu muốn hủy. Hệ thống thoát khỏi màn hình Generate Schedule và không tạo lịch học mới.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thêm phòng học cho lớp sau khi tạo lịch tự động</summary>

{% stepper %}
{% step %}
**Mở tab Add Classroom**

Người dùng chọn biểu tượng **Edit** tại tab **Add Classroom** trên màn hình **Generate Schedule**.

<figure><img src="../../.gitbook/assets/image (821).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Add Classroom**.
{% endstep %}

{% step %}
**Mở danh sách phòng học**

Người dùng chọn **Add Classroom** hoặc biểu tượng **Edit** tại màn hình **Add Classroom**.

<figure><img src="../../.gitbook/assets/image (822).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở danh sách phòng học phù hợp với lớp.
{% endstep %}

{% step %}
**Tìm kiếm/lọc phòng học**

Người dùng tìm kiếm theo **Name, Code** hoặc lọc theo **Type** nếu cần.
{% endstep %}

{% step %}
**Chọn phòng học và Add**

Người dùng chọn một phòng học trong danh sách, sau đó chọn **Add** để gắn phòng học cho lớp. Hệ thống quay lại màn hình Add Classroom và hiển thị phòng học đã chọn.
{% endstep %}

{% step %}
**Nhập Link Meeting (Live Online)**

Người dùng nhập **Link Meeting** nếu lớp có Construction Mode = **Live Online**.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save** tại màn hình **Add Classroom**. Hệ thống cập nhật Classroom và Link Meeting vào các lịch học được tạo tự động của lớp.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa lịch học được tạo tự động</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần chỉnh sửa**

Người dùng chọn buổi học muốn chỉnh sửa tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
**Chọn Edit**

Người dùng chọn **Edit** tại màn hình chi tiết buổi học.

<figure><img src="../../.gitbook/assets/image (824).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình chỉnh sửa buổi học.

<figure><img src="../../.gitbook/assets/image (825).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật thông tin buổi học**

Người dùng cập nhật thông tin cần chỉnh sửa tại màn hình **Edit Lesson** theo các trường được phép tùy Learning Mode và loại lớp.

Có thể chỉnh sửa **Lesson Date** (hệ thống kiểm tra rule trùng lịch và thứ tự buổi), **Classroom**, **Teacher** (cập nhật lịch lớp, xóa lịch giảng viên cũ và tạo request cho giảng viên mới), **Course Content** (cần kiểm tra lại giảng viên liên quan).
{% endstep %}

{% step %}
**Tick/bỏ tick Don't Reschedule**

Người dùng tick hoặc bỏ tick **Don't Reschedule** để kiểm soát việc sắp xếp lại toàn bộ lịch học. Nếu tick, hệ thống không sắp xếp lại toàn bộ lịch học của lớp.
{% endstep %}

{% step %}
**Nhập Reason for Change (nếu Offline/Live Online)**

**Reason for Change** là trường bắt buộc khi chỉnh sửa buổi học Offline/Live Online.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save** tại màn hình **Edit Lesson**. Hệ thống lưu thay đổi và cập nhật lịch lớp học, lịch giảng viên, lịch phòng học và lịch trực lễ tân.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xử lý khi tick Don't Reschedule</summary>

{% stepper %}
{% step %}
**Tick Don't Reschedule**

Người dùng tick **Don't Reschedule** tại màn hình **Edit Lesson**.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save**. Hệ thống hiển thị popup xác nhận: _"Are you sure you don't want to reschedule this lesson?"_
{% endstep %}

{% step %}
**Chọn No (quay lại)**

Người dùng chọn **No** nếu muốn quay lại màn hình chỉnh sửa. Hệ thống quay lại màn hình Edit Lesson và giữ nguyên lịch của lớp.
{% endstep %}

{% step %}
**Chọn Yes (đồng ý không reschedule)**

Người dùng chọn **Yes** nếu đồng ý. Hệ thống chuyển loại buổi học từ lịch tự động sang lịch thủ công và kiểm tra lại thông tin theo rule lịch thủ công.
{% endstep %}

{% step %}
**Hệ thống lưu lịch học**

Hệ thống lưu lịch học nếu thông tin hợp lệ. Sau khi lưu thành công, checkbox **Don't Reschedule** sẽ không còn hiển thị trong các lần chỉnh sửa tiếp theo của buổi học này.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Hủy lịch học được tạo tự động</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần hủy**

Người dùng chọn buổi học muốn hủy tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
**Chọn Schedule Later**

Người dùng chọn **Schedule Later** tại màn hình chi tiết buổi học.

<figure><img src="../../.gitbook/assets/image (826).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup nhập lý do hủy.

<figure><img src="../../.gitbook/assets/image (827).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập lý do hủy**

Người dùng nhập lý do hủy buổi học tại popup.
{% endstep %}

{% step %}
**Chọn Submit**

Người dùng chọn **Submit** tại popup hủy buổi học. Hệ thống hủy buổi học và cập nhật trạng thái buổi học trên Calendar.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Kích hoạt lại buổi học đã hủy</summary>

{% stepper %}
{% step %}
**Chọn buổi học đã hủy**

Người dùng chọn buổi học đã hủy tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học đã hủy.
{% endstep %}

{% step %}
**Chọn Edit**

Người dùng chọn **Edit** tại màn hình chi tiết buổi học đã hủy.

<figure><img src="../../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Edit Lesson**.
{% endstep %}

{% step %}
**Chỉnh sửa thông tin lịch học mới**

Người dùng chỉnh sửa thông tin lịch học mới tại màn hình **Edit Lesson** theo rule chỉnh sửa lịch học được tạo tự động.
{% endstep %}

{% step %}
**Chọn Schedule**

Người dùng chọn **Schedule** tại màn hình **Edit Lesson**.

<figure><img src="../../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>

Hệ thống kích hoạt lại buổi học và cập nhật lịch học viên, lịch giảng viên, lịch phòng học, lịch trực lễ tân.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa lịch học được tạo tự động</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần xóa**

Người dùng chọn buổi học muốn xóa tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
**Chọn Delete**

Người dùng chọn **Delete** tại màn hình chi tiết buổi học.

<figure><img src="../../.gitbook/assets/image (830).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup xác nhận xóa.
{% endstep %}

{% step %}
**Xác nhận xóa**

Người dùng chọn **Yes** để xóa bản ghi lịch học và quay lại màn hình Calendar; chọn **No** để hủy thao tác và giữ nguyên buổi học.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Xếp lịch tự động chỉ áp dụng cho lớp có **Type = Lesson** và **Construction Mode = Offline, Blended hoặc Live Online**; lớp cần có **Status = Draft hoặc Public**.
2. Course của lớp bắt buộc phải có **Learning Schedule** trước khi generate lịch tự động.
3. **Start Date** không được là ngày trong quá khứ và không được trùng ngày nghỉ lễ năm. Sau khi nhập Start Date, thứ của Start Date trở thành lịch học đầu tiên và không thể sửa.
4. Standard Schedule cho phép tối thiểu 1 lịch và tối đa 3 lịch; mỗi lịch bắt buộc có **Day of Week** và **Start Time - End Time**.
5. Nếu lịch tự động trùng ngày nghỉ lễ năm, hệ thống tự động lùi sang lịch tiếp theo theo Standard Schedule.
6. Buổi Online LMS tự động xếp ngay sau buổi Offline/Live Online trước đó; bài test online (Midterm/Final Test) tự động xếp ngay sau buổi Offline hoặc Online trước đó.
7. Khi chỉnh sửa lịch của lớp Public (trừ trường **View on LMS**), hệ thống gửi thông báo qua LMS/email tới học viên và giảng viên.
8. Khi xóa lịch học thành công, toàn bộ Course Content của buổi đó có thể được chọn vào buổi khác.
9. Buổi học đã hủy hiển thị màu xanh dương trên Class Calendar; sau khi hủy, các buổi khác có thể được xếp vào ngày học đó.
{% endhint %}

### Quy tắc Standard Schedule

| Quy tắc                 | Mô tả                                                                                     |
| ----------------------- | ----------------------------------------------------------------------------------------- |
| Số lượng lịch tối thiểu | 1 lịch học tiêu chuẩn.                                                                    |
| Số lượng lịch tối đa    | 3 lịch học tiêu chuẩn.                                                                    |
| Thông tin bắt buộc      | Mỗi lịch cần có Day of Week và Start Time - End Time.                                     |
| Day of Week             | Hiển thị các thứ trong tuần và chỉ chọn 1 giá trị.                                        |
| Start Date              | Sau khi nhập Start Date, thứ của Start Date trở thành lịch học đầu tiên và không thể sửa. |
| Thứ 2 - Thứ 6           | Start Time phải từ 18:00 trở đi, End Time không vượt quá 22:00.                           |
| Thứ 7 - Chủ nhật        | Start Time phải từ 08:00 trở đi, End Time không vượt quá 22:00.                           |
| Thời lượng buổi học     | End Time - Start Time phải từ 2.5 giờ đến 3.5 giờ.                                        |

### Quy tắc hệ thống tạo lịch tự động

**Lịch Offline / Live Online**

| Quy tắc                | Mô tả                                                               |
| ---------------------- | ------------------------------------------------------------------- |
| Cách xếp lịch          | Hệ thống tự động sắp xếp ngày học liên tiếp theo Standard Schedule. |
| Ngày nghỉ lễ           | Không xếp lịch trùng ngày nghỉ lễ năm.                              |
| Khi trùng ngày nghỉ lễ | Hệ thống tự động lùi sang lịch tiếp theo theo Standard Schedule.    |

**Lịch Online LMS**

| Quy tắc             | Mô tả                                                                                                                                         |
| ------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| Điều kiện           | Buổi học không chứa Midterm/Final Test.                                                                                                       |
| Cách xếp lịch       | Tự động xếp ngay sau buổi Offline/Live Online trước đó.                                                                                       |
| Deadline            | Deadline tự động là trước buổi học tiếp theo, bỏ qua lịch buổi test.                                                                          |
| Ngày nghỉ lễ        | Không xếp trùng ngày nghỉ lễ năm.                                                                                                             |
| Không có ngày trống | Nếu 2 ngày Offline/Live Online quá gần nhau, hệ thống tự động lùi buổi Offline/Live Online phía sau và xếp buổi Online LMS vào ngày trống đó. |

**Lịch Test Online**

| Quy tắc       | Mô tả                                                   |
| ------------- | ------------------------------------------------------- |
| Điều kiện     | Course Content của buổi học chỉ gồm Midterm/Final Test. |
| Cách xếp lịch | Tự động xếp ngay sau buổi Offline hoặc Online trước đó. |
| Ngày nghỉ lễ  | Không xếp trùng ngày nghỉ lễ năm.                       |

### Quy tắc thêm Classroom cho lớp

| Quy tắc                  | Mô tả                                                                         |
| ------------------------ | ----------------------------------------------------------------------------- |
| Điều kiện                | Lớp đã tạo lịch học tự động.                                                  |
| Live Online              | Chỉ hiển thị phòng học ảo có Mode = Virtual.                                  |
| Offline/Blended          | Chỉ hiển thị phòng học vật lý có Mode = Physical và gắn với Facility của lớp. |
| Status phòng học         | Chỉ hiển thị phòng học có Status = Active.                                    |
| Sức chứa phòng học       | Số lượng học viên của lớp phải ≤ sức chứa phòng học vật lý.                   |
| Trùng lịch phòng học     | Chỉ hiển thị phòng có số buổi trùng lịch ≤ 3 buổi.                            |
| Sắp xếp phòng học        | Danh sách phòng học được sắp xếp theo số buổi trùng từ nhỏ nhất đến lớn nhất. |
| Không có kết quả         | Nếu không có phòng phù hợp, hệ thống hiển thị **No matching records found.**  |
| Live Online Link Meeting | Với lớp Live Online, Link Meeting là trường bắt buộc sau khi chọn Classroom.  |

### Quy tắc chỉnh sửa Lesson Date

| Learning Mode       | Quy tắc                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------ |
| Offline/Live Online | Có thể điều chỉnh trùng lịch Offline/Live Online được tạo tự động.                         |
| Offline/Live Online | Không thể điều chỉnh trùng đồng thời lịch Offline/Live Online thủ công và lịch Online LMS. |
| Offline/Live Online | Không thể tiến lịch lên trước buổi học phía trước nó.                                      |
| Online LMS          | Không thể điều chỉnh trùng các lịch khác.                                                  |

### Quy tắc chỉnh sửa Course Content

| Quy tắc                    | Mô tả                                                       |
| -------------------------- | ----------------------------------------------------------- |
| Cấp hiển thị               | Course Content hiển thị đến cấp Unit.                       |
| Chọn nhiều cấu phần        | Người dùng có thể chọn nhiều cấu phần học.                  |
| ACCA, Cert/Dip             | Người dùng có thể chọn nhiều Section trong một buổi học.    |
| Các Program còn lại        | Người dùng không thể chọn nhiều Section trong một buổi học. |
| Sau khi đổi Course Content | Người dùng cần kiểm tra hoặc chọn lại Teacher nếu cần.      |

### Quy tắc Don't Reschedule

| Quy tắc                            | Mô tả                                                                                            |
| ---------------------------------- | ------------------------------------------------------------------------------------------------ |
| Tick Don't Reschedule              | Hệ thống không sắp xếp lại toàn bộ lịch học của lớp.                                             |
| Không tick Don't Reschedule        | Hệ thống sắp xếp lại toàn bộ lịch học của lớp.                                                   |
| Xác nhận Don't Reschedule          | Hệ thống hiển thị popup xác nhận trước khi lưu.                                                  |
| Chọn No                            | Quay lại màn Edit Lesson, lịch của lớp được giữ nguyên.                                          |
| Chọn Yes                           | Hệ thống chuyển buổi học từ lịch tự động sang lịch thủ công và kiểm tra theo rule lịch thủ công. |
| Sau khi chuyển thành lịch thủ công | Checkbox Don't Reschedule không còn hiển thị trong các lần chỉnh sửa sau.                        |

### Quy tắc hủy lịch học tự động

| Quy tắc               | Mô tả                                                                                   |
| --------------------- | --------------------------------------------------------------------------------------- |
| Điều kiện hủy         | Buổi học chưa kết thúc và lớp thỏa mãn điều kiện thao tác.                              |
| Reason                | Người dùng bắt buộc nhập lý do hủy.                                                     |
| Sau khi hủy           | Hệ thống ẩn buổi học tại lịch học viên, lịch giảng viên, lịch phòng học và lịch lễ tân. |
| Receptionist Schedule | Hệ thống xóa buổi học khỏi ca trực lễ tân.                                              |
| Email thông báo       | Gửi email hủy buổi học tới học viên, giảng viên, Facility Manager và CX.                |
| Class Calendar        | Buổi học đã hủy hiển thị màu đỏ.                                                        |
| Activate/Delete       | Tại màn chi tiết lịch đã hủy, hệ thống hiển thị nút Activate và Delete.                 |

### Quy tắc kích hoạt lại buổi học đã hủy

| Quy tắc                         | Mô tả                                                                                                                                                                                             |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Edit                            | Người dùng chọn Edit để chọn lại lịch học bù cho buổi đã hủy.                                                                                                                                     |
| Xác nhận Schedule               | Hệ thống hiển thị popup xác nhận trước khi kích hoạt lại.                                                                                                                                         |
| Sau khi Schedule thành công     | Buổi học hiển thị lại trên lịch học viên, giảng viên, phòng học và lịch trực lễ tân.                                                                                                              |
| Email thông báo                 | Gửi email thông báo lịch học bù tới học viên, giảng viên, Facility Manager và CX.                                                                                                                 |
| Nhắc cập nhật lịch bù lúc 12:00 | Vào 12:00 ngày ngay trước lịch học Offline/Live Online tiếp theo, nếu chưa chọn Lesson Date mới, hệ thống gửi email nhắc CX Admin cập nhật lịch học bù.                                           |
| Tự động cập nhật lúc 21:00      | Vào 21:00 ngày ngay trước lịch học tiếp theo, nếu chưa chọn Lesson Date mới, hệ thống tự động sửa Lesson Date thành lịch tiếp theo theo Standard Schedule và lùi các lịch buổi tiếp theo của lớp. |

### Quy tắc xóa lịch học tự động

| Quy tắc         | Mô tả                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Điều kiện xóa   | Buổi học tự động chưa diễn ra.                                                                                            |
| Xác nhận xóa    | Hệ thống hiển thị popup xác nhận trước khi xóa.                                                                           |
| Chọn Yes        | Hệ thống xóa bản ghi lịch học và quay lại màn Calendar.                                                                   |
| Chọn No         | Hệ thống hủy thao tác xóa và giữ nguyên thông tin buổi học.                                                               |
| Course Content  | Toàn bộ cấu phần của buổi học đã xóa có thể được chọn vào buổi học khác.                                                  |
| Lịch liên quan  | Lịch học viên, lịch giảng viên, lịch phòng học và lịch trực lễ tân gắn với buổi học cũng bị xóa.                          |
| Email thông báo | Nếu lớp có Status = Public và Start Date của lớp ≤ hiện tại, hệ thống gửi email thông báo hủy lịch tới các bên liên quan. |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                            | Nguyên nhân                                                    | Cách xử lý                                                            |
| ------------------------------------------- | -------------------------------------------------------------- | --------------------------------------------------------------------- |
| Không generate được lịch tự động            | Lớp không thỏa điều kiện hoặc Course chưa có Learning Schedule | Đảm bảo lớp đủ điều kiện và Course đã cấu hình Learning Schedule      |
| Không chọn được Start Date                  | Start Date là ngày quá khứ hoặc trùng ngày nghỉ lễ năm         | Chọn Start Date hợp lệ, không quá khứ, không trùng nghỉ lễ            |
| Lỗi Standard Schedule                       | Quá 3 lịch, thời lượng ngoài 2.5–3.5 giờ, hoặc khung giờ sai   | Nhập tối đa 3 lịch, thời lượng 2.5–3.5h, đúng khung giờ theo thứ      |
| Không thêm được phòng học                   | Không có phòng phù hợp (Mode, Active, sức chứa, trùng lịch)    | Chọn phòng đúng điều kiện; nếu "No matching records" thì đổi tiêu chí |
| Không nhập được Link Meeting                | Chưa chọn phòng học cho lớp Live Online                        | Chọn phòng (Virtual) trước rồi nhập Link Meeting                      |
| Không lưu được khi chỉnh sửa                | Thiếu Reason for Change (Offline/Live Online)                  | Nhập Reason for Change rồi lưu                                        |
| Buổi tự động không reschedule như mong muốn | Đã tick Don't Reschedule (chuyển sang lịch thủ công)           | Hiểu rõ tác động; bỏ tick nếu muốn hệ thống tự sắp xếp lại lịch       |
| Không xóa/hủy được buổi học                 | Buổi học đã diễn ra hoặc lớp không đủ điều kiện                | Chỉ thao tác với buổi chưa diễn ra và lớp đủ điều kiện                |
