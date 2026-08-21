# Event Test

## Record of Changes

| Ngày có hiệu lực | Người cập nhật    | Loại thay đổi (A/M/D) | Mô tả thay đổi                                                    | Phiên bản |
| ---------------- | ----------------- | --------------------- | ----------------------------------------------------------------- | --------- |
| 23/06/2026       | it-ba@sapp.edu.vn | A                     | Viết lại theo template chuẩn Gitbook từ UG cũ (Confluence v1.7.0) | v2.0.0    |

***

## I. Thông tin chung

**Dành cho:** Ops Admin, CX\
**Đường dẫn:** Menu bên trái → Assessment Management → Test Management -> Entrance Test / Entrance Test Participants

### Phạm vi & Module liên quan

Tài liệu hướng dẫn đội Ops Admin và CX thực hiện toàn bộ nghiệp vụ quản lý bài kiểm tra theo sự kiện (Event Test): tạo mới, xem danh sách, chỉnh sửa bài kiểm tra; tra cứu và quản lý học viên tham gia; xem chi tiết kết quả bài làm.

**Module liên quan:**

* Question Bank (nguồn câu hỏi cho bài kiểm tra)
* LMS Pro (nơi học viên thấy và làm bài kiểm tra)

### Điều kiện tiên quyết

* Đã đăng nhập thành công vào hệ thống Ops
* Tài khoản được cấp quyền **Event Test** (xem/tạo/chỉnh sửa/quản lý học viên)

***

## II. Chi tiết hướng dẫn

### Event Test List — Quản lý danh sách bài kiểm tra

#### Xem danh sách & chi tiết bài kiểm tra

**Kết quả:** Tìm được bài kiểm tra cần tra cứu và xem đầy đủ thông tin, danh sách câu hỏi.

{% stepper %}
{% step %}
## Tại menu bên trái, chọn **Event Test** → **Event Test List**
{% endstep %}

{% step %}
## Danh sách hiển thị các cột

| Cột                                  | Mô tả                                                  |
| ------------------------------------ | ------------------------------------------------------ |
| Test Name                            | Tên bài kiểm tra                                       |
| Program / Event                      | Chương trình học và sự kiện tương ứng                  |
| Event Duration                       | Thời gian diễn ra sự kiện                              |
| Test Duration (Start At – Finish At) | Thời gian học viên được truy cập bài kiểm tra          |
| Participants                         | Số học viên đã tham gia                                |
| Status                               | Trạng thái bài kiểm tra (xem bảng trạng thái bên dưới) |

**Bảng trạng thái bài kiểm tra:**

| Trạng thái   | Ý nghĩa                | Hiển thị trên LMS                              |
| ------------ | ---------------------- | ---------------------------------------------- |
| **Draft**    | Sự kiện chưa diễn ra   | Ẩn với học viên                                |
| **Active**   | Sự kiện đang diễn ra   | Hiển thị với học viên                          |
| **Locked**   | Đã có học viên làm bài | Hiển thị với học viên                          |
| **Inactive** | Sự kiện đã kết thúc    | Ẩn với HV chưa làm; vẫn hiện với HV đã làm bài |
{% endstep %}

{% step %}
## (Tuỳ chọn) Dùng bộ lọc để thu hẹp kết quả

| Bộ lọc    | Mô tả                          |
| --------- | ------------------------------ |
| Test Name | Tìm kiếm theo tên bài kiểm tra |
| Program   | Lọc theo chương trình học      |
| Event     | Lọc theo sự kiện               |
| Sort by   | Sắp xếp kết quả                |
| Status    | Lọc theo trạng thái            |

Click **Search** để lọc · Click **Reset** để xóa bộ lọc.
{% endstep %}

{% step %}
## Click vào **tên bài kiểm tra** để xem chi tiết với 2 tab

| Tab           | Nội dung                                                         |
| ------------- | ---------------------------------------------------------------- |
| **Test Info** | Thông tin chung: Test Name, Program, Event, Start At – Finish At |
| **Tab 2**     | Danh sách câu hỏi của bài kiểm tra                               |

Danh sách bài kiểm tra và thông tin chi tiết hiển thị thành công → Xem hoàn tất.
{% endstep %}
{% endstepper %}

