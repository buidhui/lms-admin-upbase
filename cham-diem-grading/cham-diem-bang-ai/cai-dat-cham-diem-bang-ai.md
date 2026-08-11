# Cài đặt chấm điểm bằng AI

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version | Effective Date |
| -------------- | --------------- | ----- | ------------------ | ------- | -------------- |
| 18/06/2026     | Nguyễn Duy Hiếu | A     |                    | 1.0.0   | 18/06/2026     |

## I. Giới Thiệu Chung

{% hint style="info" %}
**Dành cho:** SX (Study Experience)

**Đường dẫn:** [https://ops.sapp.edu.vn/](https://ops.sapp.edu.vn/)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** AI Auto Grading – Chấm điểm tự luận
* **Chức năng chính:** Cài đặt dữ liệu đầu vào để AI chấm điểm
* **Bước thực hiện:** Grading Files cho câu hỏi · Context File cho khóa học · Cài đặt bài Test/Quiz
* **Module liên quan:**
  * Question Bank
  * Course Management
  * Test/Quiz List
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản có quyền tạo/chỉnh sửa Question và Course.
* Khóa học có **Program Category = "ACCA"** (mục Grading Files / Context File chỉ hiển thị với khóa ACCA).
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Cài đặt Grading Files cho câu hỏi tự luận</summary>

> 🎯 _Mục tiêu: Upload Rubric File và các file hỗ trợ để AI có đủ thông tin chấm điểm câu hỏi tự luận._

{% stepper %}
{% step %}
**Đăng nhập hệ thống OPS**
{% endstep %}

{% step %}
**Từ Menu, vào Course & Materials → Question Bank**
{% endstep %}

{% step %}
**Tạo mới hoặc chỉnh sửa câu hỏi Tự luận thuộc khóa học ACCA**

Câu hỏi có Type = "Essay" và thuộc khóa ACCA (Belong to → Program Category = "ACCA").
{% endstep %}

{% step %}
**Nhập nội dung câu hỏi (Nội dung câu hỏi, Solution...)**
{% endstep %}

{% step %}
**Tại mục "Grading Files for AI", upload file/nhập text**

* **Nếu Question không có Requirement:** Upload tại mục "Grading Files for AI" của Question.

<figure><img src="../../.gitbook/assets/image (1308).png" alt=""><figcaption></figcaption></figure>

* **Nếu Question có Requirement:** Upload tại mục "Grading Files for AI" cho _từng Requirement_.

<figure><img src="../../.gitbook/assets/image (1309).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click "Save" để lưu thông tin**
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chi tiết mục Grading Files for AI</summary>

| Mục             | Bắt buộc? | Số lượng file          | Mô tả                                                                                    |
| --------------- | --------- | ---------------------- | ---------------------------------------------------------------------------------------- |
| **Rubric File** | Y         | Chỉ 1 file hoặc 1 text | File cơ chế chấm điểm cho AI. Nếu không upload, hệ thống cảnh báo và không cho phép lưu. |
| **Other Files** | N         | 1 hoặc nhiều file/text | Các file hỗ trợ bổ sung giúp AI chấm chính xác hơn.                                      |

Mỗi file/text cần điền thêm:

| Trường             | Bắt buộc? | Mô tả                                                                           |
| ------------------ | --------- | ------------------------------------------------------------------------------- |
| Description for AI | Y         | Mô tả ý nghĩa file để AI hiểu cách sử dụng. Tối đa 500 ký tự.                   |
| Show to Students   | Y         | Cho phép file hiển thị cho học viên khi xem đáp án chi tiết. Mặc định: Checked. |

</details>

<details>

<summary>Quy tắc upload file</summary>

| Tiêu chí    | Quy định                                            | Thông báo lỗi                                              |
| ----------- | --------------------------------------------------- | ---------------------------------------------------------- |
| Định dạng   | Word (.doc, .docx), Excel (.xls, .xlsx), PDF (.pdf) | "Only Word, Excel, and PDF files are allowed"              |
| Kích thước  | Tối đa 500MB                                        | "File size must not exceed 500MB"                          |
| Rubric File | Bắt buộc, chỉ 1 file                                | "Only one file can be uploaded" / "This field is required" |

</details>

<details>

<summary>Logic khi chỉnh sửa/xóa Grading Files</summary>

| Tình huống                                                 | Cho phép sửa? | Ảnh hưởng                                                                                      |
| ---------------------------------------------------------- | ------------- | ---------------------------------------------------------------------------------------------- |
| Question chưa dùng trong bài Test nào                      | Có            | Không ảnh hưởng                                                                                |
| Question đã dùng trong Test nhưng chưa có học viên nộp bài | Có            | Không ảnh hưởng                                                                                |
| Question đã dùng trong Test và đã có học viên nộp bài      | Có            | Kết quả các bài AI đã chấm trước không đổi. AI dùng file mới nhất cho các lượt chấm tiếp theo. |

</details>

<details>

<summary>Cài đặt Context File cho khóa học</summary>

> 🎯 _Mục tiêu: Upload các file bối cảnh doanh nghiệp để AI có căn cứ chấm điểm chính xác hơn._

{% stepper %}
{% step %}
**Đăng nhập hệ thống OPS**
{% endstep %}

{% step %}
**Vào Course → Create/Edit Course**
{% endstep %}

{% step %}
**Tại Course Info, chọn Program Category = "ACCA"**

Mục Context File for AI chỉ hiển thị khi chọn ACCA.
{% endstep %}

{% step %}
**Tại mục Resource → Context File for AI, upload các file bối cảnh**

<figure><img src="../../.gitbook/assets/image (1310).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền Description for AI cho từng file (tối đa 500 ký tự)**

<figure><img src="../../.gitbook/assets/image (1311).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click "Save"**
{% endstep %}
{% endstepper %}

{% hint style="info" %}
📝 **Lưu ý:** Context Files không bắt buộc. Kết quả các bài AI đã chấm trước đó không bị ảnh hưởng khi thêm/sửa/xóa Context Files. AI sẽ dùng Context Files mới nhất cho các bài chấm tiếp theo. Cùng quy tắc upload file với Grading Files (Word/Excel/PDF, tối đa 500MB).
{% endhint %}

</details>

<details>

<summary>Cài đặt bài Test/Quiz cho AI chấm tự động</summary>

> 🎯 _Mục tiêu: Cấu hình bài Test/Quiz để AI tự động chấm khi học viên nộp bài._

{% stepper %}
{% step %}
**Đăng nhập hệ thống OPS**
{% endstep %}

{% step %}
**Vào Course → Create/Edit Course → Course Content → Tạo/chỉnh sửa bài Test/Quiz**

Bài Test chứa câu tự luận (Type of Test = Constructed hoặc Mixed) và Manual Grading = "Yes".
{% endstep %}

{% step %}
**Tại mục List Questions, cài đặt câu hỏi tự luận bằng cách ấn "Configure Question"**

<figure><img src="../../.gitbook/assets/image (1312).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn câu hỏi cần add vào bài Test/Quiz**

<figure><img src="../../.gitbook/assets/image (1313).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Cài đặt điểm tối đa (Mark) cho từng Question**

Nếu Question có Requirement, cần cài điểm tối đa cho từng Requirement sao cho _tổng điểm các R = điểm Q_.

<figure><img src="../../.gitbook/assets/image (1314).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sắp xếp thứ tự các câu trong bài Test/Quiz**

<figure><img src="../../.gitbook/assets/image (1315).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Click "Finish"**
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
⚠️ **Lưu ý:** Nếu tổng Mark của các Requirement khác Mark của Question, hệ thống báo lỗi _"Mark of all requirements not equal mark of question"_. Không được chỉnh sửa điểm khi đã có học viên nộp bài cho bài Test đó.
{% endhint %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Mục "Grading Files for AI" và "Context File for AI" chỉ hiển thị với khóa học ACCA.
2. **Rubric File là bắt buộc.** Nếu thiếu Rubric File, AI không thể chấm bài.
3. Định dạng file hợp lệ: Word, Excel, PDF; dung lượng tối đa 500MB.
4. Với Question có Requirement, tổng điểm các Requirement phải bằng điểm của Question.
5. Không chỉnh sửa điểm bài Test khi đã có học viên nộp bài.
6. Khi cập nhật Grading Files/Context Files, các bài AI đã chấm trước đó không đổi; AI dùng file mới nhất cho lượt chấm tiếp theo.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Viết Rubric File rõ ràng với thang điểm cụ thể để AI cho kết quả chính xác nhất.
2. Sử dụng Context Files cho các câu hỏi tình huống doanh nghiệp.
3. Điền Description for AI đầy đủ để AI hiểu đúng vai trò của từng file.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                      | Nguyên nhân                                                 | Cách xử lý                                                         |
| ----------------------------------------------------- | ----------------------------------------------------------- | ------------------------------------------------------------------ |
| Không thấy mục "Grading Files for AI"                 | Câu hỏi không phải loại Tự luận, hoặc không thuộc khóa ACCA | Kiểm tra Type câu hỏi và trường "Belong to" phải gắn với khóa ACCA |
| "This field is required" khi Save câu hỏi             | Chưa upload Rubric File                                     | Upload Rubric File cho câu hỏi/requirement trước khi lưu           |
| "Mark of all requirements not equal mark of question" | Tổng điểm các Requirement khác điểm Question                | Điều chỉnh điểm Mark từng Requirement sao cho tổng = điểm Question |
| "Only Word, Excel, and PDF files are allowed"         | Upload file sai định dạng                                   | Chuyển đổi file về đúng định dạng Word, Excel hoặc PDF             |
| "File size must not exceed 500MB"                     | File quá lớn                                                | Nén hoặc tách file thành các phần nhỏ hơn 500MB                    |
