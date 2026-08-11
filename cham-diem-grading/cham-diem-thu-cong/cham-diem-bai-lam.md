# Chấm điểm bài làm

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description             | Version | Effective Date |
| -------------- | --------------- | ----- | ------------------------------ | ------- | -------------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | M     | Chuẩn hóa nội dung lên GitBook | 3.2.0   | Jun 24, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Mentor, Mentor chính

**Đường dẫn:** Operations → Class → Test/Quiz → Grade work
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* User đăng nhập thành công vào hệ thống.
* Học viên nộp bài thành công.
* Tài khoản có quyền xem bài làm của học viên.
* Người dùng được giao chấm bài làm của học viên.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>1. Truy cập giao diện chấm bài &#x26; tổng quan màn hình</summary>

**Người dùng truy cập giao diện chấm bài bằng 1 trong 4 cách:**

{% stepper %}
{% step %}
**Cách 1 — Từ email:** Click vào link chấm bài được gửi qua mail cho người được giao chấm.
{% endstep %}

{% step %}
**Cách 2 — Từ Test/Quiz trong lớp:** Click vào bài kiểm tra cần chấm → chọn **Grade work** tại nút Action tương ứng với học viên.
{% endstep %}

{% step %}
**Cách 3 — Từ Grading List:** Chọn **Grade** tại màn Grading List.
{% endstep %}

{% step %}
**Cách 4 — Từ Test/Quiz Detail:** Chọn **Grade** tại Test/Quiz Detail trong Class Detail.
{% endstep %}
{% endstepper %}

**Giao diện chấm bài hiển thị các thông tin:**

* **Tên bài kiểm tra.**
* **Total:** tổng điểm, gồm Điểm trắc nghiệm (Multiple Choice) và Điểm tự luận (Constructed). Tổng điểm cập nhật liên tục khi thêm điểm cho câu tự luận.
* **Danh sách câu hỏi** (click để chuyển câu):
  * Màu **đỏ:** câu trắc nghiệm học viên trả lời chưa chính xác.
  * Màu **xanh:** câu trắc nghiệm trả lời đúng, hoặc câu tự luận đã chấm điểm.
  * Màu **xám:** câu tự luận chưa được chấm điểm.
* **Khu vực câu hỏi:** số thứ tự câu, trạng thái (Correct/Incorrect với trắc nghiệm; Submitted/Unsubmitted với tự luận), % trả lời đúng, Time Spent, Grade.

**Bộ lọc câu hỏi:**

* **Graded/Correct:** câu tự luận đã chấm / câu trắc nghiệm trả lời đúng.
* **Incorrect:** câu trắc nghiệm trả lời sai.
* **Chưa chấm:** câu tự luận chưa được chấm.

</details>

<details>

<summary>2. Chấm câu trả lời bằng File</summary>

{% stepper %}
{% step %}
**Xem bài làm:** Click vào câu hỏi tự luận cần chấm để xem bài làm; click **View Solution** để xem lời giải chi tiết.
{% endstep %}

{% step %}
**Tải file bài làm về máy:** Click vào tên file hoặc nút **Download** để tải file trả lời của học viên và chấm điểm/bình luận trên file.
{% endstep %}

{% step %}
**Tải file đã chấm lên hệ thống:** Chọn **Upload graded file** → chọn file từ thiết bị → **Save**.
{% endstep %}

{% step %}
**Điền điểm & lưu:** Sau khi upload thành công, điền điểm cho phần trả lời và chọn **Save** để lưu, hoặc **Cancel** để hủy (khi Cancel, file chấm điểm cũng bị xóa).
{% endstep %}

{% step %}
**Xóa file (nếu cần):** Click biểu tượng **Xóa** → **Yes** để xác nhận. Lưu ý: điểm đã chấm gắn với file cũng sẽ bị xóa.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>3. Chấm câu trả lời bằng Word/Excel trên hệ thống</summary>

{% stepper %}
{% step %}
**Bôi đoạn cần chấm:** Khi bôi đoạn, màn hình hiển thị 2 lựa chọn: **Comment** và **Grading**.
{% endstep %}

{% step %}
**Chọn hành động:**

* **Comment:** bắt buộc để lại bình luận cho đoạn đã bôi, có thể thêm điểm hoặc không.
* **Grading:** bắt buộc chấm điểm cho đoạn đã bôi, có thể thêm bình luận hoặc không.
{% endstep %}

{% step %}
**Lưu:** Sau khi thêm bình luận/điểm, chọn **Save**.

Lưu ý: tổng điểm toàn bộ câu hỏi không được vượt quá số điểm đã cài đặt cho câu hỏi đó, nếu không hệ thống sẽ báo lỗi.
{% endstep %}

{% step %}
**Chỉnh sửa / xóa:** Chọn biểu tượng **Chỉnh sửa** → thay đổi thông tin → **Save**; hoặc biểu tượng **Xóa** → **Yes** để xóa bình luận/điểm đã thêm.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>4. Thêm bình luận &#x26; hoàn tất</summary>

{% stepper %}
{% step %}
**Thêm bình luận & gợi ý cải thiện:** Click **biểu tượng mũi tên xuống** ở góc trên cùng bên phải → **Comment & Recommendations** → điền thông tin → **Save**.
{% endstep %}

{% step %}
**Hoàn tất & gửi kết quả:** Click **biểu tượng mũi tên xuống** → **Finish** để gửi kết quả bài kiểm tra cho học viên.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ chấm các câu học viên đã trả lời (Submitted); câu Unsubmitted được tự động chấm 0.
2. Tổng điểm một câu hỏi không được vượt quá điểm cài đặt của câu đó.
3. Có thể thoát giữa chừng (đóng trình duyệt hoặc Exit) — việc chấm được lưu đến thời điểm thoát.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                | Nguyên nhân                                 | Hướng dẫn khắc phục                                    |
| ------------------------------- | ------------------------------------------- | ------------------------------------------------------ |
| Không lưu được điểm             | Tổng điểm vượt quá điểm cài đặt của câu hỏi | Giảm điểm cho phù hợp với mức tối đa của câu           |
| Mất file đã chấm sau khi Cancel | Cancel sẽ xóa file chấm điểm đã upload      | Upload lại file và điền điểm, chọn Save thay vì Cancel |
| Không thấy nút Grade work       | Chưa được giao chấm hoặc thiếu quyền        | Liên hệ Mentor chính để được giao bài / cấp quyền      |
