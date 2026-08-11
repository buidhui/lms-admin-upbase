# Tạo kỳ thi (Exam)

## Record of changes

A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 26, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Ops User, CX

**Đường dẫn:** Exam → (CFA / ACCA / CMA) Exam → Create Exam
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Exam Management
* **Chức năng chính:** Create Exam
* **Module liên quan:** Class, Revision Class, Course, Subject, Student
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Exam**.
* Tài khoản có quyền tạo mới kỳ thi.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Tạo mới một kỳ thi thủ công</summary>

{% stepper %}
{% step %}
**Chọn màn hình Exam theo chương trình**

Admin chọn màn hình Exam tương ứng tại menu **Exam** (ví dụ: **CFA Exam**, **ACCA Exam** hoặc **CMA Exam**).

<figure><img src="../../.gitbook/assets/image (1288).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Create Exam**

Admin chọn **Create Exam** tại màn hình danh sách kỳ thi. Hệ thống mở màn hình tạo mới kỳ thi.

<figure><img src="../../.gitbook/assets/image (717).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin kỳ thi theo chương trình**

Admin nhập thông tin tại màn hình **Create Exam**. Các trường có dấu **(\*)** là trường bắt buộc.

**Đối với chương trình CFA:**

<table data-search="false"><thead><tr><th>Trường thông tin</th><th>Bắt buộc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Kỳ thi</td><td>Có</td><td>Kỳ thi tổng, định dạng <strong>mm/yy</strong>.</td></tr><tr><td>Mở đăng ký</td><td>Không</td><td>Ngày mở đăng ký, định dạng <strong>dd/mm/yyyy</strong>.</td></tr><tr><td>Hạn đăng ký sớm</td><td>Không</td><td>Hạn đăng ký sớm, định dạng <strong>dd/mm/yyyy</strong>.</td></tr><tr><td>Hạn đăng ký chuẩn</td><td>Không</td><td>Hạn đăng ký chuẩn, định dạng <strong>dd/mm/yyyy</strong>.</td></tr><tr><td>Ngày thi</td><td>Có</td><td>Cài đặt ngày thi theo từng môn học/level.</td></tr><tr><td>Subject</td><td>Có</td><td>Môn học/level thuộc chương trình CFA.</td></tr><tr><td>Ngày thi theo môn</td><td>Có</td><td>Khoảng thời gian thi của môn học/level đã chọn.</td></tr><tr><td>Thêm ngày thi</td><td>-</td><td>Thêm ngày thi cho môn học/level khác.</td></tr></tbody></table>

**Đối với chương trình ACCA:**

| Trường thông tin  | Bắt buộc | Mô tả                               |
| ----------------- | -------- | ----------------------------------- |
| Kỳ thi            | Có       | Kỳ thi tổng, định dạng **mm/yy**.   |
| Ngày thi          | Có       | Cài đặt ngày thi theo từng môn học. |
| Subject           | Có       | Môn học thuộc chương trình ACCA.    |
| Ngày thi theo môn | Có       | Ngày thi của môn học đã chọn.       |
| Thêm ngày thi     | -        | Thêm ngày thi cho môn học khác.     |

**Đối với chương trình CMA:**

| Trường thông tin  | Bắt buộc | Mô tả                                                                            |
| ----------------- | -------- | -------------------------------------------------------------------------------- |
| Ngày thi          | Có       | Ngày thi đầu và ngày thi cuối của kỳ thi, định dạng **dd/mm/yyyy - dd/mm/yyyy**. |
| Ngày đăng ký cuối | Không    | Ngày đăng ký cuối của kỳ thi, định dạng **dd/mm/yyyy**.                          |
{% endstep %}

{% step %}
**Thêm ngày thi (nếu cần)**

Admin chọn **Thêm ngày thi** nếu cần thêm ngày thi cho môn học khác. Hệ thống hiển thị thêm dòng cấu hình ngày thi theo môn học.

<figure><img src="../../.gitbook/assets/image (718).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Save**

