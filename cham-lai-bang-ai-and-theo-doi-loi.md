# Chấm lại bằng AI & theo dõi lỗi

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description | Version |
| -------------- | --------------- | ----- | ------------------ | ------- |
| 18/06/2026     | Nguyễn Duy Hiếu | A     |                    | 1.0.0   |

## I. Giới Thiệu Chung

**Dành cho:** Mentor phụ trách

**Đường dẫn:** https://ops.sapp.edu.vn/

#### Phạm vi & Module liên quan

* **Module chính:** AI Auto Grading – Chấm điểm tự luận
* **Chức năng chính:** Yêu cầu AI chấm lại & theo dõi các câu AI chấm lỗi
* **Bước thực hiện:** AI Regrade từng câu · AI Grade All · Theo dõi AI Grading Failures
* **Module liên quan:**
  * Grading List
  * Marks
  * Test/Quiz List

#### Điều kiện tiên quyết

* Người dùng đang đăng nhập là **Mentor phụ trách** của bài làm.
* Trạng thái bài làm là **"Awaiting Grading"** hoặc **"Regrading"**.
* **AI Grading Count** của câu hỏi/requirement còn dưới **3 lần**.

## II. Hướng dẫn chi tiết

### Chấm lại từng câu (AI Regrade)

> 🎯 _Mục tiêu: Yêu cầu AI chấm lại một câu hỏi/requirement khi kết quả chưa phù hợp._

{% stepper %}
{% step %}
## Tại Section kết quả AI của câu muốn chấm lại, bấm "AI Regrade"

![](<.gitbook/assets/image (780)>)
{% endstep %}

{% step %}
## Popup xác nhận

_"Are you sure to use AI to regrade this question/requirement? All comments/grades you have added will be deleted."_

![](<.gitbook/assets/image (781)>)
{% endstep %}

{% step %}
## Bấm "Yes" để xác nhận

**Kết quả:** AI chấm lại câu đó, AI Grading Count tăng +1. Các comment và điểm chấm tay bổ sung trong câu đó sẽ bị xóa. Kết quả các câu khác không bị ảnh hưởng.
{% endstep %}
{% endstepper %}

### Chấm lại toàn bộ bài (AI Grade All)

> 🎯 _Mục tiêu: Yêu cầu AI chấm lại toàn bộ câu trong bài cùng lúc._

{% stepper %}
{% step %}
## Tại màn chi tiết bài chấm, bấm "AI Grade All" (góc phải trên cùng)

![](<.gitbook/assets/image (782)>)
{% endstep %}

{% step %}
## Bấm "Yes" để xác nhận

![](<.gitbook/assets/image (783)>)

**Kết quả:** AI chấm lại tất cả câu có AI Grading Count < 3. Các câu đã đạt 3 lần bị bỏ qua. Hiển thị báo cáo **"AI Grade All Summary"**:

| Thông tin           | Mô tả                                                   |
| ------------------- | ------------------------------------------------------- |
| Successfully Graded | Số Question/Requirement chấm lại thành công             |
| Failed Grading      | Số Question/Requirement chấm lại thất bại               |
| Skipped Grading     | Số Question/Requirement bỏ qua do đã đạt giới hạn 3 lần |

Từ màn báo cáo, có thể chọn **"Regrade Failed"** hoặc **"Regrade All"**.

{% hint style="warning" %}
**Lưu ý:** Khi AI chấm lại, toàn bộ comment và điểm chấm tay bổ sung sẽ bị xóa. Hãy ghi chú lại trước khi thực hiện. Giới hạn tối đa 3 lần AI chấm cho mỗi câu hỏi/requirement.
{% endhint %}
{% endstep %}
{% endstepper %}

### Theo dõi AI Grading Failures

> 🎯 _Mục tiêu: Theo dõi các câu hỏi bị lỗi AI chưa chấm được để kịp thời chấm bổ sung._

Các màn hình sau có thêm cột **"AI Grading Failures"**:

* **Grading List:** Danh sách toàn bộ bài làm mà Mentor phụ trách.
* **Marks:** Danh sách bài làm theo từng lớp.
* **Test/Quiz Detail:** Danh sách học viên theo từng bài Test.

**Ý nghĩa cột:** Số câu bị lỗi AI / Tổng số câu AI cần chấm (ví dụ: 2/5 = 2 câu bị lỗi trong tổng số 5 câu cần AI chấm).

**Bộ lọc AI Grading Failures:**

* **Yes:** Các bài có ít nhất 1 câu chưa được AI chấm do lỗi.
* **No:** Các bài đã được AI chấm đầy đủ toàn bộ câu tự luận.

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Mỗi câu hỏi/requirement chỉ được AI chấm tối đa **3 lần**.
2. Khi yêu cầu AI chấm lại (Regrade/Grade All), toàn bộ comment và điểm chấm tay bổ sung của câu đó sẽ bị xóa.
3. AI Grade All chỉ chấm lại các câu còn dưới 3 lần; câu đã đạt 3 lần sẽ bị bỏ qua (Skipped).
4. AI có thể cho kết quả khác nhau ở mỗi lần chấm do bản chất mô hình AI; điểm cuối do Mentor xác nhận.
5. Dùng cột/bộ lọc **AI Grading Failures** để phát hiện sớm các bài cần can thiệp thủ công.

### Mẹo sử dụng

1. Ghi chú lại comment/điểm chấm tay trước khi bấm AI Regrade để tránh mất dữ liệu.
2. Tận dụng "AI Grade All" thay vì chấm lại từng câu khi muốn làm mới toàn bộ kết quả.
3. Lọc "AI Grading Failures = Yes" để ưu tiên xử lý các bài còn lỗi.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                          | Nguyên nhân                         | Cách xử lý                                           |
| --------------------------------------------------------- | ----------------------------------- | ---------------------------------------------------- |
| Nút "AI Regrade" bị vô hiệu hóa                           | AI Grading Count đã đạt 3 lần       | Mentor chấm tay thủ công cho câu hỏi đó              |
| "The maximum AI grading count is 3. No attempts remained" | Đã đạt giới hạn 3 lần chấm AI       | Mentor chấm tay thủ công cho câu hỏi đó              |
| Trạng thái "AI Error" sau khi chấm lại                    | AI gặp lỗi kỹ thuật sau 3 lần thử   | Thử "AI Regrade"; nếu vẫn lỗi, chấm tay thủ công     |
| Mất comment/điểm chấm tay sau khi chấm lại                | AI Regrade/Grade All xóa dữ liệu cũ | Ghi chú trước khi chấm lại; nhập lại sau khi AI xong |
| Một số câu bị "Skipped" khi AI Grade All                  | Câu đó đã đạt giới hạn 3 lần        | Chấm tay thủ công cho các câu bị bỏ qua              |
