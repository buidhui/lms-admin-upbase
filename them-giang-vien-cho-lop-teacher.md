# them giang vien cho lop teacher

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 25, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Ops User, CX/Admin lớp

**Đường dẫn:** LMS → Class List → Chọn lớp học → Teachers
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Teacher
* **Module liên quan:** Class List, Class Detail, Course Content, Section, Learning Schedule, Teacher Calendar, LMS Teacher Request
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class** và quyền xem chi tiết lớp học.
* Tài khoản có quyền thêm/chỉnh sửa giảng viên trong lớp.
* Lớp học đã được tạo, khóa học đã được gắn vào lớp và Course đã có cấu trúc **Section**.
* Lớp cần có lịch học tự động trước khi chọn giảng viên; nếu chưa có, hệ thống báo lỗi **"Please add learning schedule before choosing teacher"**.
* Giảng viên cần thêm phải thỏa mãn điều kiện hiển thị trong danh sách giảng viên của hệ thống.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách giảng viên của lớp</summary>

{% stepper %}
{% step %}
## Mở màn hình Class Detail

Người dùng nhấp vào **tên lớp học** tại màn hình **Class List**. Hệ thống mở màn hình **Class Detail**.
{% endstep %}

{% step %}
## Chọn tab Teachers

Người dùng chọn tab **Teachers** tại màn hình **Class Detail**. Hệ thống hiển thị danh sách giảng viên của lớp.

<figure><img src="https://sapp-academy.gitbook.io/files/HTpBhViG29S2TbMh2JAQ" alt=""><figcaption></figcaption></figure>

Danh sách giảng viên hiển thị theo thứ tự thời gian gắn (sớm nhất → muộn nhất):

| Cột thông tin        | Mô tả                                 |
| -------------------- | ------------------------------------- |
| **Name**             | Tên giảng viên.                       |
| **Phone**            | Số điện thoại của giảng viên.         |
| **Email**            | Email của giảng viên.                 |
| **Teaching Section** | Section đang được gắn với giảng viên. |
{% endstep %}

{% step %}
## Tìm kiếm giảng viên

Người dùng nhập thông tin vào ô **Search teacher** nếu cần tìm kiếm theo Name, Phone hoặc Email, sau đó chọn **Search** để hiển thị danh sách theo điều kiện tìm kiếm.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Gắn giảng viên cho Section</summary>

{% stepper %}
{% step %}
## Mở tab Teachers

Người dùng mở tab **Teachers** trong màn hình **Class Detail**.
{% endstep %}

{% step %}
## Chọn Add/Edit Teacher

Người dùng chọn **Add/Edit Teacher** tại tab **Teachers**. Hệ thống mở màn hình **Add/Edit Teacher** và hiển thị danh sách Section của Course.

<figure><img src="https://sapp-academy.gitbook.io/files/RUP9FIRVetnqtVvv2THT" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Chọn Add Teacher tại Section chưa có giảng viên

Người dùng chọn **Add Teacher** tại Section chưa có giảng viên. Hệ thống chuyển đến màn hình chọn giảng viên.

<figure><img src="https://sapp-academy.gitbook.io/files/0uH82SIJq68qHWtcubc7" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Tìm kiếm/lọc giảng viên

Người dùng tìm kiếm hoặc lọc giảng viên (Search, Belong To, Priority, From/To Date) tại màn hình chọn giảng viên nếu cần.

<figure><img src="https://sapp-academy.gitbook.io/files/ntKslDkOSLYCeyf3sBw9" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Chọn giảng viên

Người dùng tick/radio chọn giảng viên muốn gắn cho Section.
{% endstep %}

{% step %}
## Chọn Add

Người dùng chọn **Add** tại màn hình chọn giảng viên. Hệ thống quay lại màn hình **Add/Edit Teacher** và hiển thị giảng viên đã chọn tại Section tương ứng.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Add/Edit Teacher**. Hệ thống lưu thông tin và gửi request/email đặt lịch tới giảng viên nếu Section có buổi học phù hợp.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thay đổi giảng viên của Section</summary>

{% stepper %}
{% step %}
## Mở tab Teachers

Người dùng mở tab **Teachers** trong màn hình **Class Detail**.
{% endstep %}

