# Chấm lại (Regrading)

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | M     | Chuẩn hóa nội dung lên GitBook | 3.2.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Mentor, Mentor chính, Học viên (gửi yêu cầu chấm lại)

**Đường dẫn:** Màn chấm bài (Mentor) / Kết quả bài test (Học viên)
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* User đăng nhập thành công vào hệ thống.
* Học viên nộp bài thành công.
* Tài khoản có quyền xem bài làm của học viên.
* Bài đã được chấm điểm.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>1. Review bài trước khi gửi kết quả</summary>

{% stepper %}
{% step %}
**Gửi bài review:** Khi chấm bài, người dùng chọn **Submit to review** để gửi bài cho Mentor chính review. Mentor chính nhận thông báo qua email.
{% endstep %}

{% step %}
**Mentor chính xử lý:** Trên màn chấm, Mentor chính có 2 lựa chọn:

1. **Chấp nhận & gửi kết quả cho học viên** — chọn Finish, trạng thái chuyển **Finish Grading**, kết quả gửi tới học viên qua Email.
2. **Yêu cầu sửa kết quả chấm (Regrading)** — trạng thái chuyển **Regrading**.
{% endstep %}

{% step %}
**Nhập thông tin Regrading:**

* **Reason:** lý do chấm lại.
* **Mentor:** người chấm (có thể giao bài cho người chấm mới).

Mentor được phân chấm lại sẽ nhận được email thông báo.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>2. Học viên yêu cầu chấm lại (Request Regrading)</summary>

{% stepper %}
{% step %}
**Gửi yêu cầu:** Tại kết quả bài test, học viên chọn **Request Regrading** để yêu cầu chấm lại.
{% endstep %}

{% step %}
**Nhập lý do:** Học viên nhập lý do chấm lại.
{% endstep %}

{% step %}
**Lưu:** Học viên chọn **Save** để lưu yêu cầu. Sau khi gửi thành công, hệ thống gửi thông báo cho Mentor chính.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Chỉ áp dụng chấm lại cho các bài **đã được chấm điểm**.
2. Khi chọn **Finish**, trạng thái thành **Finish Grading** và kết quả được gửi cho học viên; khi chọn **Regrading**, trạng thái thành **Regrading**.
3. Mentor chính có thể giao bài chấm lại cho người chấm mới.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                | Nguyên nhân                              | Hướng dẫn khắc phục                    |
| ------------------------------- | ---------------------------------------- | -------------------------------------- |
| Không thấy Submit to review     | Chưa phải trạng thái cho phép gửi review | Hoàn tất chấm trước khi gửi review     |
| Không gửi được yêu cầu chấm lại | Bỏ trống lý do                           | Học viên cần nhập lý do trước khi Save |
