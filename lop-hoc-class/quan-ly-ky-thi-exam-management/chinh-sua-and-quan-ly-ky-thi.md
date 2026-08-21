# Chỉnh sửa & quản lý kỳ thi

## Record of changes

A - Add, M - Modify, D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 26, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Ops User, CX

**Đường dẫn:** Exam → (CFA / ACCA / CMA) Exam
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Exam Management
* **Chức năng chính:** Edit & Manage Exam
* **Module liên quan:** Class, Revision Class, Student, Course, HubSpot Ticket, HubSpot Contact
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Exam** và quyền xem danh sách kỳ thi.
* Chỉnh sửa: cần quyền chỉnh sửa kỳ thi.
* Xóa: cần quyền xóa kỳ thi.
* Quản lý học viên theo kỳ thi: cần quyền thao tác với danh sách học viên trong kỳ thi.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách kỳ thi</summary>

{% stepper %}
{% step %}
**Chọn màn hình kỳ thi theo chương trình**

Người dùng chọn màn hình kỳ thi tương ứng tại menu **Exam Management** (ví dụ: CFA Exam, ACCA Exam hoặc CMA Exam).

<figure><img src="../../.gitbook/assets/image (272).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem danh sách kỳ thi**

Người dùng xem danh sách kỳ thi tại màn hình Exam đã chọn. Hệ thống hiển thị danh sách theo chương trình học tương ứng.

Thông tin hiển thị khác nhau theo chương trình (CFA có Mở đăng ký/Hạn đăng ký sớm/chuẩn, ngày thi theo level; ACCA có ngày thi theo môn; CMA có ngày thi đầu/cuối, ngày đăng ký cuối) — đều có cột **Số học viên đăng ký**.

<figure><img src="../../.gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết kỳ thi</summary>

{% stepper %}
{% step %}
**Mở chi tiết kỳ thi**

Người dùng nhấp vào **kỳ thi tổng** tại màn hình danh sách kỳ thi. Hệ thống mở màn hình chi tiết kỳ thi.

<figure><img src="../../.gitbook/assets/image (273).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin chi tiết**

Người dùng xem thông tin chi tiết tại màn hình **Exam Detail**. Hệ thống hiển thị thông tin kỳ thi theo chương trình học tương ứng.

<figure><img src="../../.gitbook/assets/image (1289).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tìm kiếm kỳ thi</summary>

{% stepper %}
{% step %}
**Nhập/chọn điều kiện tìm kiếm**

Người dùng nhập hoặc chọn điều kiện tìm kiếm tại màn hình danh sách kỳ thi. Điều kiện tìm kiếm có thể khác nhau theo từng chương trình học.

<figure><img src="../../.gitbook/assets/image (275).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search** để áp dụng điều kiện. Hệ thống hiển thị danh sách kỳ thi thỏa mãn điều kiện đã nhập.
{% endstep %}

{% step %}
**Chọn Reset**

Người dùng chọn **Reset** nếu muốn xóa toàn bộ điều kiện. Hệ thống hiển thị lại danh sách kỳ thi theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa thông tin kỳ thi</summary>

{% stepper %}
{% step %}
**Mở màn hình chỉnh sửa kỳ thi**

Người dùng mở màn hình chỉnh sửa bằng một trong hai cách: nhấp vào **kỳ thi tổng** rồi chọn tab **Setting**, hoặc chọn **Action → Edit** tại màn hình danh sách kỳ thi.

<figure><img src="../../.gitbook/assets/image (276).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin**

Người dùng chỉnh sửa thông tin tại màn hình **Setting/Edit Exam**. Có thể thay đổi thông tin hiện có, thêm mới hoặc xóa môn học có tổ chức thi trong kỳ nếu hệ thống cho phép.

<figure><img src="../../.gitbook/assets/image (277).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Save**

Người dùng chọn **Save** tại màn hình chỉnh sửa kỳ thi. Hệ thống lưu thông tin kỳ thi đã chỉnh sửa.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa kỳ thi</summary>

{% stepper %}
{% step %}
**Chọn Action → Delete**

Người dùng chọn **Action → Delete** tại kỳ thi cần xóa trên màn hình danh sách kỳ thi. Hệ thống hiển thị popup xác nhận xóa.

<figure><img src="../../.gitbook/assets/image (278).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận xóa**

Người dùng chọn **Yes** tại popup xác nhận. Hệ thống xóa kỳ thi khỏi danh sách nếu kỳ thi thỏa mãn điều kiện xóa.

<figure><img src="../../.gitbook/assets/image (279).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem danh sách học viên theo kỳ thi</summary>

{% stepper %}
{% step %}
**Mở chi tiết kỳ thi**