#### Tạo mới bài kiểm tra

**Kết quả:** Bài kiểm tra được tạo thành công và xuất hiện trong Event Test List.

{% hint style="warning" %}
**Trước khi bắt đầu:** Mỗi sự kiện (Event) của một chương trình học chỉ được tạo **1 bài kiểm tra duy nhất** — kiểm tra danh sách trước khi tạo mới.
{% endhint %}

{% stepper %}
{% step %}
## Bước 1 — Mở form tạo mới

Tại màn hình **Event Test List**, click nút **+ Create Event Test** ở góc trên bên phải (hoặc chọn **Create Event Test** từ menu bên trái).
{% endstep %}

{% step %}
## Bước 2 — Điền thông tin chung (tab Test Info)

Điền các trường có dấu (\*) là bắt buộc:

| Trường               | Bắt buộc | Mô tả                                         |
| -------------------- | -------- | --------------------------------------------- |
| Test Name            | Có (\*)  | Tên bài kiểm tra                              |
| Program              | Có (\*)  | Chương trình học — chọn từ danh sách          |
| Event                | Có (\*)  | Sự kiện — tự động lọc theo Program đã chọn    |
| Start At – Finish At | Có (\*)  | Thời gian học viên được truy cập bài kiểm tra |
{% endstep %}

{% step %}
## Bước 3 — Cài đặt câu hỏi

Sau khi lưu tab Test Info, hệ thống chuyển sang màn hình cài đặt câu hỏi. Điền các trường:

| Trường            | Bắt buộc          | Mô tả                                                |
| ----------------- | ----------------- | ---------------------------------------------------- |
| Type of Test      | Có (\*)           | Loại bài kiểm tra — chọn 1 trong 3 giá trị           |
| Test Mode         | Có (\*)           | **Tutor** (không tính giờ) / **Timed** (có tính giờ) |
| Duration          | Có (\*) nếu Timed | Thời gian làm bài (chỉ hiển thị khi chọn Timed)      |
| Danh sách câu hỏi | Có (\*)           | Thêm câu hỏi cho bài kiểm tra                        |
{% endstep %}

{% step %}
## Bước 4

Click **Save** để lưu.

Hệ thống chuyển về **Event Test List** và bài kiểm tra mới xuất hiện đầu danh sách → Tạo thành công.
{% endstep %}
{% endstepper %}

#### Chỉnh sửa bài kiểm tra

**Kết quả:** Thông tin bài kiểm tra được cập nhật thành công.

{% stepper %}
{% step %}
## Tại màn hình **Event Test List**, click vào **tên bài kiểm tra** muốn chỉnh sửa
{% endstep %}

{% step %}
## Chỉnh sửa thông tin tại tab **Test Info** hoặc tab câu hỏi

Lưu ý giới hạn chỉnh sửa theo trạng thái:

| Trạng thái bài kiểm tra                 | Trường được phép chỉnh sửa                            |
| --------------------------------------- | ----------------------------------------------------- |
| Chưa có học viên đăng ký                | Tất cả các trường                                     |
| Đã có ít nhất 1 học viên đăng ký        | Tất cả trừ **Program** và **Event**                   |
| Đã có ít nhất 1 học viên hoàn thành bài | Chỉ **Test Name** — không sửa được các trường còn lại |
{% endstep %}

{% step %}
## Click **Save** để lưu thay đổi

Hệ thống lưu thành công → Thông tin bài kiểm tra được cập nhật → Chỉnh sửa hoàn tất.
{% endstep %}
{% endstepper %}

***

### Participants — Quản lý học viên tham gia

#### Xem danh sách học viên theo bài kiểm tra

**Kết quả:** Tra cứu được danh sách học viên tham gia một bài kiểm tra cụ thể, kèm điểm số và trạng thái nộp bài.

Truy cập bằng 1 trong 2 cách:

* **Cách 1:** Tại **Event Test List**, click vào giá trị trường **Participants** của bài kiểm tra.
* **Cách 2:** Tại **Event Test List**, click nút **⋮ (Action)** → chọn **Participant List**.

Các cột hiển thị trong danh sách:

