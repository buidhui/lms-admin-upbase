# Entrance test

## Record of Changes

| Ngày có hiệu lực | Người cập nhật    | Loại thay đổi (A/M/D) | Mô tả thay đổi                                       | Phiên bản |
| ---------------- | ----------------- | --------------------- | ---------------------------------------------------- | --------- |
| 29/06/2026       | it-ba@sapp.edu.vn | A                     | Khởi tạo tài liệu theo template mới từ Confluence UG | v2.0.0    |

***

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Ops Admin, CX\
**Đường dẫn:** `Menu → Entrance Test`
{% endhint %}

### Phạm vi & Module liên quan

Tài liệu hướng dẫn Ops Admin và CX quản lý bài kiểm tra đầu vào trên hệ thống Ops, bao gồm: tạo và chỉnh sửa bài kiểm tra đầu vào, quản lý danh sách học viên tham gia theo từng bài kiểm tra, và xem tổng hợp toàn bộ học viên đã làm bài trên tất cả các chương trình.

**Module liên quan:**

* Entrance Test → Entrance Test List (quản lý bài kiểm tra)
* Entrance Test → Participants (toàn bộ học viên)
* Tab Participants trong từng bài kiểm tra (học viên theo bài)

### Điều kiện tiên quyết

{% hint style="warning" %}
* Đã đăng nhập vào hệ thống Ops với vai trò Ops Admin hoặc CX
* Bài kiểm tra phải ở trạng thái **Active** hoặc **Locked** thì học viên mới có thể làm bài
* Mỗi Program chỉ được phép có **1 bài kiểm tra Active hoặc Locked** tại một thời điểm
{% endhint %}

***

## II. Chi tiết hướng dẫn

### Entrance Test List — Quản lý danh sách bài kiểm tra đầu vào

<details>

<summary>Xem danh sách &#x26; chi tiết bài kiểm tra</summary>

**Kết quả:** Xem được danh sách bài kiểm tra đầu vào và thông tin chi tiết của từng bài.

1. Vào **Menu → Entrance Test → Entrance Test List**.
2. Danh sách hiển thị các cột:

| Cột       | Mô tả                           |
| --------- | ------------------------------- |
| Test Name | Tên bài kiểm tra                |
| Program   | Chương trình (CFA / ACCA / CMA) |
| Subject   | Môn học                         |
| Duration  | Thời lượng làm bài              |
| Status    | Trạng thái bài kiểm tra         |

3. (Tùy chọn) Tìm kiếm và lọc danh sách theo: **Tên bài kiểm tra**, **Program**, **Subject**, **Status**.
4. Click vào tên bài kiểm tra để xem chi tiết gồm 2 tab:
   * **Test Info**: thông tin cơ bản và cài đặt Settings
   * **Participants**: danh sách học viên đã tham gia bài này

**Các trạng thái bài kiểm tra:**

| Trạng thái      | Ý nghĩa                                                                              |
| --------------- | ------------------------------------------------------------------------------------ |
| **Draft**       | Bản nháp — chưa hiển thị cho học viên, chỉnh sửa toàn bộ                             |
| **Active**      | Đang hoạt động — hiển thị cho học viên trên LMS                                      |
| **Locked**      | Bị khóa — hệ thống tự chuyển khi có học viên nộp bài; chỉ sửa một số trường giới hạn |
| **Deactivated** | Đã hủy — ẩn bài thi, không thể chỉnh sửa hay thêm/xóa học viên                       |

{% hint style="success" %}
Danh sách bài kiểm tra hiển thị thành công → Xem hoàn tất.
{% endhint %}

</details>

<details>

<summary>Tạo mới bài kiểm tra đầu vào</summary>

**Kết quả:** Bài kiểm tra đầu vào mới được tạo thành công ở trạng thái Draft.

{% hint style="warning" %}
**Trước khi bắt đầu:**

* Xác định rõ Program, Subject và thời lượng bài thi
* Chuẩn bị danh sách câu hỏi cho từng Section
{% endhint %}

{% stepper %}
{% step %}
**Tab 1 — Test Info**

1. Click nút **+ Create** (hoặc **Create Entrance Test**).
2. Điền thông tin bài kiểm tra:

| Trường             | Bắt buộc | Mô tả                     |
| ------------------ | -------- | ------------------------- |
| Test Name          | Có       | Tên bài kiểm tra          |
| Program            | Có       | CFA / ACCA / CMA          |
| Subject            | Có       | Môn học tương ứng Program |
| Duration (Hours)   | Có       | Số giờ làm bài            |
| Duration (Minutes) | Có       | Số phút làm bài           |