{% step %}
## Chọn Add/Edit Teacher

Người dùng chọn **Add/Edit Teacher** tại tab **Teachers**.

<figure><img src="https://sapp-academy.gitbook.io/files/FZ9ljl161QVCSGAFMlVJ" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Chọn Change Teacher

Người dùng chọn **Change Teacher** tại Section cần thay đổi giảng viên. Hệ thống chuyển đến màn hình chọn giảng viên.

<figure><img src="https://sapp-academy.gitbook.io/files/oeKvT8SiIxx69ZoaCrGj" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Chọn giảng viên mới và Add

Người dùng chọn giảng viên mới tại màn hình chọn giảng viên, sau đó chọn **Add** để gắn giảng viên mới cho Section.
{% endstep %}

{% step %}
## Nhập lý do thay đổi (nếu request Approved)

Người dùng nhập lý do thay đổi giảng viên nếu request hiện tại có trạng thái **Approved**.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Add/Edit Teacher**. Hệ thống gửi request đặt lịch tới giảng viên mới để giảng viên duyệt đề xuất.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem lịch sử giảng viên gắn với Section</summary>

{% stepper %}
{% step %}
## Mở tab Teachers

Người dùng mở tab **Teachers** trong màn hình **Class Detail**.
{% endstep %}

{% step %}
## Chọn Add/Edit Teacher

Người dùng chọn **Add/Edit Teacher** tại tab **Teachers**.
{% endstep %}

{% step %}
## Chọn Action → History

Người dùng chọn **Action → History** tại Section đã từng gắn giảng viên. Hệ thống hiển thị màn hình **History**.

<figure><img src="https://sapp-academy.gitbook.io/files/GoF0CyfnRkxLQsmG3VMX" alt=""><figcaption></figcaption></figure>

<figure><img src="https://sapp-academy.gitbook.io/files/5CwvikqhaZAGLhE9JRT5" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
## Chọn Back

Người dùng chọn **Back** tại màn hình **History** để quay lại màn hình **Add/Edit Teacher**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa giảng viên khỏi Section</summary>

{% stepper %}
{% step %}
## Mở tab Teachers

Người dùng mở tab **Teachers** trong màn hình **Class Detail**.
{% endstep %}

{% step %}
## Chọn Add/Edit Teacher

Người dùng chọn **Add/Edit Teacher** tại tab **Teachers**.
{% endstep %}

{% step %}
## Chọn Action → Delete

<figure><img src="https://sapp-academy.gitbook.io/files/6rikJyAvfUZTwXN3XdAF" alt=""><figcaption></figcaption></figure>

Người dùng chọn **Action → Delete** tại Section cần xóa giảng viên. Chỉ có thể xóa giảng viên khi request đặt lịch dạy của giảng viên có trạng thái **Pending**.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Add/Edit Teacher**. Hệ thống xóa giảng viên khỏi Section, đồng thời xóa request đặt lịch của giảng viên cũ.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Với program khác ACCA, Cert/Dip:** giảng viên được gắn theo từng **Section**, không gắn chung cho toàn bộ lớp. **Với program = ACCA/Cert/Dip:** giảng viên được gắn chung cho toàn bộ lớp.
2. Lớp cần có lịch học tự động trước khi chọn giảng viên; nếu chưa có, hệ thống báo lỗi **"Please add learning schedule before choosing teacher"**.
3. Được phép chỉnh sửa giảng viên khi request có trạng thái **Pending, Approved, Rejected** hoặc **Cancelled**.
4. Chỉ có thể xóa giảng viên khi request đặt lịch dạy có trạng thái **Pending**.
5. Khi thay đổi giảng viên với request có trạng thái **Approved**, cần nhập lý do thay đổi.
6. Khi xóa giảng viên thành công, Section gắn với giảng viên đó sẽ trống trường **Responsibility** và request đặt lịch của giảng viên cũ bị xóa (không hiển thị ở phía giảng viên cũ).
7. Với Section có tất cả buổi học đều là **Online LMS**, hệ thống vẫn cho phép gắn giảng viên nhưng không gửi email, không gửi request và không có status.
8. Khi gắn giảng viên vào Section, hệ thống gửi request đặt lịch cho tất cả các buổi trong Section có Learning Mode là **Offline** hoặc **Live Online**.
9. Với request đặt lịch có trạng thái **Approved**, hệ thống cập nhật giảng viên tại các buổi có lịch tự động được gắn với Section và cập nhật lịch tại Calendar của giảng viên. Hệ thống không cập nhật giảng viên cho các buổi lịch thủ công.
{% endhint %}

