---
description: >-
  Tài liệu này hướng dẫn người dùng cách sử dụng và thao tác với SIS Operational
  Dashboard - nơi cung cấp các dashboard hỗ trợ theo dõi và phân tích dữ liệu
  vận hành học tập trên hệ thống.
---

# SIS Operational Dashboard

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin / Ops, Giảng viên (Teacher), Quản lý chương trình

**Đường dẫn:** Dashboard → SIS Operational Dashboard
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** SIS Operational Dashboard
* **Bao gồm 5 dashboard:**
  * Tỉ lệ chuyên cần
  * Tỉ lệ đầu vào
  * Phân phối điểm các bài kiểm tra
  * Tỉ lệ ghi điểm trên từng câu/chủ đề kiến thức
  * Tiến độ học trên LMS
* **Module liên quan:** Class Management (dữ liệu lớp học), Test Management (dữ liệu bài kiểm tra), LMS (dữ liệu tiến độ học tập)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Đã có tài khoản và được cấp quyền truy cập hệ thống SIS.
* Đã đăng nhập vào hệ thống.
* Dữ liệu lớp học, bài kiểm tra và tiến độ LMS đã được khởi tạo/đồng bộ trong hệ thống.
{% endhint %}

## II. Tổng quan giao diện

Người dùng truy cập theo đường dẫn **Dashboard → SIS Operational Dashboard** để vào màn hình chức năng Dashboard vận hành SIS.

<figure><img src="../.gitbook/assets/image (1376).png" alt=""><figcaption></figcaption></figure>

Tại giao diện, bấm vào dropdown list **"Chọn loại biểu đồ"** để chọn dashboard muốn xem. Cụm dashboard vận hành gồm 5 dashboard:

* Tỉ lệ chuyên cần
* Tỉ lệ đầu vào
* Phân phối điểm các bài kiểm tra
* Tỉ lệ ghi điểm trên từng câu/chủ đề kiến thức
* Tiến độ học trên LMS

Mỗi dashboard gồm **2 vùng chính**:

* **Vùng Filter:** thiết lập điều kiện lọc để xác định phạm vi dữ liệu.
* **Vùng hiển thị Dashboard:** trực quan hóa dữ liệu bằng biểu đồ và cho phép tương tác (hover/click) để xem chi tiết.
*

```
<figure><img src="../.gitbook/assets/image (1377).png" alt=""><figcaption></figcaption></figure>
```

## III. Hướng dẫn chi tiết

<details>

<summary>Dashboard Tỉ lệ chuyên cần</summary>

Theo dõi và phân tích **tỷ lệ chuyên cần (Attendance Rate)** của học viên theo từng buổi học (session) của một lớp cụ thể. Từ biểu đồ, người dùng có thể nhanh chóng nhận biết buổi học nào đạt hoặc không đạt tỷ lệ chuyên cần mục tiêu, đồng thời tra cứu chi tiết danh sách học viên tương ứng.

{% stepper %}
{% step %}
**Truy cập Dashboard Tỉ lệ chuyên cần**

Tại dropdown list **"Chọn loại biểu đồ"**, bấm chọn **Tỉ lệ chuyên cần**.

<figure><img src="../.gitbook/assets/image (1378).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Áp dụng bộ lọc (Filter)**