3. Click **Next** để chuyển sang bước 2.
{% endstep %}

{% step %}
**Tab 2 — Add Sections**

4. Click **+ Add Section** để thêm section.
5. Điền thông tin section:

| Trường              | Bắt buộc | Mô tả                                      |
| ------------------- | -------- | ------------------------------------------ |
| Section Name        | Có       | Tên phần thi (VD: Chuyên ngành, Tiếng Anh) |
| Question Type       | Có       | Loại câu hỏi                               |
| Pass Point          | Có       | Điểm đạt của section                       |
| Nhận xét Pass       | Có       | Nhận xét hiển thị khi học viên đạt         |
| Nhận xét không Pass | Có       | Nhận xét hiển thị khi học viên không đạt   |

6. Click **Add Questions** để thêm câu hỏi vào section.
7. Lặp lại bước 4–6 để thêm các section khác nếu cần.
8. Click **Next** để chuyển sang bước 3.
{% endstep %}

{% step %}
**Tab 3 — Settings**

9. Cài đặt Pass Point và Nhận xét cho từng Question Type:

| Question Type | Pass Point mặc định |
| ------------- | ------------------- |
| Chuyên ngành  | 90                  |
| Tiếng Anh     | 70                  |

10. Điều chỉnh điểm và nhận xét nếu cần.
11. Click **Save** để hoàn tất.
{% endstep %}
{% endstepper %}

{% hint style="success" %}
Bài kiểm tra được tạo thành công ở trạng thái **Draft** → Tạo mới hoàn tất.
{% endhint %}

</details>

<details>

<summary>Chỉnh sửa thông tin &#x26; trạng thái</summary>

**Kết quả:** Thông tin bài kiểm tra hoặc trạng thái được cập nhật thành công.

**Chuyển đổi trạng thái:**

| Từ     | Sang        | Cách thực hiện                                                    |
| ------ | ----------- | ----------------------------------------------------------------- |
| Draft  | Active      | Thủ công — click nút **Active**                                   |
| Active | Draft       | Thủ công — click nút **Draft** (chỉ khi chưa có học viên đăng ký) |
| Active | Locked      | Tự động — hệ thống chuyển khi có học viên nộp bài                 |
| Locked | Deactivated | Thủ công — click nút **Deactivate**                               |

{% hint style="warning" %}
**Quy tắc 1 Active/Locked mỗi Program:**\
Nếu muốn Active bài kiểm tra mới cùng Program → phải Deactivate bài đang Active/Locked trước.
{% endhint %}

**Quyền chỉnh sửa theo trạng thái:**

Chỉnh sửa toàn bộ: Test Info, Sections (bao gồm danh sách câu hỏi), và Settings.Click vào tên bài kiểm tra → Click Edit.Chỉnh sửa thông tin cần thay đổi → Click Save.Quyền chỉnh sửa phụ thuộc vào việc đã có học viên đăng ký chưa:Click vào tên bài kiểm tra → Click Edit.Chỉnh sửa các trường được phép → Click Save.Chỉ được sửa một số trường giới hạn:Click vào tên bài kiểm tra → Click Edit.Chỉnh sửa các trường được phép → Click Save.Không thể chỉnh sửa bất kỳ thông tin nào. Đây là trạng thái cuối — không thể chuyển lại.

{% hint style="success" %}
Thông tin hoặc trạng thái được cập nhật thành công → Chỉnh sửa hoàn tất.
{% endhint %}

</details>

***

### Participants (theo bài thi) — Quản lý học viên của từng bài kiểm tra

<details>

<summary>Xem danh sách học viên &#x26; chi tiết kết quả</summary>

**Kết quả:** Xem được danh sách học viên đã tham gia bài kiểm tra và kết quả chi tiết của từng người.

1. Vào **Entrance Test List** → click tên bài kiểm tra → chọn tab **Participants**.
2. Danh sách hiển thị các cột:

| Cột             | Mô tả                                        |
| --------------- | -------------------------------------------- |
| #               | STT                                          |
| Name            | Họ và tên học viên                           |
| Email           | Email học viên                               |
| Phone           | Số điện thoại                                |
| Entrance Test   | Tên bài kiểm tra                             |
| Status          | Finished / Unfinished                        |
| Result          | Số câu đúng / tổng số câu                    |
| Level           | Phân loại trình độ                           |
| Submission Time | Thời điểm nộp bài                            |
| Source          | Form (tự đăng ký) / Manually (thêm thủ công) |