Admin chọn **Save** tại màn hình **Create Exam**. Hệ thống lưu thông tin kỳ thi và chuyển về màn hình danh sách kỳ thi.
{% endstep %}

{% step %}
**Hệ thống tự động tạo lớp Revision**

Hệ thống tự động tạo lớp **Revision** tương ứng với môn học của kỳ thi sau khi tạo kỳ thi thành công.

<figure><img src="../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo nhiều kỳ thi bằng Import Exam</summary>

{% stepper %}
{% step %}
**Chọn màn hình Exam theo chương trình**

Admin chọn màn hình Exam tương ứng tại menu **Exam** (CFA Exam, ACCA Exam hoặc CMA Exam).
{% endstep %}

{% step %}
**Chọn Import Exam**

Admin chọn **Import Exam** tại màn hình danh sách kỳ thi. Hệ thống hiển thị popup tải file import.

<figure><img src="../../.gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tải file mẫu (nếu cần)**

Admin bấm vào tên file mẫu trong popup **Import Exam**. Hệ thống tải file mẫu về thiết bị.

<figure><img src="../../.gitbook/assets/image (722).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (721).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Browse để chọn file**

Admin chọn **Browse** trong popup **Import Exam** để chọn file từ thiết bị. Hệ thống chỉ chấp nhận file định dạng **.csv** hoặc **.xlsx** và mỗi lần chỉ chọn **01 file**.

<figure><img src="../../.gitbook/assets/image (723).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Import**

Admin chọn **Import** sau khi đã chọn file hợp lệ. Hệ thống tải file lên và xử lý dữ liệu kỳ thi trong file.
{% endstep %}

{% step %}
**Xem kết quả import**

Hệ thống hiển thị hộp thoại kết quả import: **Source, Data, Successfully, Error**.
{% endstep %}

{% step %}
**Xem chi tiết lỗi (nếu cần)**

Admin chọn **View Log** tại hộp thoại kết quả import. Hệ thống mở màn hình log chi tiết; các trường không hợp lệ được bôi đỏ và lý do lỗi hiển thị tại cột **Errors**.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Kỳ thi được tạo theo từng chương trình học: **CFA, ACCA, CMA**.
2. Các trường có dấu **(\*)** là trường bắt buộc.
3. Không thể tạo 2 kỳ thi có cùng thông tin tại trường **Kỳ thi**.
4. Với CFA và ACCA, trường **Kỳ thi** là kỳ thi tổng và cần nhập đúng định dạng **mm/yy** khi tạo thủ công; cần cấu hình ngày thi theo từng môn học/level.
5. Với CMA, cần nhập ngày thi đầu và ngày thi cuối của kỳ thi.
6. Sau khi tạo kỳ thi thành công, hệ thống tự động tạo lớp **Revision** tương ứng với môn học của kỳ thi.
{% endhint %}

### Quy tắc dữ liệu import theo chương trình

{% tabs %}
{% tab title="CFA" %}
| Trường trong file                                  | Bắt buộc     | Định dạng / Quy tắc                                                                          |
| -------------------------------------------------- | ------------ | -------------------------------------------------------------------------------------------- |
| Season / Kỳ thi                                    | Có           | Định dạng **mm-yyyy**.                                                                       |
| Registration opening date / Mở đăng ký             | Không        | Định dạng **yyyy-mm-dd**.                                                                    |
| Early registration deadline / Hạn đăng ký sớm      | Không        | Định dạng **yyyy-mm-dd**.                                                                    |
| Standard registration deadline / Hạn đăng ký chuẩn | Không        | Định dạng **yyyy-mm-dd**.                                                                    |
| Ngày thi theo từng môn/level                       | Có điều kiện | Không được để trống đồng thời cả 3 cột level 1, 2, 3; định dạng **yyyy-mm-dd - yyyy-mm-dd**. |
{% endtab %}