<table><thead><tr><th width="90.727294921875">Tên Filter</th><th width="95.72723388671875">Bắt buộc chọn?</th><th width="100.54541015625">Cho phép chọn nhiều?</th><th width="120.818115234375">Phụ thuộc filter khác</th><th>Mô tả</th></tr></thead><tbody><tr><td>Facility</td><td>N</td><td>Có</td><td>Không</td><td>Hiển thị danh sách các cơ sở</td></tr><tr><td>Program</td><td>N</td><td>Không</td><td>Không</td><td>ACCA, CFA, CMA</td></tr><tr><td>Course</td><td>Y</td><td>Không</td><td>Program</td><td>Hiển thị tên khóa học thuộc chương trình đã chọn. Nếu không chọn chương trình thì hiển thị toàn bộ khóa. Chỉ lấy course 4 level.</td></tr><tr><td>From - To</td><td>N</td><td></td><td>Không</td><td>Từ ngày - Đến ngày. Nếu lọc theo thời gian → chỉ lấy các lớp có Start date nằm trong khoảng thời gian lọc.</td></tr><tr><td>Status</td><td>N</td><td>Có</td><td>Không</td><td>Status của lớp (DRAFT, PUBLIC, ENDED)</td></tr><tr><td>Class code</td><td>Y</td><td>Có</td><td>Course + From-to + Status</td><td>Hiển thị Code lớp học thuộc khóa học &#x26; Trạng thái/Thời gian đã chọn. <strong>Được chọn tối đa 4 lớp</strong>, mỗi lớp tương ứng với 1 biểu đồ.</td></tr><tr><td>Section</td><td>N</td><td>Không</td><td>Chọn Khóa học, Lớp học trước mới được chọn Section</td><td>Hiển thị tên các section có trong khóa học đã chọn. Khi lọc theo filter này, các cột sẽ thể hiện các buổi học của lớp thuộc section đó.</td></tr></tbody></table>
{% endstep %}

{% step %}
**Xem biểu đồ Attendance Rate**

Cấu trúc hiển thị của biểu đồ:

* **Tên Dashboard:** _Attendance rate by sessions_ – Biểu đồ thể hiện tỷ lệ chuyên cần theo từng buổi học.
* **Mã lớp học:** Hiển thị mã lớp tương ứng (ví dụ: `ACCA102.46AA`).
* **Tổng số buổi học:** Dòng "Total: X ranges" thể hiện tổng số buổi học (mỗi cột tương ứng 1 buổi).
*   **Biểu đồ cột:**

    * Mỗi cột đại diện cho một buổi học, hiển thị tỷ lệ chuyên cần (%).
    * Đường gạch ngang màu xanh lá thể hiện **ngưỡng mục tiêu 70%**.
    * Cột cao hơn ngưỡng = buổi đạt mục tiêu; cột thấp hơn = chưa đạt.

    <figure><img src="../.gitbook/assets/image (1379).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hover lên cột để xem tooltip chi tiết**

Khi di chuột lên một cột bất kỳ, tooltip hiển thị:

* **Tên buổi học** (ví dụ: _Buổi 1 - Offline - 22/08/2025_)
* **Tỷ lệ chuyên cần (%)** của buổi học
* **Sĩ số** (số học viên có mặt / tổng học viên)

<figure><img src="../.gitbook/assets/image (1380).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào cột để xem danh sách học viên chi tiết**

Khi bấm vào cột, hệ thống mở popup danh sách học viên chi tiết của buổi học tương ứng, bao gồm:

* **ID:** Mã học viên
* **Student Name:** Họ tên học viên
* **Email / Phone:** Thông tin liên hệ
* **Checkin:** Thời điểm điểm danh
* **Status:** Trạng thái chuyên cần — **PRESENT** (Có mặt) / **ABSENT** (Vắng mặt)

Người dùng có thể lọc danh sách theo tên học viên, email, trạng thái, hoặc sắp xếp theo cột bất kỳ.

<figure><img src="../.gitbook/assets/image (1381).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Dashboard Tỉ lệ đầu vào</summary>

Theo dõi phân bố học viên theo từng **level đầu vào (IA, IIA, IB, IIB, Other)** trong một lớp học cụ thể. Từ biểu đồ này, người dùng có thể nhanh chóng nắm được tỷ trọng học viên thuộc từng nhóm level, từ đó đánh giá độ đồng đều và chất lượng đầu vào của lớp.

{% stepper %}
{% step %}
**Truy cập Dashboard Tỉ lệ đầu vào**

Tại dropdown list **"Chọn loại biểu đồ"**, bấm chọn **Tỉ lệ đầu vào**.

<figure><img src="../.gitbook/assets/image (1382).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Áp dụng bộ lọc (Filter)**

