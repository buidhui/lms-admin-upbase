# Tạo lớp học

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 25, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |
| May 18, 2026   |               |       |                                |         |

## I. Thông tin chung

**Dành cho:** Admin, Ops User, CX User

**Đường dẫn:** Class → Class List → Create Class

#### Phạm vi & Module liên quan

* **Module chính:** Class
* **Chức năng chính:** Create Class
* **Module liên quan:** Course, Program, Subject, Exam, Student, Mentor, Teacher, Foundation Class, Hybrid Class

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Class**.
* Tài khoản có quyền tạo mới lớp học.

## II. Hướng dẫn chi tiết

### Tạo mới lớp học (thông tin cơ bản)

{% stepper %}
{% step %}
## Chọn Create Class

Admin chọn **Create Class** tại màn hình **Class List**. Hệ thống mở màn hình **Create Class**.

![](<../.gitbook/assets/image (193)>)

![](<../.gitbook/assets/image (195)>)
{% endstep %}

{% step %}
## Nhập Name và Code

Admin nhập **Name** và **Code** tại màn hình **Create Class**. Mỗi lớp cần có một mã duy nhất (mã lớp phải có ký tự ".").
{% endstep %}

{% step %}
## Chọn Construction Mode và Facility

Admin chọn **Construction Mode** và **Facility**. Nếu Construction Mode là **Offline** hoặc **Blended**, Admin cần chọn Facility.

![](<../.gitbook/assets/image (197)>)
{% endstep %}

{% step %}
## Chọn Type và nhập Số học viên tối đa

| Type         | Mô tả                 |
| ------------ | --------------------- |
| **Lesson**   | Lớp học chính.        |
| **Trial**    | Lớp học thử.          |
| **Revision** | Lớp ôn tập/luyện tập. |

Người dùng chỉ có thể tạo các lớp có Type là **Lesson**, **Trial** hoặc **Revision**. Lớp **Foundation** sẽ do hệ thống tự động tạo khi khóa học Normal thuộc Lesson Class có gắn với Foundation Course.
{% endstep %}

{% step %}
## Tick Create Hybrid Class (nếu cần)

![](<../.gitbook/assets/image (199)>)

Admin tick **Create Hybrid Class** và nhập **Hybrid Class Code** nếu cần tạo lớp Hybrid. Checkbox này chỉ hiển thị khi Construction Mode là **Offline/Blended** và Type là **Lesson**.
{% endstep %}

{% step %}
## Tick Cho phép học viên chọn kỳ thi (nếu cần)

![](<../.gitbook/assets/image (201)>)

Admin tick **Cho phép học viên chọn kỳ thi** nếu cần tạo lớp revision bán độc lập mà HV được phép chọn kỳ thi khi vào lớp. Checkbox này chỉ hiển thị khi Type của lớp là **Revision** và **lớp được tạo thủ công** (không phải lớp được tạo tự động gán với kỳ thi cụ thể).
{% endstep %}

{% step %}
## Nhập Duration (nếu Construction Mode = Online LMS)

| Kiểu Duration | Mô tả                                                        |
| ------------- | ------------------------------------------------------------ |
| **Fixed**     | Lớp kết thúc trong khoảng Start Date - End Date.             |
| **Flexible**  | Thời hạn lớp phụ thuộc vào ngày học viên khởi động khóa học. |
{% endstep %}

{% step %}
## Nhập Standard Schedule (nếu Construction Mode khác Online LMS)

Một lịch học gồm **Day of week** và **Start time - End time**.

![](<../.gitbook/assets/image (203)>)
{% endstep %}

{% step %}
## Nhập Number of Extended Days và Reason of Extension (nếu có gia hạn)

Nếu **Number of Extended Days** có giá trị, **Reason of Extension** là trường bắt buộc.

![](<../.gitbook/assets/image (204)>)
{% endstep %}
{% endstepper %}

### Gắn khóa học cho lớp

{% stepper %}
{% step %}
## Chọn trường Course

Admin chọn trường **Course** tại màn hình **Create Class**. Hệ thống mở màn hình **Add Course**.

![](<../.gitbook/assets/image (205)>)
{% endstep %}

{% step %}
## Tìm kiếm khóa học

Admin tìm kiếm khóa học tại màn hình **Add Course** nếu cần.

![](<../.gitbook/assets/image (206)>)
{% endstep %}

{% step %}
## Chọn khóa học và Add