| Cột                   | Mô tả                                                             |
| --------------------- | ----------------------------------------------------------------- |
| Name                  | Tên học viên                                                      |
| Multiple Choice Score | Điểm trắc nghiệm = Điểm đúng / Tổng điểm câu hỏi MCQ              |
| Test Time             | Thời gian làm bài thực tế                                         |
| Submission Time       | Thời gian nộp bài                                                 |
| Source                | **Manual** (thêm thủ công) / **Form register** (đăng ký qua form) |

Tìm kiếm học viên theo: Tên/Email/Số điện thoại, Source, Result (sắp xếp điểm Descending/Ascending). Click **Search** · **Reset** để xóa.

Danh sách học viên của bài kiểm tra hiển thị thành công → Xem hoàn tất.

#### Xem tất cả học viên (All Participants)

**Kết quả:** Tra cứu được toàn bộ học viên đã tham gia mọi bài kiểm tra trong một màn hình tổng hợp.

{% stepper %}
{% step %}
## Tại menu bên trái, chọn **Event Test** → **All Participants**
{% endstep %}

{% step %}
## Các cột hiển thị

| Cột             | Mô tả                                 |
| --------------- | ------------------------------------- |
| Name            | Tên học viên                          |
| Event Test      | Tên bài kiểm tra                      |
| Result          | Số câu đúng / Tổng số câu trắc nghiệm |
| Source          | Manual / Form register                |
| Submission Time | Thời gian nộp bài                     |
{% endstep %}

{% step %}
## (Tuỳ chọn) Tìm kiếm theo

Tìm kiếm theo: Tên/Email/Số điện thoại, Program, Event, Sort by. Click **Search** · **Reset** để xóa.

Danh sách tổng hợp tất cả học viên hiển thị thành công → Xem hoàn tất.
{% endstep %}
{% endstepper %}

#### Xem chi tiết kết quả/bài làm học viên

**Kết quả:** Xem được kết quả từng câu hỏi và đáp án chi tiết của học viên; có thể export kết quả toàn bài.

{% stepper %}
{% step %}
## Tại màn hình **Participant List** của bài kiểm tra, click vào **điểm số** của học viên tại cột **Multiple Choice Score**
{% endstep %}

{% step %}
## Màn hình kết quả hiển thị từng câu hỏi

| Cột      | Mô tả                                                               |
| -------- | ------------------------------------------------------------------- |
| Question | Nội dung câu hỏi                                                    |
| Type     | Loại câu hỏi (trắc nghiệm / tự luận)                                |
| Result   | **Correct/Incorrect** (MCQ) · **Completed/Not Completed** (tự luận) |
{% endstep %}

{% step %}
## (Tuỳ chọn) Lọc câu hỏi theo Question Type hoặc Result
{% endstep %}

{% step %}
## Click vào **câu hỏi** để xem đáp án đúng và câu trả lời của học viên
{% endstep %}

{% step %}
## Để tải kết quả toàn bộ học viên, click **Export Result**

Kết quả chi tiết từng câu hỏi của học viên hiển thị thành công → Xem hoàn tất.
{% endstep %}
{% endstepper %}

#### Thêm học viên thủ công

**Kết quả:** Học viên được thêm vào bài kiểm tra với Source = Manual và xuất hiện trong Participant List.

Truy cập màn hình thêm học viên bằng 1 trong 2 cách:

* **Cách 1:** Tại **Event Test List**, click nút **⋮ (Action)** trên dòng bài kiểm tra → chọn **Add Participants**.
* **Cách 2:** Tại màn hình **Participant List** của bài kiểm tra, click nút **Add Participants**.

{% stepper %}
{% step %}
## Tại màn hình **Add Participant**, tìm kiếm và chọn học viên cần thêm
{% endstep %}

{% step %}
## Click **Add** để xác nhận

Hệ thống quay về **Participant List** và học viên vừa thêm xuất hiện trong danh sách (Source = Manual) → Thêm thành công.
{% endstep %}
{% endstepper %}

#### Xóa học viên thủ công

**Kết quả:** Học viên được xóa khỏi bài kiểm tra.

{% hint style="warning" %}
**Chỉ xóa được học viên khi đáp ứng ít nhất 1 trong các điều kiện:**