| Tên Filter | Bắt buộc chọn? | Cho phép chọn nhiều? | Phụ thuộc filter khác     | Mô tả                                                                                                                             |
| ---------- | -------------- | -------------------- | ------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Facility   | N              | Có                   | Không                     | Hiển thị danh sách các cơ sở                                                                                                      |
| Program    | N              | Không                | Không                     | ACCA, CFA, CMA                                                                                                                    |
| Course     | Y              | Không                | Program                   | Hiển thị tên khóa học thuộc chương trình đã chọn. Chỉ lấy course 4 level.                                                         |
| From - To  | N              |                      | Không                     | Từ ngày - Đến ngày. Chỉ lấy các lớp có Start date nằm trong khoảng thời gian lọc.                                                 |
| Status     | N              | Có                   | Không                     | Status của lớp (DRAFT, PUBLIC, ENDED)                                                                                             |
| Class code | Y              | Có                   | Course + From-to + Status | Hiển thị Code lớp học thuộc khóa học & Trạng thái/Thời gian đã chọn. **Được chọn tối đa 4 lớp**, mỗi lớp tương ứng với 1 biểu đồ. |
{% endstep %}

{% step %}
**Xem biểu đồ Student background distribution**

Cấu trúc hiển thị:

* **Tên Dashboard:** _Student background distribution_ – Biểu đồ thể hiện phân bố học viên theo level đầu vào.
* **Mã lớp học:** Hiển thị ở góc phải phía trên (ví dụ: `CFA105.08`).
* **Tổng số học viên:** Dòng "Total: X students" (ví dụ: _Total: 9 students_).
* **Biểu đồ tròn (Pie Chart):**
  * Mỗi màu đại diện cho một level đầu vào (IA, IIA, IB, IIB, Other).
  * Tỷ lệ phần trăm thể hiện tỷ trọng học viên của từng level trên tổng số.
* **Danh sách các nhóm học viên theo level** (bên phải biểu đồ), gồm: Ký hiệu level, Số lượng học viên / tổng, Tên level đầy đủ - đồng bộ theo màu sắc với biểu đồ.

<figure><img src="../.gitbook/assets/image (1383).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hover lên biểu đồ để xem tooltip chi tiết**

Khi hover vào từng phần của biểu đồ, tooltip hiển thị:

* **Tổng số học viên** trong lớp
* **Số học viên** thuộc level tương ứng
* **Tỷ lệ phần trăm** học viên của level đó

<figure><img src="../.gitbook/assets/image (1384).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào phần biểu đồ để xem danh sách học viên**

Khi bấm vào phần biểu đồ hoặc click vào dòng level bên phải, hệ thống hiển thị popup danh sách học viên chi tiết thuộc level đó.

Danh sách bao gồm:

* **ID:** Mã học viên
* **Student Name:** Họ và tên học viên
* **Email / Phone:** Thông tin liên hệ
* **Duration:** Thời gian học (Từ ngày - Đến ngày)
* **Progress:** Tiến độ học tập (%)

Người dùng có thể tìm kiếm, lọc, hoặc sắp xếp dữ liệu trong bảng theo các tiêu chí mong muốn.

<figure><img src="../.gitbook/assets/image (1385).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Dashboard Phân phối điểm các bài kiểm tra</summary>

Theo dõi phân bố điểm của học viên trong một lớp cho từng bài kiểm tra cụ thể (ví dụ: _F7 Final Test_). Từ đó, giảng viên hoặc bộ phận quản lý có thể nhanh chóng nắm bắt mức độ đồng đều về kết quả học tập, điểm trung bình của lớp, và tỷ lệ học viên đạt hoặc vượt điểm trung bình.

{% stepper %}
{% step %}
**Truy cập Dashboard Phân phối điểm**

Tại dropdown list **"Chọn loại biểu đồ"**, bấm chọn **Phân phối điểm các bài kiểm tra**.

<figure><img src="../.gitbook/assets/image (1386).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Áp dụng bộ lọc (Filter)**

