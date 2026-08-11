# Xếp lịch thủ công (Add Lesson)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, CX/Admin lớp

**Đường dẫn:** Classes → Class List → Class Detail → Calendar
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Class Calendar / Manual Lesson Scheduling
* **Module liên quan:** Class List, Class Detail, Calendar, Course Content, Teacher, Classroom, Receptionist Schedule, Student Calendar, Teacher Calendar
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class** và quyền thao tác trên **Class Calendar**.
* Lớp học có **Type = Lesson**.
* Lớp học có **Construction Mode = Offline, Blended hoặc Live Online**.
* Lớp học có **Status = Draft hoặc Public**.
* Lớp học đã được gắn Course và có Course Content để chọn nội dung học.
{% endhint %}

{% hint style="info" %}
Các loại **Learning Mode**: **Online LMS** (học qua nội dung trên hệ thống), **Offline** (trực tiếp tại cơ sở/phòng học vật lý), **Live Online** (trực tuyến có phòng học ảo và link meeting).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Tạo lịch học thủ công</summary>

{% stepper %}
{% step %}
**Truy cập Class Calendar**

Người dùng truy cập **Class List → Class Detail → Calendar** tại lớp cần xếp lịch.

<figure><img src="../../.gitbook/assets/image (796).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị màn hình **Class Calendar**.
{% endstep %}

{% step %}
**Chọn Add Lesson hoặc click vào ngày**

Người dùng chọn **Add Lesson** hoặc click vào ngày muốn tạo lịch học trên màn hình **Calendar**.

<figure><img src="../../.gitbook/assets/image (797).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình tạo mới buổi học.

<figure><img src="../../.gitbook/assets/image (798).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Learning Mode**

Người dùng chọn **Learning Mode**. Hệ thống hiển thị các trường thông tin tương ứng với Learning Mode đã chọn.

**Buổi Online LMS:** Lesson Date (\*), Deadline (\*), Course Content (\*), Note.

**Buổi Offline / Live Online:** View on LMS, Lesson Date (\*, không chọn ngày quá khứ), Start Time - End Time (\*), Course Content (\*), Teacher (\*), Classroom (\*), Link Meeting (bắt buộc khi Live Online), Note.
{% endstep %}

{% step %}
**Nhập Lesson Date và thông tin thời gian**

Với Offline/Live Online: nhập **Start Time - End Time**. Với Online LMS: nhập **Deadline**.
{% endstep %}

{% step %}
**Chọn Course Content**

Người dùng chọn **Course Content**. Hệ thống hiển thị danh sách cấu phần học chưa được chọn vào buổi học khác. Người dùng tick chọn một hoặc nhiều cấu phần học.
{% endstep %}

{% step %}
**Chọn Teacher (Offline/Live Online)**

Người dùng chọn **Teacher**, chọn giảng viên phù hợp tại màn hình **Teacher List** và chọn **Add**.

<figure><img src="../../.gitbook/assets/image (799).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (800).png" alt=""><figcaption></figcaption></figure>

Hệ thống lưu giảng viên cho buổi học.
{% endstep %}

{% step %}
**Chọn Classroom (Offline/Live Online)**

Người dùng chọn **Classroom**, chọn phòng học phù hợp tại màn hình **Classroom List** và chọn **Add**.

<figure><img src="../../.gitbook/assets/image (801).png" alt=""><figcaption></figcaption></figure>

Hệ thống lưu phòng học cho buổi học.

<figure><img src="../../.gitbook/assets/image (802).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Link Meeting (Live Online)**

Người dùng nhập **Link Meeting** nếu buổi học có Learning Mode = Live Online.

Trường này chỉ hiển thị sau khi chọn phòng học cho buổi Live Online.

<figure><img src="../../.gitbook/assets/image (803).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Note và Save**

Người dùng nhập **Note** nếu cần, sau đó chọn **Save**. Hệ thống lưu thông tin lịch học thủ công và hiển thị buổi học trên Class Calendar.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chọn Course Content cho buổi học</summary>

{% stepper %}
{% step %}
**Chọn trường Course Content**

Người dùng chọn trường **Course Content** tại màn hình tạo/chỉnh sửa buổi học.

<figure><img src="../../.gitbook/assets/image (804).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách cấu phần học chưa được chọn vào buổi học khác.
{% endstep %}

{% step %}
**Mở rộng để xem cấu phần học nhỏ hơn**

Người dùng mở rộng các toggle để xem cấu phần học cấp nhỏ hơn.

<figure><img src="../../.gitbook/assets/image (805).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị cấu phần học đến cấp **Unit**.
{% endstep %}

{% step %}
**Tick chọn cấu phần học**