Admin chọn một khóa học trong danh sách và chọn **Add**. Hệ thống quay lại màn hình **Create Class** và hiển thị khóa học đã chọn.

![](<../.gitbook/assets/image (207)>)
{% endstep %}
{% endstepper %}

### Nhập Class Owner và CX Admin

{% stepper %}
{% step %}
## Kiểm tra điều kiện bắt buộc

![](<../.gitbook/assets/image (208)>)

Admin kiểm tra điều kiện bắt buộc của **Class Owner** và **CX Admin** sau khi chọn **Type** và **Course**. Hai trường này bắt buộc khi **Type = Lesson** và Course thuộc một trong các program **ACCA, CFA, CMA, Cert/Dip, CGMA**.
{% endstep %}

{% step %}
## Nhập và chọn Class Owner

Admin nhập tên hoặc email nhân viên tại trường **Class Owner**, sau đó chọn nhân viên phù hợp trong danh sách gợi ý.
{% endstep %}

{% step %}
## Nhập và chọn CX Admin

Admin nhập tên hoặc email nhân viên tại trường **CX Admin**, sau đó chọn nhân viên phù hợp trong danh sách gợi ý.
{% endstep %}
{% endstepper %}

### Gắn kỳ thi cho lớp

{% stepper %}
{% step %}
## Chọn trường Exam

Admin chọn trường **Exam** tại màn hình **Create Class**. Hệ thống mở màn hình **Add Exam**.

![](<../.gitbook/assets/image (209)>)
{% endstep %}

{% step %}
## Tìm kiếm kỳ thi

Admin tìm kiếm kỳ thi tại màn hình **Add Exam** nếu cần.

![](<../.gitbook/assets/image (210)>)
{% endstep %}

{% step %}
## Chọn kỳ thi và Add

Admin chọn một kỳ thi trong danh sách và chọn **Add**. Hệ thống quay lại màn hình **Create Class** và hiển thị kỳ thi đã chọn.
{% endstep %}
{% endstepper %}

### Lưu lớp học

{% stepper %}
{% step %}
## Kiểm tra lại thông tin

Admin kiểm tra lại toàn bộ thông tin đã nhập tại màn hình **Create Class**.
{% endstep %}

{% step %}
## Chọn Save

Admin chọn **Save** tại màn hình **Create Class**. Hệ thống lưu thông tin và tạo mới lớp học.
{% endstep %}

{% step %}
## Nhận thông báo thành công

Hệ thống hiển thị thông báo tạo lớp học thành công.
{% endstep %}
{% endstepper %}

### Hệ thống tự động tạo lớp Hybrid (nếu có chọn Create Hybrid Class)

{% stepper %}
{% step %}
## Tạo lớp gốc kèm lớp Hybrid

Admin tick **Create Hybrid Class**, nhập **Hybrid Class Code** và chọn **Save** tại màn hình **Create Class**. Hệ thống tạo lớp gốc và tự động tạo thêm lớp Hybrid.
{% endstep %}

{% step %}
## Đồng bộ thông tin sang lớp Hybrid

Hệ thống đồng bộ thông tin từ lớp gốc sang lớp Hybrid, gồm: **Status, Facility, Type, Duration, Start Date, End Date, Standard Schedule, Course, Class Owner, CX Admin, Exam, Mentor, Teacher, lịch học và tiến độ giảng viên**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Mã lớp học **Code** phải là duy nhất.
2. Chỉ có thể tạo thủ công các lớp có Type là **Lesson**, **Trial** hoặc **Revision**.
3. Lớp **Foundation** được hệ thống tự động tạo khi Lesson Class gắn với Normal Course có cấu hình Foundation Course.
4. Với lớp **Trial**, mỗi khóa học thử chỉ được gắn với một lớp học; không thể tạo nhiều lớp với cùng một Trial Course.
5. Nếu Construction Mode là **Offline/Blended**, trường **Facility** là bắt buộc; nếu là **Online LMS/Live Online** thì không bắt buộc.
6. Checkbox **Create Hybrid Class** chỉ hiển thị khi Construction Mode là **Offline/Blended** và Type là **Lesson**; khi tick thì bắt buộc nhập **Hybrid Class Code**.
7. Checkbox **Cho phép học viên chọn kỳ thi** chỉ hiển thị khi Type của lớp là **Revision** và **lớp được tạo thủ công**; khi tick checkbox này, HV sẽ được chọn kỳ thi phía LMS pro và chỉ tạo ticket cho CX, **không add HV vào lớp Revision có gán kỳ thi tương ứng khác**.
8. Với lớp **Lesson** có Course thuộc program **ACCA, CFA, CMA, Cert/Dip, CGMA**, hai trường **Class Owner** và **CX Admin** là bắt buộc.
9. Danh sách Course hiển thị theo Type của lớp: Lesson → Normal Course; Revision → Practice Course; Trial → Trial Course.
10. Danh sách Exam hiển thị theo Program của Course đã chọn.
11. Sau khi tạo thành công lớp Hybrid, một số thông tin của lớp Hybrid được đồng bộ từ lớp gốc và không nhập thủ công.