| Tên Filter | Bắt buộc chọn? | Cho phép chọn nhiều? | Phụ thuộc filter khác                    | Mô tả                                                                                                                             |
| ---------- | -------------- | -------------------- | ---------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Facility   | N              | Có                   | Không                                    | Hiển thị danh sách các cơ sở                                                                                                      |
| Program    | N              | Không                | Không                                    | ACCA, CFA, CMA                                                                                                                    |
| Course     | Y              | Không                | Program                                  | Hiển thị tên khóa học thuộc chương trình đã chọn. Chỉ lấy course 4 level.                                                         |
| From - To  | N              | Có                   | Không                                    | Từ ngày - Đến ngày. Chỉ lấy các lớp có Start date nằm trong khoảng thời gian lọc.                                                 |
| Status     | N              | Có                   | Không                                    | Status của lớp (DRAFT, PUBLIC, ENDED)                                                                                             |
| Class code | Y              | Có                   | Course + From-to + Status                | Hiển thị Code lớp học thuộc khóa học & Trạng thái/Thời gian đã chọn. **Được chọn tối đa 4 lớp**, mỗi lớp tương ứng với 1 biểu đồ. |
| Test       | Y              | Không                | Chọn Course trước mới được chọn Bài test | Hiển thị toàn bộ Midterm / Final / Mocktest thuộc khóa học đã chọn.                                                               |
{% endstep %}

{% step %}
**Xem biểu đồ Score Distribution**

Cấu trúc hiển thị:

* **Tên bài test:** Hiển thị tiêu đề biểu đồ.
* **Mã lớp học:** Hiển thị ở góc phải trên, ví dụ: `F703.35 - Final test`.
* **Số range điểm:** Dòng "Total: X ranges" thể hiện số khoảng điểm (ví dụ: _Total: 10 ranges_ tương ứng 0–10, 10–20, ..., 90–100).
* **Điểm trung bình của lớp (Average Score):**
  * Đường đứt nét màu xanh kèm nhãn "Aver. score: 56.06" thể hiện điểm trung bình toàn lớp.
  * Giúp người dùng dễ dàng xác định tỷ lệ học viên đạt trên hoặc dưới điểm trung bình.
*   **Biểu đồ cột (Score Distribution):**

    * Mỗi cột tương ứng với một khoảng điểm (range).
    * Chiều cao của cột thể hiện số lượng học viên đạt điểm nằm trong khoảng đó.

    <figure><img src="../.gitbook/assets/image (1387).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hover lên cột để xem tooltip chi tiết**

Khi di chuột lên một cột bất kỳ, tooltip hiển thị:

* **Tổng số học viên** làm bài kiểm tra
* **Số học viên** đạt điểm trong khoảng tương ứng
* **Tỷ lệ phần trăm (%)** số học viên trong khoảng đó

<figure><img src="../.gitbook/assets/image (1388).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào cột để xem danh sách học viên**

Khi bấm vào một cột bất kỳ, hệ thống mở popup danh sách học viên chi tiết thuộc nhóm điểm đó, bao gồm:

* **ID:** Mã học viên
* **Student Name:** Họ và tên học viên
* **Email / Phone:** Thông tin liên hệ
* **Submission time:** Thời gian nộp bài
* **No of attempt:** Số lần làm bài
* **Score:** Điểm đạt được

Người dùng có thể tìm kiếm, lọc theo trạng thái, hoặc sắp xếp điểm tăng/giảm dần bằng các tùy chọn trên đầu bảng.

<figure><img src="../.gitbook/assets/image (1389).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Dashboard Tỉ lệ ghi điểm trên từng câu/chủ đề kiến thức</summary>

Theo dõi **tỉ lệ ghi điểm (accuracy rate)** của học viên trên từng câu hỏi hoặc chủ đề trong bài kiểm tra. Từ đó, giảng viên có thể nhận biết những câu hoặc phần nội dung học viên làm tốt (tỉ lệ ghi điểm cao) và những phần cần cải thiện (tỉ lệ thấp hơn trung bình).

{% stepper %}
{% step %}
**Truy cập Dashboard Tỉ lệ ghi điểm**

Tại dropdown list **"Chọn loại biểu đồ"**, bấm chọn **Tỉ lệ ghi điểm trên từng câu/chủ đề kiến thức**.

<figure><img src="../.gitbook/assets/image (1390).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Áp dụng bộ lọc (Filter)**