Người dùng tick chọn cấu phần học cần gắn vào buổi học. Hệ thống tự tick các cấu phần con nếu tick cấu phần cha.
{% endstep %}

{% step %}
**Bỏ tick cấu phần học**

Người dùng bỏ tick cấu phần học nếu không muốn gắn vào buổi học. Hệ thống tự bỏ tick các cấu phần con nếu bỏ tick cấu phần cha.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chọn Teacher cho buổi học</summary>

{% stepper %}
{% step %}
**Mở màn hình chọn Teacher**

Người dùng chọn **Teacher** tại màn hình tạo/chỉnh sửa buổi học. Chỉ có thể chọn Teacher sau khi đã chọn **Course Content, Lesson Date** và **Start Time - End Time**.

<figure><img src="../../.gitbook/assets/image (1291).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm/lọc giảng viên**

Người dùng tìm kiếm/lọc giảng viên tại màn hình **Teacher List** nếu cần.

<figure><img src="../../.gitbook/assets/image (1293).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn giảng viên và Add**

Người dùng chọn giảng viên phù hợp trong danh sách, sau đó chọn **Add**. Hệ thống lưu thông tin giảng viên cho buổi học.
{% endstep %}

{% step %}
**Xử lý cảnh báo vượt định mức tuần**

Người dùng chọn **Yes** tại popup cảnh báo nếu giảng viên vượt định mức tuần nhưng vẫn muốn đặt lịch. Nếu chọn **No**, hệ thống quay lại màn hình Add Teacher.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chọn Classroom cho buổi học</summary>

{% stepper %}
{% step %}
**Mở màn hình chọn Classroom**

Người dùng chọn **Classroom** tại màn hình tạo/chỉnh sửa buổi học. Hệ thống mở màn hình danh sách phòng học phù hợp.

<figure><img src="../../.gitbook/assets/image (1294).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm/lọc phòng học**

Người dùng tìm kiếm/lọc phòng học tại màn hình **Classroom List** nếu cần.

<figure><img src="../../.gitbook/assets/image (1295).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn phòng học và Add**

Người dùng chọn phòng học phù hợp trong danh sách, sau đó chọn **Add**. Hệ thống lưu thông tin phòng học cho buổi học.
{% endstep %}

{% step %}
**Nhập Link Meeting (Live Online)**

Người dùng nhập **Link Meeting** nếu buổi học có Learning Mode = Live Online.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa lịch học thủ công</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần chỉnh sửa**

Người dùng chọn buổi học muốn chỉnh sửa tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.

<figure><img src="../../.gitbook/assets/image (1297).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Edit**

Người dùng chọn **Edit** tại màn hình chi tiết buổi học. Hệ thống mở màn hình chỉnh sửa buổi học.

<figure><img src="../../.gitbook/assets/image (1296).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cập nhật thông tin**

Người dùng cập nhật thông tin cần thay đổi theo quyền và điều kiện của từng Learning Mode.

<figure><img src="../../.gitbook/assets/image (1298).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Reason for Change (nếu yêu cầu)**

**Reason for Change** là trường bắt buộc khi chỉnh sửa buổi học Offline/Live Online.
{% endstep %}

{% step %}
**Chọn lại Teacher nếu đổi Course Content**

Khi Course Content thay đổi, người dùng cần chọn lại giảng viên phụ trách buổi học.
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save**. Hệ thống cập nhật lịch lớp học, lịch giảng viên, phòng học và lịch trực lễ tân.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Hủy lịch học thủ công</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần hủy**

Người dùng chọn buổi học muốn hủy tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
**Chọn Schedule Later**

Người dùng chọn **Schedule Later** tại màn hình chi tiết buổi học.

<figure><img src="../../.gitbook/assets/image (806).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup nhập lý do hủy.

<figure><img src="../../.gitbook/assets/image (807).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập Reason**

Người dùng nhập **Reason** tại popup hủy buổi học.
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

Người dùng chọn buổi học đã hủy trên màn hình **Class Calendar**. Hệ thống hiển thị chi tiết buổi học đã hủy.
{% endstep %}

{% step %}
**Chọn Edit**

Người dùng chọn **Edit** tại màn hình chi tiết buổi học đã hủy.

<figure><img src="../../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình chỉnh sửa lịch học.
{% endstep %}

{% step %}
**Cập nhật thông tin lịch học mới**

Người dùng cập nhật thông tin lịch học mới tại màn hình **Edit Lesson** theo quy tắc chỉnh sửa lịch học thủ công.
{% endstep %}

{% step %}
**Chọn Schedule**

Người dùng chọn **Schedule** để lưu thông tin lịch học mới.

<figure><img src="../../.gitbook/assets/image (808).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị lại buổi học trên lịch học viên, lịch giảng viên, lịch phòng học và lịch trực lễ tân.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa lịch học thủ công</summary>