### Quy tắc Standard Schedule

| Quy tắc                     | Mô tả                                                                       |
| --------------------------- | --------------------------------------------------------------------------- |
| Số lượng lịch học tối thiểu | 1 lịch.                                                                     |
| Số lượng lịch học tối đa    | 3 lịch.                                                                     |
| Day of week                 | Chọn một giá trị từ Monday đến Sunday.                                      |
| Thứ 2 - Chủ nhật            | Start time cho phép từ **08:00** trở đi; End time không vượt quá **23:00**. |

### Quy tắc lớp Hybrid được tạo tự động

| Thông tin                                                                                                          | Quy tắc                                                                                 |
| ------------------------------------------------------------------------------------------------------------------ | --------------------------------------------------------------------------------------- |
| **Name**                                                                                                           | Tên lớp gốc + "Hybrid".                                                                 |
| **Construction Mode**                                                                                              | Mặc định là **Hybrid**.                                                                 |
| **Origin Class**                                                                                                   | Mã lớp gốc.                                                                             |
| **Status, Facility, Type, Duration, Start Date, End Date, Standard Schedule, Course, Class Owner, CX Admin, Exam** | Đồng bộ giống lớp gốc.                                                                  |
| **Classroom, Link Meeting, Description, Max Students**                                                             | Để rỗng.                                                                                |
| **Student**                                                                                                        | Lớp Hybrid lưu học viên riêng.                                                          |
| **Mentor**                                                                                                         | Đồng bộ từ lớp gốc.                                                                     |
| **Teacher**                                                                                                        | Đồng bộ từ lớp gốc.                                                                     |
| **Lịch học Offline của lớp gốc**                                                                                   | Đồng bộ sang lớp Hybrid với Learning Mode = Live Online, ngoại trừ thông tin phòng học. |
| **Lịch học Online LMS/Live Online của lớp gốc**                                                                    | Đồng bộ toàn bộ thông tin sang lớp Hybrid.                                              |
| **Tiến độ giảng viên**                                                                                             | Đồng bộ từ lớp gốc.                                                                     |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                        | Nguyên nhân                                                                                | Cách xử lý                                                    |
| --------------------------------------- | ------------------------------------------------------------------------------------------ | ------------------------------------------------------------- |
| Không lưu được lớp học                  | Chưa nhập đủ các trường bắt buộc (Name, Code, Construction Mode, Type, Số học viên tối đa) | Nhập đầy đủ các trường bắt buộc rồi bấm Save                  |
| Báo lỗi mã lớp (Code)                   | Code bị trùng hoặc thiếu ký tự "."                                                         | Đặt mã lớp duy nhất và đảm bảo có ký tự "."                   |
| Bắt buộc nhập Facility                  | Construction Mode là Offline/Blended                                                       | Chọn Facility cho lớp                                         |
| Bắt buộc nhập Class Owner / CX Admin    | Lớp Lesson có Course thuộc ACCA, CFA, CMA, Cert/Dip, CGMA                                  | Nhập đầy đủ Class Owner và CX Admin                           |
| Bắt buộc nhập Reason of Extension       | Đã nhập Number of Extended Days                                                            | Nhập lý do gia hạn tại Reason of Extension                    |
| Không thấy checkbox Create Hybrid Class | Construction Mode/Type không thỏa điều kiện (Offline/Blended + Lesson)                     | Checkbox chỉ hiển thị khi đúng điều kiện nêu trên             |
| Không thấy Course/Exam mong muốn        | Danh sách lọc theo Type của lớp và Program của Course                                      | Chọn đúng Type trước; với Exam chọn Course có Program phù hợp |
| Lỗi Standard Schedule                   | Quá 3 lịch, hoặc Start/End time ngoài khung 08:00–23:00                                    | Nhập tối đa 3 lịch, thời gian trong khung cho phép            |