| Tên Filter        | Bắt buộc chọn? | Cho phép chọn nhiều? | Phụ thuộc filter khác                     | Mô tả                                                                                                                                                                          |
| ----------------- | -------------- | -------------------- | ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Facility          | N              | Có                   | Không                                     | Hiển thị danh sách các cơ sở                                                                                                                                                   |
| Program           | N              | Không                | Không                                     | ACCA, CFA, CMA                                                                                                                                                                 |
| Course            | Y              | Không                | Không                                     | Hiển thị tên khóa học thuộc chương trình đã chọn. Chỉ lấy course 4 level.                                                                                                      |
| From - To         | N              | Có                   | Không                                     | Từ ngày - Đến ngày. Chỉ lấy các lớp có Start date nằm trong khoảng thời gian lọc.                                                                                              |
| Status            | N              | Có                   | Không                                     | Status của lớp (DRAFT, PUBLIC, ENDED)                                                                                                                                          |
| Class code        | Y              | Có                   | Course + From-to + Status                 | Hiển thị Code lớp học thuộc khóa học & Trạng thái/Thời gian đã chọn. **Được chọn tối đa 4 lớp**, mỗi lớp tương ứng với 1 biểu đồ.                                              |
| Test              | Y              | Không                | Chọn Course trước mới được chọn Bài test  | Hiển thị toàn bộ Midterm / Final / Mocktest thuộc khóa học đã chọn.                                                                                                            |
| Section Belong To | N              | Không                | Chọn Bài test trước mới được chọn Section | Hiển thị tên các section có trong mục belong to của các câu hỏi trong bài test đã chọn. Khi lọc theo filter này, data có thể thể hiện theo section lớn mà câu hỏi đó thuộc về. |
{% endstep %}

{% step %}
**Xem biểu đồ Accuracy Rate**

Cấu trúc hiển thị:

* **Tên bài test:** Hiển thị tiêu đề biểu đồ.
* **Mã lớp học:** Hiển thị ở góc phải phía trên, ví dụ: `CMA103.08 - Midterm Test - Final Test`.
* **Tổng số câu hỏi:** Dòng "Total: X questions" (ví dụ: _Total: 62 questions_).
*   **Biểu đồ dạng cột kết hợp đường (Column + Line chart):**

    * **Cột màu xanh dương:** biểu thị tỉ lệ ghi điểm của lớp cho từng câu hỏi (Q1, Q2, Q3, …).
    * **Đường màu xanh lá:** biểu thị tỉ lệ ghi điểm trung bình toàn hệ thống (average rate).
    * Khi so sánh, người dùng dễ dàng nhận thấy câu nào học viên lớp làm tốt hơn hoặc kém hơn mức trung bình.

    <figure><img src="../.gitbook/assets/image (615).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hover lên cột để xem tooltip chi tiết**

Khi di chuột vào một cột bất kỳ, tooltip hiển thị:

* **Nội dung kiểm tra:** Section / Topic tương ứng (VD: _Section 4 – Cost Management_)
* **Tỉ lệ ghi điểm của lớp:** tỷ lệ phần trăm học viên trong lớp trả lời đúng câu hỏi đó
* **Tỉ lệ ghi điểm trung bình:** mức trung bình chung giữa các lớp (hoặc toàn hệ thống)

<figure><img src="../.gitbook/assets/image (616).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Dashboard Tiến độ học trên LMS</summary>

Theo dõi mức độ tham gia học tập (engagement) của học viên trên hệ thống LMS theo từng topic hoặc nội dung bài học. Từ đó, giảng viên và quản lý chương trình có thể đánh giá tiến độ học tập của lớp, nhận biết số học viên đã hoàn thành, đang học, hoặc chưa bắt đầu khóa học.

{% stepper %}
{% step %}
**Truy cập Dashboard Tiến độ học trên LMS**

Tại dropdown list **"Chọn loại biểu đồ"**, bấm chọn **Tiến độ học trên LMS**.

<figure><img src="../.gitbook/assets/image (619).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Áp dụng bộ lọc (Filter)**