3. (Tùy chọn) Tìm kiếm và lọc theo: **Tên học viên**, **Status**, **Level**, **Source**, **Sort by**, **Từ ngày / Đến ngày**.
4. Xem chi tiết kết quả: Click **Action → View Result** (hoặc click trực tiếp vào tên học viên).

Màn hình kết quả hiển thị:

* **Phân loại Level:**

| Level | Trình độ           |
| ----- | ------------------ |
| IA    | Upper Intermediate |
| IIA   | Intermediate       |
| IB    | Elementary         |
| IIB   | Beginner           |

* Biểu đồ điểm từng Section (xanh = Passed, đỏ = Not Passed).
* **Score Detail**: bảng chi tiết từng câu (#, Question, Section, Type, Result, Time Spent).
* Click vào một câu hỏi để xem: đáp án học viên chọn, đáp án đúng, giải thích.

{% hint style="success" %}
Kết quả bài kiểm tra của học viên hiển thị đầy đủ → Xem hoàn tất.
{% endhint %}

</details>

<details>

<summary>Thêm học viên thủ công</summary>

**Kết quả:** Học viên được thêm vào bài kiểm tra thành công với Source = Manually.

{% hint style="warning" %}
**Trước khi bắt đầu:**\
Bài kiểm tra phải đang ở trạng thái **Active** hoặc **Locked**.
{% endhint %}

Có 2 cách thêm học viên thủ công:

Tại tab Participants của bài kiểm tra, click nút + Add Participants.Tìm kiếm học viên theo tên hoặc email.Chọn học viên cần thêm → Click Add.Tại tab Participants, click Action → Add Participants.Tìm kiếm học viên theo tên hoặc email.Chọn học viên cần thêm → Click Add.

{% hint style="success" %}
Học viên được thêm thành công vào danh sách với Source = **Manually** → Thêm thủ công hoàn tất.
{% endhint %}

</details>

<details>

<summary>Import học viên từ file</summary>

**Kết quả:** Danh sách học viên được import hàng loạt vào bài kiểm tra.

1. Tại tab **Participants**, click nút **Import**.
2. Click **Browse file** để chọn file danh sách học viên từ máy tính.
3. Click **Import** để bắt đầu xử lý.
4. Sau khi import xong, hệ thống hiển thị bảng kết quả:

| Cột        | Mô tả                     |
| ---------- | ------------------------- |
| Source     | Nguồn file đã import      |
| Data       | Tổng số dòng dữ liệu      |
| Successful | Số dòng import thành công |
| Error      | Số dòng bị lỗi            |

5. (Tùy chọn) Click **View log** để xem chi tiết các dòng bị lỗi và nguyên nhân.

{% hint style="success" %}
Học viên hợp lệ được import thành công vào danh sách → Import hoàn tất.
{% endhint %}

</details>

<details>

<summary>Xóa học viên thủ công</summary>

**Kết quả:** Học viên được xóa khỏi danh sách tham gia bài kiểm tra.

{% hint style="danger" %}
**Lưu ý:** Chỉ được xóa học viên có **Source = Manually**. Học viên có Source = Form (tự đăng ký) không thể xóa thủ công.
{% endhint %}

1. Tại tab **Participants**, tìm học viên cần xóa (Source = Manually).
2. Click **Action → Delete**.
3. Xác nhận trong hộp thoại popup → Click **Yes**.

{% hint style="success" %}
Học viên được xóa khỏi danh sách thành công → Xóa hoàn tất.
{% endhint %}

</details>

***

### All Participants — Xem tổng hợp học viên tất cả bài kiểm tra

<details>

<summary>Xem danh sách tổng hợp &#x26; chi tiết kết quả học viên</summary>

**Kết quả:** Xem được toàn bộ học viên đã tham gia kiểm tra đầu vào trên tất cả Program và bài kiểm tra.

1. Vào **Menu → Entrance Test → Participants**.
2. Danh sách hiển thị các cột:

| Cột           | Mô tả                     |
| ------------- | ------------------------- |
| #             | STT                       |
| Name          | Họ và tên học viên        |
| Email         | Email học viên            |
| Phone         | Số điện thoại             |
| Entrance Test | Tên bài kiểm tra đã làm   |
| Status        | Finished / Unfinished     |
| Result        | Số câu đúng / tổng số câu |
| Level         | Phân loại trình độ        |
| CLS           | Customer Life Cycle       |
| Submit Time   | Thời điểm nộp bài         |
| Source        | Form / Manually           |

3. (Tùy chọn) Tìm kiếm và lọc theo: **Tên học viên**, **Program**, **Subject**, **Entrance Test**, **Sort by**, **Từ ngày / Đến ngày**.
4. Xem tổng quan kết quả: click vào tên học viên để mở panel bên phải hiển thị:
   * Thông tin cá nhân: Tên, Email, Số điện thoại, Trường đại học
   * Điểm từng Section và phân loại Level
   * **Kế hoạch tổng hợp** được đề xuất dựa trên kết quả
5. Xem chi tiết bài làm:
   * Click **Action → Test Result**, hoặc
   * Từ panel Participant Detail → click **Test Result**

{% hint style="success" %}
Danh sách và kết quả tổng hợp học viên hiển thị thành công → Xem hoàn tất.
{% endhint %}

</details>

***

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
**Lưu ý quan trọng:**

1. **1 Active/Locked mỗi Program:** Mỗi Program chỉ được có 1 bài kiểm tra Active hoặc Locked tại một thời điểm. Muốn kích hoạt bài mới cùng Program → phải Deactivate bài cũ trước.
2. **Deactivated là trạng thái cuối:** Sau khi Deactivate, bài kiểm tra ẩn khỏi LMS, không thể chỉnh sửa, không thể thêm/xóa học viên và không thể chuyển về trạng thái khác.
3. **Locked do hệ thống tự chuyển:** Không thể chủ động chuyển bài sang Locked — hệ thống tự động khóa khi có học viên nộp bài lần đầu.
4. **Quyền sửa giảm dần theo trạng thái:** Draft → Active → Locked → Deactivated; càng về sau càng ít trường được phép chỉnh sửa.
5. **Xóa học viên:** Chỉ xóa được học viên Source = Manually. Học viên tự đăng ký qua Form không thể xóa thủ công.
{% endhint %}

{% hint style="info" %}
**Mẹo sử dụng:**

1. **Dùng All Participants để tra cứu nhanh:** Khi cần tìm kết quả một học viên mà không biết họ đã làm bài nào, vào Entrance Test → Participants tìm theo tên — nhanh hơn vào từng bài kiểm tra.
2. **Kiểm tra View log sau Import:** Sau mỗi lần import file, luôn click View log để xác nhận các dòng lỗi và import bổ sung nếu cần — tránh bỏ sót học viên.
3. **Kế hoạch tổng hợp trong Participant Detail:** Panel chi tiết học viên trong All Participants hiển thị Kế hoạch tổng hợp được đề xuất dựa trên kết quả kiểm tra — hữu ích để CX tư vấn lộ trình học cho học viên.
{% endhint %}

***

## IV. Lỗi thường gặp

| Lỗi / Tình huống                         | Nguyên nhân                                            | Hướng dẫn xử lý                                                                  |
| ---------------------------------------- | ------------------------------------------------------ | -------------------------------------------------------------------------------- |
| Không Active được bài kiểm tra           | Cùng Program đã có 1 bài đang Active hoặc Locked       | Deactivate bài cũ trước, sau đó Active bài mới                                   |
| Nút Edit bị mờ / không chỉnh sửa được    | Bài đang ở trạng thái Deactivated                      | Trạng thái Deactivated không thể chỉnh sửa — tạo mới bài kiểm tra nếu cần        |
| Một số trường bị khóa khi sửa bài Active | Đã có học viên đăng ký → không cho sửa Program/Subject | Chỉ sửa các trường được phép; xem bảng quyền chỉnh sửa tại Section II            |
| Một số trường bị khóa khi sửa bài Locked | Trạng thái Locked giới hạn chỉ sửa một số trường       | Xem tab Locked trong bảng quyền chỉnh sửa tại Section II                         |
| Import file bị lỗi toàn bộ               | Sai định dạng file hoặc không đúng template            | Download file mẫu từ màn hình Import, điền lại đúng cấu trúc rồi import lại      |
| Không xóa được học viên                  | Học viên có Source = Form (tự đăng ký)                 | Chỉ xóa được Source = Manually — liên hệ admin nếu cần xử lý trường hợp ngoại lệ |

***

📩 Cần hỗ trợ thêm? Liên hệ **it-ba@sapp.edu.vn** hoặc tạo ticket hỗ trợ nội bộ.