{% stepper %}
{% step %}
**Chọn buổi học cần xóa**

Người dùng chọn buổi học muốn xóa tại màn hình **Class Calendar**. Hệ thống hiển thị thông tin chi tiết của buổi học.
{% endstep %}

{% step %}
**Chọn Delete**

Người dùng chọn **Delete** tại màn hình chi tiết buổi học.

<figure><img src="../../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup xác nhận xóa.

<figure><img src="../../.gitbook/assets/image (812).png" alt=""><figcaption></figcaption></figure>
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

1. Xếp lịch thủ công chỉ áp dụng cho lớp có **Type = Lesson** và **Construction Mode = Offline, Blended hoặc Live Online**.
2. Lớp cần có **Status = Draft hoặc Public** để tạo/sửa/hủy/xóa lịch thủ công.
3. Có thể tạo lịch bằng nút **Add Lesson** hoặc click trực tiếp vào ngày trên Calendar; nếu click vào một ngày, trường **Lesson Date** mặc định là ngày đã chọn.
4. **Lesson Date** không được là ngày trong quá khứ.
5. Course Content chỉ hiển thị các cấu phần chưa được chọn vào buổi học khác.
6. Với Program = **CFA** hoặc **CMA**, không thể chọn Subsection/Unit từ nhiều Section khác nhau trong cùng một Lesson; các Program còn lại thì được phép.
7. Khi tick/bỏ tick cấu phần cha, tất cả cấu phần con sẽ được tick/bỏ tick theo.
8. Chỉ có thể chọn Teacher sau khi đã chọn Course Content, Lesson Date và Start Time - End Time.
9. Với buổi Live Online, trường Link Meeting chỉ hiển thị sau khi chọn phòng học.
10. Khi chỉnh sửa Course Content của buổi học, cần chọn lại Teacher.
11. Buổi học đã hủy hiển thị màu xanh dương (trên một số màn) / màu đỏ trên Class Calendar; khi xóa lịch thành công, toàn bộ cấu phần của buổi đó có thể được chọn vào buổi khác.
{% endhint %}

### Quy tắc chọn Teacher

| Quy tắc                | Mô tả                                                                                                                                                 |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| Điều kiện chọn Teacher | Chỉ được chọn sau khi đã chọn Course Content, Lesson Date và Start Time - End Time.                                                                   |
| Môn giảng dạy          | Giảng viên phải có dạy môn/nội dung tương ứng.                                                                                                        |
| Teacher Status         | Chỉ hiển thị giảng viên có trạng thái **Teaching**.                                                                                                   |
| Facility               | Giảng viên cần gắn với Facility của lớp nếu lớp có Facility. Không kiểm tra Facility nếu lớp không gắn Facility hoặc Construction Mode = Live Online. |
| Trùng lịch             | Giảng viên không được trùng lịch với buổi học.                                                                                                        |
| Weekly Norm            | Nếu số buổi dạy trong tuần vượt định mức, hệ thống hiển thị popup cảnh báo.                                                                           |
| Vượt định mức tuần     | Chọn **Yes** để vẫn tạo request đặt lịch; chọn **No** để quay lại màn Add Teacher.                                                                    |

### Quy tắc chọn Classroom

| Quy tắc              | Mô tả                                                                  |
| -------------------- | ---------------------------------------------------------------------- |
| Live Online          | Chỉ hiển thị phòng học ảo có Mode = Virtual.                           |
| Offline              | Chỉ hiển thị phòng học vật lý có Mode = Physical tại Facility của lớp. |
| Status phòng học     | Chỉ hiển thị phòng học có Status = Active.                             |
| Sức chứa phòng học   | Số lượng học viên của lớp phải ≤ sức chứa phòng.                       |
| Trùng lịch phòng học | Chỉ hiển thị phòng học không trùng với lịch buổi học.                  |
| Filter Type          | Trường Type bị disable nếu Learning Mode = Live Online.                |

### Quy tắc chỉnh sửa lịch học thủ công

| Nhóm thông tin         | Quy tắc                                                                                                                                         |
| ---------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| Điều kiện chỉnh sửa    | Buổi học phải là lịch thủ công và chưa diễn ra.                                                                                                 |
| Offline/Live Online    | Có thể chỉnh sửa Classroom, Link Meeting, Note và các trường khác theo quyền.                                                                   |
| Hybrid Class           | Chỉ được chỉnh sửa Classroom, Link Meeting và Note.                                                                                             |
| Reason for Change      | Bắt buộc với buổi học Offline/Live Online.                                                                                                      |
| Đổi Teacher            | Hệ thống cập nhật lịch lớp, xóa lịch dạy của giảng viên cũ và tạo request đặt lịch cho giảng viên mới.                                          |
| Giảng viên mới đồng ý  | Hệ thống cập nhật lịch giảng viên thay thế mới.                                                                                                 |
| Giảng viên mới từ chối | Hệ thống không cập nhật lịch giảng viên và làm trống trường Teacher.                                                                            |
| Public Class           | Nếu lớp có Status = Public, khi chỉnh sửa thành công (trừ trường View on LMS), hệ thống gửi thông báo qua LMS/email tới học viên và giảng viên. |