| Tên Filter      | Bắt buộc chọn? | Cho phép chọn nhiều? | Phụ thuộc filter khác                                     | Mô tả                                                                                                                             |
| --------------- | -------------- | -------------------- | --------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| Facility        | N              | Có                   | Không                                                     | Hiển thị danh sách các cơ sở                                                                                                      |
| Program         | N              | Không                | Không                                                     | ACCA, CFA, CMA                                                                                                                    |
| Course          | Y              | Không                | Program                                                   | Hiển thị tên khóa học thuộc chương trình đã chọn. Chỉ lấy course 4 level.                                                         |
| From - To       | N              | Có                   | Không                                                     | Từ ngày - Đến ngày. Chỉ lấy các lớp có Start date nằm trong khoảng thời gian lọc.                                                 |
| Status          | N              | Có                   | Không                                                     | Status của lớp (DRAFT, PUBLIC, ENDED)                                                                                             |
| Class code      | Y              | Có                   | Course + From-to + Status                                 | Hiển thị Code lớp học thuộc khóa học & Trạng thái/Thời gian đã chọn. **Được chọn tối đa 4 lớp**, mỗi lớp tương ứng với 1 biểu đồ. |
| Section         | N              | Không                | Chọn Course trước mới được chọn Section                   | Hiển thị tên các Section có trong khóa học đã chọn. Khi lọc, mỗi cột sẽ thể hiện tiến độ của các **Subsection** thuộc Section đó. |
| Subsection      | N              | Không                | Chọn Course + Section trước mới được chọn Subsection      | Hiển thị tên các Subsection có trong Section đã chọn. Khi lọc, mỗi cột sẽ thể hiện tiến độ của các **Unit** thuộc Subsection đó.  |
| Unit            | N              | Không                | Chọn Course + Section + Subsection rồi mới được chọn Unit | Hiển thị tên các Unit có trong Subsection đã chọn. Khi lọc, mỗi cột sẽ thể hiện tiến độ của các **Activity** thuộc Unit đó.       |
| Test/Case Study | Y              | Có                   | Chọn Course trước rồi mới chọn filter này                 | Hiển thị tên các Test/Case Study có trong khóa học đã chọn. Khi lọc, mỗi cột sẽ thể hiện tiến độ của test/case study đã chọn.     |
{% endstep %}

{% step %}
**Xem biểu đồ Student engagement on LMS**

Cấu trúc hiển thị:

* **Tên Dashboard:** _Student engagement on LMS_ — Biểu đồ thể hiện tiến độ học tập của học viên trên hệ thống LMS.
* **Khóa học:** Hiển thị tên chương trình/khóa học (ví dụ: _Chartered Financial Analyst – CFA Level I_).
* **Mã lớp học:** Hiển thị ở góc phải trên, ví dụ: `CFA103.44`.
* **Biểu đồ cột:**
  * Mỗi cột tương ứng với một topic/nội dung học (Topic 0, Topic 1, Topic 2, …).
  * Cột được chia thành **3 màu** thể hiện trạng thái học tập:
    * **Completed:** Đã hoàn thành
    * **Studying:** Đang học
    * **Not Started:** Chưa bắt đầu
* **Giá trị (%)** phía trên mỗi cột thể hiện tỉ lệ học viên ở trạng thái tương ứng trong topic đó.

<figure><img src="../.gitbook/assets/image (620).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hover lên cột để xem tooltip chi tiết**

Khi di chuột lên một cột bất kỳ, tooltip hiển thị:

* **Tổng số học viên được học:** Tổng số học viên trong lớp có quyền truy cập topic này.
* **Số học viên hoàn thành:** Học viên đã hoàn thành toàn bộ nội dung topic.
* **Số học viên đang học:** Học viên đang trong quá trình học (progress < 100%).
* **Số học viên chưa học:** Học viên chưa bắt đầu topic.

<figure><img src="../.gitbook/assets/image (621).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click vào topic để xem danh sách học viên chi tiết**

Khi click vào một topic bất kỳ, hệ thống mở popup danh sách chi tiết học viên tương ứng, bao gồm:

* **ID:** Mã học viên
* **Student Name:** Họ và tên học viên
* **Email / Phone:** Thông tin liên hệ
* **Duration:** Thời gian học (Từ ngày – Đến ngày)
* **Progress:** Tiến độ học tập (%) của học viên

Người dùng có thể tìm kiếm, lọc, hoặc sắp xếp theo tiến độ học (Progress) để dễ dàng theo dõi.

<figure><img src="../.gitbook/assets/image (622).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