### Điều kiện hiển thị giảng viên tại màn chọn Teacher

Màn hình chọn giảng viên chỉ hiển thị các giảng viên thỏa mãn đồng thời các điều kiện sau:

| Điều kiện           | Quy tắc                                                                                        |
| ------------------- | ---------------------------------------------------------------------------------------------- |
| **Teaching Status** | Giảng viên có Teaching Status = Đang dạy.                                                      |
| **Facility**        | Giảng viên có gắn với cơ sở diễn ra buổi học.                                                  |
| **Belong To**       | Giảng viên có thông tin Section giảng dạy trùng với Belong To của cấu phần học.                |
| **Lịch cá nhân**    | Giảng viên có lịch cá nhân trùng lịch học của Section tối đa 3 buổi.                           |
| **Định mức tuần**   | Số buổi định mức tuần của giảng viên không vượt quá số buổi tối đa khi nhận thêm lịch dạy này. |

### Quy tắc xử lý trùng lịch giảng viên

| Trường hợp                             | Quy tắc                                                                           |
| -------------------------------------- | --------------------------------------------------------------------------------- |
| Lịch giảng viên trùng nhiều hơn 3 buổi | Giảng viên không hiển thị tại màn Add Teacher.                                    |
| Lịch giảng viên trùng từ 1 đến 3 buổi  | Hệ thống vẫn cho phép chọn nhưng hiển thị popup cảnh báo danh sách buổi bị trùng. |
| Lịch giảng viên không trùng            | Giảng viên hiển thị và có thể được chọn bình thường.                              |

Nội dung popup cảnh báo có dạng: _"The class schedule overlaps with lecturer's existing schedule on the following sessions: \[tên buổi 1], \[tên buổi 2], …"_

### Quy tắc request đặt lịch giảng viên

| Trạng thái request | Ý nghĩa / Quy tắc                                                                                 |
| ------------------ | ------------------------------------------------------------------------------------------------- |
| **Pending**        | Request đang chờ giảng viên duyệt. Người dùng có thể xóa giảng viên nếu request ở trạng thái này. |
| **Approved**       | Giảng viên đã duyệt request. Nếu đổi giảng viên, người dùng cần nhập lý do thay đổi.              |
| **Rejected**       | Giảng viên đã từ chối request. Hệ thống hiển thị Reason.                                          |
| **Cancelled**      | Request đã bị hủy. Hệ thống hiển thị Reason.                                                      |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                               | Nguyên nhân                                                                                                        | Cách xử lý                                                  |
| -------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------- |
| Báo lỗi "Please add learning schedule before choosing teacher" | Lớp chưa có lịch học tự động                                                                                       | Tạo lịch học tự động cho lớp trước khi chọn giảng viên      |
| Không thấy giảng viên cần gắn tại màn chọn                     | Giảng viên không thỏa điều kiện hiển thị (Teaching Status, Facility, Belong To, trùng lịch >3 buổi, định mức tuần) | Đối chiếu điều kiện hiển thị; chọn giảng viên phù hợp       |
| Popup cảnh báo trùng lịch giảng viên                           | Lịch giảng viên trùng từ 1–3 buổi với lịch Section                                                                 | Xem danh sách buổi trùng, cân nhắc trước khi xác nhận chọn  |
| Không xóa được giảng viên khỏi Section                         | Request đặt lịch không ở trạng thái **Pending**                                                                    | Chỉ xóa được khi request ở trạng thái Pending               |
| Đổi giảng viên không lưu được                                  | Request Approved nhưng chưa nhập lý do thay đổi                                                                    | Nhập lý do thay đổi khi đổi giảng viên với request Approved |
| Section Online LMS không có status/email                       | Toàn bộ buổi là Online LMS nên không gửi request/email                                                             | Đây là quy tắc hệ thống, không phải lỗi                     |
