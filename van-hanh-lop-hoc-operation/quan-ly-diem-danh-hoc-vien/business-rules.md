# Business Rules

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person   | A,M,D | Change Description             | Version |
| -------------- | --------------- | ----- | ------------------------------ | ------- |
| Jun 24, 2026   | Nguyễn Duy Hiếu | A     | Chuẩn hóa nội dung lên GitBook | 1.0.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin CX

**Mục đích:** Mô tả quy tắc hệ thống dùng để xác định điểm danh của học viên từ dữ liệu Zoom và quy tắc gửi email nhắc nhở.
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Chuyên cần học viên (Student Attendance)
* **Hệ thống tích hợp:** Zoom
* **Phạm vi:** lớp Live Online / Hybrid qua Zoom
{% endhint %}

## II. Rule Điểm Danh

{% stepper %}
{% step %}
## Mapping thời gian vào – ra với buổi học

Sau khi ghi nhận thời gian vào – ra của học viên, hệ thống kiểm tra thời gian đó thuộc buổi học nào theo lịch học. Thời gian ra – vào link Zoom được tính là của **buổi học A** nếu **đồng thời** thỏa mãn 2 điều kiện:

```
Start(A) − 60 phút  <  Thời gian học viên VÀO học  <  End(A)
Start(A)            <  Thời gian học viên RỜI buổi <  End(A) + 60 phút
```

**Ví dụ:** lịch cố định buổi A từ 8:00 → 11:00, học viên vào Zoom 7:30 → 11:30 ⇒ hệ thống xác định khoảng 7:30 → 11:30 thuộc buổi A, sau đó tính thời lượng điểm danh theo quy tắc bên dưới.
{% endstep %}

{% step %}
## Tính thời lượng tham gia

* Thời lượng buổi học tính theo **lịch cố định trên LMS**, không theo thời gian host mở lớp thực tế.
  * _VD:_ lịch 8:00 → 11:00, host mở Zoom 7:50 → 11:30 ⇒ thời lượng buổi vẫn tính theo 8:00 → 11:00.
* Thời lượng tham gia = **tổng thời gian có mặt trong khung giờ chính thức của buổi học**; thời gian ngoài khung giờ tự động bị loại bỏ.
  * _VD:_ lịch 8:00 → 11:00, học viên vào 2 lần: 7:45 → 9:00 và 9:10 → 11:15 ⇒ tính từ 8:00 → 9:00 và 9:10 → 11:00.
* Nếu lớp có **phòng chờ**, chỉ tính thời gian sau khi học viên được host thêm vào phòng chính.
* Khi học viên vào – ra nhiều lần hoặc dùng nhiều thiết bị cùng lúc, hệ thống **tự động hợp nhất thời gian và loại bỏ thời gian trùng lặp**.
  * _VD:_ Thiết bị 1: 8:00 → 9:00; Thiết bị 2: 8:45 → 9:30. Khoảng 8:45 → 9:00 bị trùng ⇒ chỉ tính 8:00 → 9:30.
{% endstep %}

{% step %}
## Xác định kết quả điểm danh

| Kết quả                      | Điều kiện                              |
| ---------------------------- | -------------------------------------- |
| **Có điểm danh (Present)**   | Tham gia ≥ **2/3** thời lượng buổi học |
| **Không điểm danh (Absent)** | Tham gia < **2/3** thời lượng buổi học |
{% endstep %}
{% endstepper %}

## III. Rule Gửi Email Nhắc Nhở

<details>

<summary>Điều kiện &#x26; thời điểm gửi email</summary>

* Nếu học viên **vắng mặt 2 buổi học liên tiếp trong cùng 1 lớp**, hệ thống gửi email nhắc nhở vào **8:00 sáng ngày liền sau**.
* **Nội dung email:** theo mẫu nội dung email nhắc nhở chuyên cần (template nội bộ).

</details>

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Mọi mốc thời gian điểm danh đều quy chiếu theo **lịch cố định trên LMS**, không theo thời gian mở lớp thực tế.
2. Ngưỡng để được tính **Có điểm danh** là tham gia **≥ 2/3** thời lượng buổi.
3. Khoảng đệm mapping buổi học là **±60 phút** quanh giờ bắt đầu/kết thúc.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Khi trạng thái điểm danh chưa đúng kỳ vọng, dùng màn "Lịch sử check-in trong ngày" để đối chiếu các khoảng vào – ra theo các quy tắc trên.
{% endhint %}