* Học viên được thêm thủ công (Source = **Manual**) **và** chưa làm bài kiểm tra.
* Học viên đã làm bài nhưng là **Test Account** (tài khoản nghiệm thu nội bộ SAPP).

Không thể xóa học viên đăng ký qua Form register, hoặc học viên thực đã nộp bài.
{% endhint %}

{% stepper %}
{% step %}
## Tại màn hình **Participant List** của bài kiểm tra, click nút **⋮ (Action)** trên dòng học viên cần xóa → chọn **Delete**
{% endstep %}

{% step %}
## Xác nhận trong hộp thoại

Học viên biến mất khỏi danh sách → Xóa thành công.
{% endstep %}
{% endstepper %}

***

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
**Lưu ý quan trọng:**

1. **Một sự kiện – một bài kiểm tra:** Mỗi Event của cùng một Program chỉ được tạo 1 bài kiểm tra duy nhất. Kiểm tra Exam List trước khi tạo mới để tránh lỗi trùng lặp.
2. **Khóa trường sau khi có học viên:** Sau khi bài kiểm tra có ít nhất 1 học viên đăng ký, không thể thay đổi **Program** và **Event**. Sau khi có học viên hoàn thành bài, chỉ còn được đổi **Test Name**.
3. **Điều kiện xóa học viên:** Chỉ xóa được học viên thêm thủ công (Manual) chưa làm bài, hoặc Test Account đã làm bài. Học viên từ Form register không xóa được.
4. **Trạng thái ảnh hưởng đến LMS:** Draft = ẩn hoàn toàn; Active = hiển thị; Inactive = ẩn với HV chưa làm, vẫn hiện với HV đã làm bài — đội Ops cần theo dõi trạng thái để hỗ trợ học viên đúng lúc.
{% endhint %}

**Mẹo sử dụng:**

1. Dùng bộ lọc **Status = Draft** để kiểm tra các bài kiểm tra sắp được kích hoạt trước khi sự kiện diễn ra.
2. Khi cần kiểm tra kết quả nhiều học viên cùng lúc, dùng **Export Result** thay vì xem từng người — tiết kiệm thời gian tra cứu.
3. Sau khi thêm học viên thủ công, kiểm tra lại cột **Source = Manual** để xác nhận đúng nguồn đăng ký trước khi báo cáo số liệu.

***

## IV. Lỗi thường gặp

| Lỗi / Tình huống                                       | Nguyên nhân                                                                 | Hướng dẫn xử lý                                                                            |
| ------------------------------------------------------ | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Không tạo được bài kiểm tra – báo trùng Event          | Đã tồn tại bài kiểm tra cho cùng Program + Event này                        | Kiểm tra Event Test List → chỉnh sửa bài kiểm tra hiện có thay vì tạo mới                  |
| Trường Program / Event bị khóa khi chỉnh sửa           | Bài kiểm tra đã có học viên đăng ký                                         | Không thể thay đổi Program/Event sau khi có HV; cần tạo bài mới nếu sai thông tin          |
| Không sửa được thông tin nào ngoài Test Name           | Đã có học viên hoàn thành bài kiểm tra                                      | Trạng thái này chỉ cho phép đổi tên; liên hệ Tech nếu cần can thiệp sâu hơn                |
| Không xóa được học viên – nút Delete bị ẩn / vô hiệu   | HV đăng ký qua Form register, hoặc HV đã làm bài và không phải Test Account | Kiểm tra cột Source và trạng thái bài làm; chỉ Test Account mới xóa được sau khi làm bài   |
| Không thấy học viên cần thêm trong màn Add Participant | HV chưa có tài khoản trong hệ thống, hoặc tìm kiếm sai tên/email            | Kiểm tra lại thông tin HV; nếu chưa có tài khoản cần tạo trước ở module quản lý người dùng |
| Không tìm thấy bài kiểm tra trong danh sách            | Sai bộ lọc hoặc bài kiểm tra chưa được tạo                                  | Click **Reset** để xóa bộ lọc → kiểm tra lại; tạo mới nếu chưa có                          |

{% hint style="info" %}
📩 Chưa tự xử lý được? Liên hệ **Hotline 1900 2225** hoặc tạo ticket tại https://sapp.edu.vn/dich-vu-cham-soc-hoc-vien-sapp-academy/.
{% endhint %}