{% tab title="ACCA" %}
| Trường trong file      | Bắt buộc | Định dạng / Quy tắc                   |
| ---------------------- | -------- | ------------------------------------- |
| Season / Kỳ thi        | Có       | Định dạng **mm-yyyy**.                |
| Subject code / Môn học | Có       | Chọn một trong các giá trị cho trước. |
| Exam date / Ngày thi   | Có       | Định dạng **yyyy-mm-dd**.             |
{% endtab %}

{% tab title="CMA" %}
| Trường trong file                             | Bắt buộc | Định dạng / Quy tắc                  |
| --------------------------------------------- | -------- | ------------------------------------ |
| Season / Kỳ thi                               | Không    | Nhập dạng text nếu template yêu cầu. |
| First exam date / Ngày thi đầu                | Có       | Định dạng **yyyy-mm-dd**.            |
| Final exam date / Ngày thi cuối               | Có       | Định dạng **yyyy-mm-dd**.            |
| Registration closing date / Ngày đăng ký cuối | Có       | Định dạng **yyyy-mm-dd**.            |
{% endtab %}
{% endtabs %}

### Quy tắc tự động tạo lớp Revision

Sau khi tạo kỳ thi thành công, hệ thống tự động tạo lớp **Revision** tương ứng với môn học của từng kỳ thi.

<table data-search="false"><thead><tr><th>Thông tin</th><th>Quy tắc</th></tr></thead><tbody><tr><td>Name</td><td><code>[Tên Subject] Revision - [Kỳ thi mm/yyyy]</code></td></tr><tr><td>Code</td><td><code>R-[Mã Subject]-[Kỳ thi]</code></td></tr><tr><td>Construction Mode</td><td>Online</td></tr><tr><td>Số học viên tối đa</td><td>10000</td></tr><tr><td>Duration</td><td>Fixed</td></tr><tr><td>Course</td><td>Để trống</td></tr><tr><td>Exam</td><td>Gắn với kỳ thi vừa tạo</td></tr></tbody></table>

**Quy tắc Start Date / End Date của lớp Revision:**

| Program | Start Date                                     | End Date                            |
| ------- | ---------------------------------------------- | ----------------------------------- |
| CFA     | 120 ngày trước ngày thi đầu tiên của kỳ thi    | Ngày cuối tháng của tháng có kỳ thi |
| ACCA    | Trước 3 tháng so với ngày thi                  | Ngày thi                            |
| CMA     | Trước 3 tháng so với ngày đầu tiên của đợt thi | Ngày cuối cùng của đợt thi          |

Khi chọn Course để thêm vào lớp Revision, hệ thống chỉ hiển thị các khóa **Revision/Practice Course** có **Program** và **Subject** trùng với kỳ thi.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                     | Nguyên nhân                                                                 | Cách xử lý                                                            |
| ------------------------------------ | --------------------------------------------------------------------------- | --------------------------------------------------------------------- |
| Không lưu được kỳ thi                | Chưa nhập đủ các trường bắt buộc (\*)                                       | Nhập đầy đủ các trường bắt buộc rồi bấm Save                          |
| Báo lỗi kỳ thi bị trùng              | Đã tồn tại kỳ thi có cùng thông tin trường **Kỳ thi**                       | Nhập thông tin kỳ thi khác, không trùng                               |
| Sai định dạng trường Kỳ thi/Ngày thi | Nhập sai định dạng (mm/yy, dd/mm/yyyy...)                                   | Nhập đúng định dạng theo từng chương trình                            |
| Import kỳ thi thất bại               | File sai định dạng (.csv/.xlsx), chọn nhiều file, hoặc dữ liệu sai template | Dùng đúng file mẫu, chọn 01 file; xem View Log sửa lỗi rồi import lại |
| CFA: lỗi cột ngày thi theo level     | Để trống đồng thời cả 3 cột level 1, 2, 3                                   | Điền ngày thi cho ít nhất 1 level theo định dạng yêu cầu              |
| Không thấy Course cho lớp Revision   | Course không cùng Program/Subject với kỳ thi                                | Chỉ Revision/Practice Course trùng Program và Subject mới hiển thị    |