## IV. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. **Filter Course là bắt buộc** ở hầu hết dashboard; cần chọn Course trước khi chọn được Class code, Test, Section, Subsection, Unit, Test/Case Study.
2. **Class code phụ thuộc** vào Course (và có thể kết hợp From-to + Status) — chọn Course trước, sau đó mới chọn được Class code.
3. Mỗi dashboard chỉ hiển thị **tối đa 4 lớp cùng lúc** (mỗi lớp 1 biểu đồ).
4. Khi lọc theo thời gian (From-to), hệ thống chỉ lấy các lớp có **Start date nằm trong khoảng đã chọn**.
5. Course chỉ lấy dữ liệu ở **cấp 4 level**.
6. Filter **Test** chỉ chọn được sau khi đã chọn Course; chỉ hiển thị Midterm / Final / Mocktest thuộc khóa học đã chọn.
7. Filter **Section / Subsection / Unit** (Dashboard LMS) có quan hệ phân cấp — chọn theo thứ tự Course → Section → Subsection → Unit.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. **Hover lên cột/phần biểu đồ** để xem nhanh số liệu chi tiết trước khi mở popup danh sách học viên.
2. Dùng filter **Section / Subsection / Unit** (Dashboard LMS) để bóc tách tiến độ theo từng cấp nội dung — hữu ích khi cần phân tích sâu một chương cụ thể.
3. So sánh **đường trung bình** với cột của lớp (Dashboard Tỉ lệ ghi điểm, Phân phối điểm) để nhanh chóng nhận biết điểm mạnh/yếu của lớp.
4. Khi cần so sánh **giữa các lớp**, chọn nhiều Class code (tối đa 4) để mỗi lớp hiển thị 1 biểu đồ riêng cạnh nhau.
5. Tại popup danh sách học viên, sử dụng chức năng **tìm kiếm/lọc/sắp xếp** để xử lý danh sách nhanh hơn (đặc biệt với lớp đông học viên).
6. Đường ngưỡng **70% chuyên cần** (Dashboard Tỉ lệ chuyên cần) là tham chiếu nhanh để xác định buổi học cần can thiệp.
{% endhint %}

## V. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                | Nguyên nhân                                                      | Cách xử lý                                                                                                   |
| ----------------------------------------------- | ---------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------ |
| Không chọn được Class code                      | Chưa chọn Course (Class code phụ thuộc Course)                   | Chọn Course trước, có thể kết hợp thêm From-to và Status để thu hẹp danh sách lớp.                           |
| Không chọn được Test / Bài kiểm tra             | Chưa chọn Course                                                 | Chọn Course trước rồi mới chọn được Test.                                                                    |
| Không chọn được Section / Subsection / Unit     | Chưa chọn đủ các filter phụ thuộc theo phân cấp                  | Chọn theo thứ tự: Course → (Class code/Test) → Section → Subsection → Unit.                                  |
| Không hiển thị Course trong dropdown            | Course không thuộc cấp 4 level (hệ thống chỉ lấy course 4 level) | Kiểm tra cấu hình Course tại module quản lý khóa học.                                                        |
| Lớp không xuất hiện khi lọc theo thời gian      | Start date của lớp nằm ngoài khoảng From-to đã chọn              | Mở rộng khoảng From-to hoặc bỏ filter thời gian.                                                             |
| Không thể chọn thêm lớp thứ 5 ở Class code      | Mỗi dashboard chỉ hiển thị tối đa 4 lớp                          | Bỏ chọn 1 lớp hiện có trước khi chọn lớp mới.                                                                |
| Tooltip / Popup không hiển thị                  | Có thể do dữ liệu chưa đồng bộ hoặc lớp không có dữ liệu         | Kiểm tra lớp đã có dữ liệu chuyên cần / bài test / tiến độ LMS chưa; làm mới trang nếu cần.                  |
| Không thấy danh sách học viên khi click vào cột | Lớp/buổi học không có học viên hoặc dữ liệu chưa được ghi nhận   | Kiểm tra danh sách học viên của lớp; xác nhận đã có dữ liệu điểm danh / nộp bài / tiến độ học tập tương ứng. |
| Filter bị reset khi đổi Course                  | Class code và các filter cấp dưới phụ thuộc vào Course           | Đây là hành vi đúng — chọn lại Class code và các filter phụ thuộc sau khi đổi Course.                        |
