# AI tự động chấm & Mentor review

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version |
| -------------- | --------------- | ----- | ------------------ | ------- |
| 18/06/2026     | Nguyễn Duy Hiếu | A     |                    | 1.0.0   |

## I. Giới thiệu chung

{% hint style="info" %}
**Dành cho:** Mentor phụ trách

**Đường dẫn:** [https://ops.upbase.asia/](https://ops.upbase.asia/)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** AI Auto Grading – Chấm điểm tự luận
* **Chức năng chính:** AI tự động chấm sau khi học viên nộp & Mentor review kết quả
* **Bước thực hiện:** AI tự động chấm · Xem kết quả AI · Chỉnh sửa kết quả · Hoàn tất chấm bài
* **Module liên quan:**
  * Grading List
  * Marks
  * Test/Quiz List
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập LMS Ops với role **Mentor phụ trách** của bài làm.
* Học viên đã nộp bài và có ít nhất 1 câu được AI chấm thành công.
* Trạng thái bài làm = **"Awaiting Grading"** hoặc **"Regrading"**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>AI tự động chấm bài sau khi học viên nộp</summary>

> Sau khi học viên bấm **"Submit"**, hệ thống tự động xử lý và chuyển bài cho AI chấm.

{% stepper %}
{% step %}
**Hiển thị popup nộp bài thành công**

Trạng thái bài làm chuyển sang **"Awaiting Grading"**.

<figure><img src="../../.gitbook/assets/image (784)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Gửi yêu cầu đến AI để chấm các câu tự luận học viên đã trả lời**

Hệ thống tự động gửi AI chấm những câu tự luận học viên đã nộp (Status = Submitted)

Câu tự luận học viên không làm (Status = Unsubmitted) → Tự động cho 0 điểm.
{% endstep %}

{% step %}
**AI chấm xong → Gửi email cho Mentor phụ trách kèm link bài chấm để review**
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Trạng thái AI chấm bài &#x26; logic quy đổi điểm</summary>

| Trạng thái (Status) | Ý nghĩa                                            |
| ------------------- | -------------------------------------------------- |
| AI Grading          | AI đang xử lý, chưa trả về kết quả                 |
| AI Graded           | AI đã chấm thành công, có điểm và nhận xét         |
| AI Error            | AI gặp lỗi sau 3 lần thử, không trả về kết quả     |
| Not Graded          | AI không xử lý chấm điểm (với các câu Unsubmitted) |

<figure><img src="../../.gitbook/assets/image (785)" alt=""><figcaption></figcaption></figure>

AI chấm theo Rubric với thang điểm tùy chỉnh, hệ thống tự quy đổi về thang điểm của bài Test:

> **Công thức:** Điểm thực = (Điểm AI / Thang điểm Rubric) × Điểm Max của Question/Requirement

</details>

<details>

<summary>Truy cập bài cần chấm</summary>

Các cách truy cập bài cần chấm:

* Click vào link trong email thông báo được gửi sau khi AI chấm xong.
* Vào Academic Management → Class → Grading List → Chọn bài → Action → Grade.
* Vào Academic Management → Class → Class List → Class Detail → Marks → Chọn bài → Action → Grade.

</details>

<details>

<summary>Xem kết quả AI theo từng câu hỏi/requirement</summary>

Tại màn chấm bài, mỗi Question hoặc Requirement có một **Section kết quả AI** (AI Assistant) ở góc phải màn hình, gồm:

| Thông tin          | Mô tả                                                                          |
| ------------------ | ------------------------------------------------------------------------------ |
| AI Grading Count   | Số lần AI đã chấm thành công / Tổng số lần tối đa (mặc định 3 lần)             |
| Status             | AI Graded / AI Error / AI Grading / Not Graded                                 |
| Comment            | Nhận xét của AI (chỉ Edit hoặc Delete, không sửa trực tiếp)                    |
| AI Suggested Grade | Điểm AI đề xuất (đã quy đổi về thang điểm của bài Test)                        |
| Last edited by     | "AI Assisted" nếu AI chấm, tên Mentor nếu Mentor sửa                           |
| Date & Time        | Thời điểm cập nhật gần nhất                                                    |
| Related Files      | Danh sách Rubric File, Other Files và Context File gắn với câu hỏi/requirement |

</details>

<details>

<summary>Chỉnh sửa kết quả AI</summary>

{% stepper %}
{% step %}
**Xem kết quả AI tại Section kết quả AI bên phải**
{% endstep %}

{% step %}
**Bấm "Edit" để sửa Comment và điểm**

<figure><img src="../../.gitbook/assets/image (786)" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (788)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Bấm "Delete" để xóa nhận xét/điểm**

<figure><img src="../../.gitbook/assets/image (790)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Bôi đen từng ý trong bài làm học viên để chấm tay bổ sung thêm điểm**

Mentor có thể bôi đen từng ý trong bài học viên để thực hiện chấm bổ sung (nếu có) như khi thao tác chấm thủ công.
{% endstep %}
{% endstepper %}

{% hint style="info" %}
ℹ️ **Lưu ý tính điểm:** Tổng điểm = Điểm AI + Điểm chấm tay bổ sung. Tổng không được vượt quá điểm tối đa của Question/Requirement. Thông báo lỗi khi vượt: _"Grading score exceeds Question's/Requirement's maximum score"_.
{% endhint %}

</details>

<details>

<summary>Hoàn tất chấm bài</summary>

{% stepper %}
{% step %}
**Click "Finish" → Bấm "Yes"**

<figure><img src="../../.gitbook/assets/image (791)" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (793)" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

{% hint style="success" %}
**Kết quả:** Trạng thái bài làm chuyển sang "Finish Grading". Hệ thống tự động gửi email kết quả cho học viên.
{% endhint %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. AI tự động chấm ngay sau khi học viên nộp bài; câu không làm được tự động cho 0 điểm.
2. Điểm AI được quy đổi về thang điểm bài Test: Điểm thực = (Điểm AI / Thang Rubric) × Điểm Max, làm tròn 2 chữ số thập phân. Điểm âm → mặc định = 0.
3. Comment của AI chỉ có thể **Edit** hoặc **Delete**, không sửa đè trực tiếp.
4. Tổng điểm (AI + chấm tay bổ sung) không được vượt điểm tối đa của Question/Requirement.
5. Hệ thống lưu kết quả gốc từ AI ngay cả khi Mentor đã chỉnh sửa, để phục vụ truy cứu.
6. Kết quả chỉ được gửi cho học viên sau khi Mentor phụ trách click **"Finish"**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Review kỹ Comment & AI Suggested Grade trước khi điều chỉnh điểm.
2. Tận dụng chấm tay bổ sung để cộng điểm cho các ý AI bỏ sót.
3. Chỉ bấm "Finish" sau khi đã rà soát toàn bộ câu trong bài.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                           | Nguyên nhân                              | Cách xử lý                                                  |
| ------------------------------------------ | ---------------------------------------- | ----------------------------------------------------------- |
| Bài chưa được AI chấm sau khi học viên nộp | AI đang xử lý (Status = "AI Grading")    | Chờ AI xử lý xong rồi review lại                            |
| Trạng thái "AI Error"                      | AI gặp lỗi kỹ thuật sau 3 lần thử        | Bấm "AI Regrade" để thử lại; nếu vẫn lỗi, chấm tay thủ công |
| "Grading score exceeds maximum score"      | Tổng điểm vượt quá điểm tối đa           | Giảm điểm chấm tay để tổng không vượt mức tối đa            |
| Không sửa được trực tiếp Comment của AI    | Comment AI chỉ cho phép Edit hoặc Delete | Dùng nút "Edit" để sửa hoặc "Delete" để xóa rồi nhập lại    |
| Học viên chưa nhận được kết quả            | Mentor chưa bấm "Finish"                 | Hoàn tất review và bấm "Finish" → "Confirm"                 |