Người dùng nhấp vào **kỳ thi tổng** tại màn hình danh sách kỳ thi. Hệ thống mở màn hình chi tiết kỳ thi.
{% endstep %}

{% step %}
**Chọn tab Students**

Người dùng chọn tab **Students** tại màn hình chi tiết kỳ thi. Hệ thống hiển thị danh sách học viên đã chọn kỳ thi này trên LMS.

<figure><img src="../../.gitbook/assets/image (280).png" alt=""><figcaption></figcaption></figure>

Các thông tin hiển thị: Name, Email, Phone, Class, Level, **Registered Exam Date** (kỳ thi đã được CX xác nhận thực tế hay chưa), **Defer** (học viên đã đổi lịch thi hay chưa).
{% endstep %}

{% step %}
**Tìm kiếm/lọc danh sách học viên**

Người dùng nhập hoặc chọn điều kiện tìm kiếm nếu cần. Có thể lọc theo **Search, Class code, Subject** và **Registered exam date**.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Đánh dấu kỳ thi là kỳ thi thực tế học viên đã đăng ký</summary>

{% stepper %}
{% step %}
**Cách 1 — Đánh dấu từng học viên**

Người dùng chọn **Action → Set as registered exam date** tại dòng học viên cần xác nhận trong tab **Students**, sau đó chọn **Yes** tại popup xác nhận.

<figure><img src="../../.gitbook/assets/image (281).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (282).png" alt=""><figcaption></figcaption></figure>

Hệ thống cập nhật **Registered Exam Date = Yes** cho học viên được chọn.
{% endstep %}

{% step %}
**Cách 2 — Đánh dấu nhiều học viên**

Người dùng tick chọn các học viên cần xác nhận trong tab **Students**, sau đó chọn **Set as registered exam date**.

<figure><img src="../../.gitbook/assets/image (283).png" alt=""><figcaption></figcaption></figure>

Hệ thống cập nhật **Registered Exam Date = Yes** cho các học viên được chọn.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Đổi kỳ thi cho học viên</summary>

{% stepper %}
{% step %}
**Chọn Action → Defer**

Người dùng chọn **Action → Defer** tại dòng học viên cần đổi kỳ thi trong tab **Students**. Hệ thống hiển thị popup **Reschedule Exam**.
{% endstep %}

{% step %}
**Chọn New Exam Date**

Người dùng chọn **New Exam Date** tại popup **Reschedule Exam**. Đây là trường bắt buộc, chọn một kỳ thi mới trong danh sách cho trước.
{% endstep %}

{% step %}
**Nhập Note (nếu cần)**

Người dùng nhập **Note** tại popup **Reschedule Exam** nếu cần ghi chú lý do thay đổi.
{% endstep %}

{% step %}
**Chọn OK**

Người dùng chọn **OK** tại popup **Reschedule Exam**. Hệ thống lưu thông tin đổi kỳ thi cho học viên.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần có quyền tương ứng để xem, chỉnh sửa hoặc xóa kỳ thi.
2. Mỗi chương trình học có màn hình quản lý kỳ thi riêng: **CFA Exam, ACCA Exam, CMA Exam**.
3. Khi chỉnh sửa kỳ thi, các trường được phép chỉnh sửa phụ thuộc vào việc kỳ thi đã được gắn với lớp hay chưa.
4. Được thay đổi toàn bộ thông tin kỳ thi nếu kỳ thi chưa gắn với lớp **Lesson, Foundation, Trial** và lớp **Revision** tự động chưa có học viên.
5. Nếu kỳ thi đã có ràng buộc dữ liệu, hệ thống giới hạn một số trường không được chỉnh sửa.
6. Khi kỳ thi được học viên chọn và được CX xác nhận thực tế, hệ thống cập nhật **Registered Exam Date = Yes**; sau đó học viên không thể tự thay đổi kỳ thi trên LMS.
7. Người dùng chỉ đổi kỳ thi cho học viên được khi **Registered Exam Date = Yes**.
8. Khi học viên cập nhật kỳ thi trên LMS, hệ thống tạo ticket tự động trên HubSpot và cập nhật property kỳ thi trong Contact của học viên.
{% endhint %}

### Quy tắc chỉnh sửa kỳ thi