### Quy tắc điều chỉnh Lesson Date

| Learning Mode       | Quy tắc                                                                                    |
| ------------------- | ------------------------------------------------------------------------------------------ |
| Offline/Live Online | Có thể điều chỉnh trùng lịch Offline/Live Online được tạo thủ công.                        |
| Offline/Live Online | Không thể điều chỉnh trùng đồng thời lịch Offline/Live Online thủ công và lịch Online LMS. |
| Offline/Live Online | Không thể tiến lịch lên trước buổi học phía trước nó.                                      |
| Online LMS          | Không thể điều chỉnh trùng các lịch khác.                                                  |

### Quy tắc hủy lịch học thủ công

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

| Quy tắc                     | Mô tả                                                                                                                                                                     |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Activate                    | Người dùng chọn Activate để chọn lại lịch học bù cho buổi đã hủy.                                                                                                         |
| Sau khi Activate thành công | Buổi học hiển thị lại trên lịch học viên, giảng viên, phòng học và lịch trực lễ tân.                                                                                      |
| Email thông báo             | Gửi email thông báo lịch học bù tới học viên, giảng viên, Facility Manager và CX.                                                                                         |
| Nhắc cập nhật lịch bù       | Nếu trước ngày học Offline/Live Online tiếp theo mà chưa chọn Lesson Date mới, hệ thống gửi email nhắc cập nhật lịch học bù vào 12:00 ngày liền trước lịch học tiếp theo. |

### Quy tắc xóa lịch học thủ công

| Quy tắc         | Mô tả                                                                                                                     |
| --------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Điều kiện xóa   | Buổi học thủ công chưa diễn ra.                                                                                           |
| Xác nhận xóa    | Hệ thống hiển thị popup xác nhận trước khi xóa.                                                                           |
| Sau khi xóa     | Hệ thống xóa bản ghi lịch học khỏi Calendar.                                                                              |
| Course Content  | Toàn bộ cấu phần của buổi học đã xóa có thể được chọn vào buổi học khác.                                                  |
| Lịch liên quan  | Lịch học viên, lịch giảng viên, lịch phòng học và lịch trực lễ tân gắn với buổi học cũng bị xóa.                          |
| Email thông báo | Nếu lớp có Status = Public và Start Date của lớp ≤ hiện tại, hệ thống gửi email thông báo hủy lịch tới các bên liên quan. |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                           | Nguyên nhân                                                         | Cách xử lý                                                               |
| ------------------------------------------ | ------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Không tạo được lịch thủ công               | Lớp không thỏa điều kiện (Type/Construction Mode/Status)            | Đảm bảo lớp Type = Lesson, Construction Mode hợp lệ, Status Draft/Public |
| Không chọn được ngày học                   | Lesson Date là ngày trong quá khứ                                   | Chọn ngày học từ hôm nay trở đi                                          |
| Không chọn được Teacher                    | Chưa chọn Course Content / Lesson Date / Start-End Time             | Hoàn tất các trường này trước khi chọn Teacher                           |
| Không thấy giảng viên phù hợp              | Giảng viên không thỏa điều kiện (Teaching, Facility, trùng lịch...) | Đối chiếu quy tắc chọn Teacher; chọn giảng viên phù hợp                  |
| Cảnh báo vượt định mức tuần                | Giảng viên vượt Weekly Norm                                         | Chọn Yes để vẫn đặt lịch hoặc chọn giảng viên khác                       |
| Không nhập được Link Meeting               | Chưa chọn phòng học cho buổi Live Online                            | Chọn phòng học (Virtual) trước, sau đó nhập Link Meeting                 |
| Không lưu được khi chỉnh sửa               | Thiếu Reason for Change (Offline/Live Online)                       | Nhập Reason for Change rồi lưu                                           |
| Đổi Course Content nhưng giữ giảng viên cũ | Hệ thống yêu cầu chọn lại Teacher khi đổi Course Content            | Chọn lại Teacher sau khi đổi Course Content                              |
| Không xóa/hủy được buổi học                | Buổi học đã diễn ra hoặc lớp không đủ điều kiện                     | Chỉ thao tác với buổi chưa diễn ra và lớp đủ điều kiện                   |