| Trường hợp                                                                               | Quy tắc                                                            |
| ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------ |
| Kỳ thi chưa gắn với lớp Lesson/Foundation/Trial và lớp Revision tự động chưa có học viên | Được chỉnh sửa toàn bộ thông tin kỳ thi.                           |
| Kỳ thi đã có ràng buộc dữ liệu                                                           | Bị giới hạn chỉnh sửa một số thông tin.                            |
| **CFA/ACCA** đã có ràng buộc                                                             | Không được chỉnh sửa trường **Kỳ thi** và **Môn học** đã có.       |
| **CMA** đã có ràng buộc                                                                  | Không được chỉnh sửa trường **Ngày thi đầu** và **Ngày thi cuối**. |
| Thêm mới môn học có tổ chức thi                                                          | Được thực hiện nếu kỳ thi còn đáp ứng điều kiện chỉnh sửa.         |
| Xóa môn học có tổ chức thi                                                               | Được thực hiện nếu môn học chưa bị ràng buộc bởi lớp/học viên.     |

### Quy tắc xóa kỳ thi

| Trường hợp                           | Quy tắc                                                         |
| ------------------------------------ | --------------------------------------------------------------- |
| Người dùng không có quyền xóa kỳ thi | Không hiển thị hoặc không thao tác được chức năng Delete.       |
| Kỳ thi có ràng buộc với lớp/học viên | Có thể không được phép xóa tùy rule hệ thống.                   |
| Kỳ thi đủ điều kiện xóa              | Người dùng chọn **Action → Delete** và xác nhận **Yes** để xóa. |

### Quy tắc quản lý học viên theo kỳ thi

| Quy tắc                            | Mô tả                                                               |
| ---------------------------------- | ------------------------------------------------------------------- |
| **Registered Exam Date = Yes**     | Kỳ thi đã được CX xác nhận là kỳ thi thực tế học viên đã đăng ký.   |
| **Registered Exam Date = No**      | Kỳ thi chưa được CX xác nhận là kỳ thi thực tế học viên đã đăng ký. |
| Sau khi Registered Exam Date = Yes | Học viên không thể tự thay đổi kỳ thi trên LMS học viên.            |
| Đổi kỳ thi cho học viên            | Chỉ thực hiện được khi **Registered Exam Date = Yes**.              |
| **Defer = Yes**                    | Học viên đã thay đổi lịch thi sau khi đăng ký thi.                  |
| **Defer = No**                     | Học viên chưa thay đổi lịch thi sau khi đăng ký thi.                |

### Quy tắc ticket và Contact HubSpot khi học viên đổi kỳ thi

Mỗi khi học viên cập nhật thông tin kỳ thi trên LMS, hệ thống sẽ tạo ticket tự động trên HubSpot cho đội vận hành và cập nhật property kỳ thi tương ứng trong Contact của học viên.

**Thông tin ticket khi học viên thêm mới kỳ thi:**

| Thông tin          | Quy tắc                                                                            |
| ------------------ | ---------------------------------------------------------------------------------- |
| Ticket name        | `[LMS] [Họ tên] - CX kiểm tra và liên hệ tư vấn thi [Program] [Subject]`           |
| Ticket description | Học viên vừa điền thông tin kỳ thi dự kiến `[Program] [Subject]` là kỳ `[Kỳ thi]`. |

**Thông tin ticket khi học viên đổi kỳ thi:**

| Thông tin          | Quy tắc                                                         |
| ------------------ | --------------------------------------------------------------- |
| Ticket name        | `[LMS] [Họ tên] - Hỗ trợ tư vấn đổi kì thi [Program] [Subject]` |
| Ticket description | Học viên đổi từ kỳ thi `[Kỳ thi A]` sang kỳ thi `[Kỳ thi B]`.   |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                         | Nguyên nhân                                           | Cách xử lý                                                           |
| ---------------------------------------- | ----------------------------------------------------- | -------------------------------------------------------------------- |
| Một số trường kỳ thi không sửa được      | Kỳ thi đã có ràng buộc dữ liệu (gắn lớp/học viên)     | Đối chiếu quy tắc chỉnh sửa; chỉ sửa được các trường cho phép        |
| Không xóa được kỳ thi                    | Kỳ thi có ràng buộc với lớp/học viên hoặc thiếu quyền | Gỡ ràng buộc liên quan hoặc liên hệ quản trị cấp quyền xóa           |
| Không tìm thấy kỳ thi                    | Sai điều kiện tìm kiếm                                | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định           |
| Không đổi được kỳ thi cho học viên       | Học viên chưa có **Registered Exam Date = Yes**       | Đánh dấu Registered Exam Date = Yes trước khi Defer                  |
| Không lưu được Reschedule Exam           | Chưa chọn **New Exam Date** (trường bắt buộc)         | Chọn kỳ thi mới tại New Exam Date rồi bấm OK                         |
| Học viên vẫn tự đổi được kỳ thi trên LMS | Chưa xác nhận Registered Exam Date = Yes              | Xác nhận Registered Exam Date = Yes để khóa việc tự đổi của học viên |
