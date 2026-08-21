# Đồng bộ Hubspot Deal - LMS

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

**Dành cho:** TVTS / Sales Admin, CX / CX Admin, Admin LMS, IT/System Admin

**Đường dẫn:** HubSpot Deal (property "Trạng thái đồng bộ") → LMS Operations

#### Phạm vi & Module liên quan

* **Module chính:** Đồng bộ Deal → LMS
* **Hệ thống liên quan:** HubSpot, LMS Operations
* **Đối tượng dữ liệu liên quan:** Deal, Student Account, Class, Course, Entry Level

#### Điều kiện tiên quyết:

* Deal đã được chuyển sang trạng thái **WON** (hoặc trạng thái hoàn tất tương ứng theo từng pipeline).
* Deal có đầy đủ thông tin bắt buộc để đồng bộ.
* Người dùng có quyền cập nhật Deal và property **Trạng thái đồng bộ** trên HubSpot.
* LMS đã có lớp tương ứng với mã lớp trên Deal hoặc có cơ chế ghi nhận lớp chờ nếu lớp chưa được tạo.
* Với thao tác đồng bộ lại: Deal cần là Deal đã từng được đồng bộ thành công trước đó.

Các property quan trọng trên Deal: **\[TVTS] Lớp đăng ký chính**, **\[TVTS] Lớp đăng ký tặng kèm**, **\[TVTS] Phân loại Test đầu vào**, **Trạng thái đồng bộ**. Trạng thái đồng bộ: **Chưa đồng bộ, Đồng bộ lại, Đồng bộ thành công, Đồng bộ thất bại**.

## II. Hướng dẫn chi tiết

### Đồng bộ lần đầu khi Deal chuyển sang WON

{% stepper %}
{% step %}
## Tạo Deal trên HubSpot

TVTS/Admin tạo Deal trên HubSpot.
{% endstep %}

{% step %}
## Nhập đầy đủ thông tin bắt buộc

TVTS/Admin nhập họ tên học viên, email đăng ký, số điện thoại, lớp đăng ký chính, lớp đăng ký tặng kèm (nếu có) và trình độ đầu vào trên Deal.
{% endstep %}

{% step %}
## Chuyển Deal sang WON

TVTS/Admin chuyển Deal sang trạng thái **WON**. Hệ thống tự động kích hoạt luồng đồng bộ từ Deal sang LMS.
{% endstep %}

{% step %}
## Hệ thống kiểm tra tài khoản học viên

Nếu email chưa tồn tại trên LMS, hệ thống tạo tài khoản học viên mới. Nếu email đã tồn tại, hệ thống dùng tài khoản hiện có và không tạo trùng.
{% endstep %}

{% step %}
## Hệ thống thêm học viên vào lớp

Hệ thống thêm học viên vào lớp theo thông tin trên Deal, xử lý cả lớp đăng ký chính và lớp đăng ký tặng kèm (nếu có).
{% endstep %}

{% step %}
## Hệ thống cập nhật trạng thái đồng bộ

Nếu đồng bộ thành công, property **Trạng thái đồng bộ** = **Đồng bộ thành công**; nếu lỗi, = **Đồng bộ thất bại**.
{% endstep %}
{% endstepper %}

### Đồng bộ lại khi thay đổi thông tin trên Deal

{% stepper %}
{% step %}
## Mở Deal đã WON

TVTS/Admin mở Deal đã ở trạng thái **WON** trên HubSpot.
{% endstep %}

{% step %}
## Cập nhật thông tin cần thay đổi

TVTS/Admin cập nhật **\[TVTS] Lớp đăng ký chính**, **\[TVTS] Lớp đăng ký tặng kèm** hoặc **\[TVTS] Phân loại Test đầu vào**.
{% endstep %}

{% step %}
## Chọn Đồng bộ lại

TVTS/Admin chọn **Đồng bộ lại** tại property **Trạng thái đồng bộ**. Hệ thống bắt đầu chạy lại luồng đồng bộ dữ liệu từ Deal sang LMS.
{% endstep %}

{% step %}
## Hệ thống xử lý đồng bộ

Hệ thống kiểm tra thay đổi về mã lớp, trình độ đầu vào và cập nhật dữ liệu tương ứng trên LMS.
{% endstep %}

{% step %}
## Hệ thống cập nhật lại trạng thái đồng bộ

Nếu thành công, cập nhật thành **Đồng bộ thành công**; nếu thất bại, **Đồng bộ thất bại**.
{% endstep %}
{% endstepper %}

### Đồng bộ khi thêm mã lớp trên Deal

{% stepper %}
{% step %}
## Thêm mã lớp mới

TVTS/Admin thêm mã lớp mới vào property **\[TVTS] Lớp đăng ký chính** hoặc **\[TVTS] Lớp đăng ký tặng kèm** trên Deal.
{% endstep %}

{% step %}
## Chọn Đồng bộ lại

TVTS/Admin chọn **Đồng bộ lại** tại property **Trạng thái đồng bộ**.
{% endstep %}

{% step %}
## Hệ thống so sánh danh sách lớp

Hệ thống so sánh danh sách lớp hiện tại trên Deal với danh sách đã đồng bộ trước đó để xác định các mã lớp mới chưa được đồng bộ.
{% endstep %}

{% step %}
## Hệ thống thêm học viên vào lớp mới

Nếu lớp đã tồn tại và đã có Course, học viên được thêm trực tiếp. Nếu lớp chưa tồn tại hoặc chưa có Course, hệ thống ghi nhận thông tin để thêm học viên sau khi dữ liệu lớp được hoàn thiện.
{% endstep %}
{% endstepper %}

### Đồng bộ khi xóa mã lớp trên Deal

{% stepper %}
{% step %}
## Xóa mã lớp

TVTS/Admin xóa mã lớp khỏi property **\[TVTS] Lớp đăng ký chính** hoặc **\[TVTS] Lớp đăng ký tặng kèm** trên Deal.
{% endstep %}

{% step %}
## Chọn Đồng bộ lại

TVTS/Admin chọn **Đồng bộ lại** tại property **Trạng thái đồng bộ**.
{% endstep %}

{% step %}
## Hệ thống so sánh danh sách lớp

Hệ thống xác định các mã lớp đã từng đồng bộ nhưng hiện không còn trên Deal.
{% endstep %}

{% step %}
## Hệ thống kiểm tra trạng thái khai giảng

Nếu lớp chưa khai giảng: hệ thống xóa học viên khỏi lớp trên LMS. Nếu lớp đã khai giảng: hệ thống không xóa học viên, gửi email thông báo cho TVTS/CX và tạo task trên HubSpot để xử lý thủ công.
{% endstep %}
{% endstepper %}

### Đồng bộ trình độ đầu vào

{% stepper %}
{% step %}
## Cập nhật Phân loại Test đầu vào

TVTS/Admin cập nhật property **\[TVTS] Phân loại Test đầu vào** trên Deal.
{% endstep %}

{% step %}
## Chọn Đồng bộ lại

TVTS/Admin chọn **Đồng bộ lại** tại property **Trạng thái đồng bộ**.
{% endstep %}

{% step %}
## Hệ thống cập nhật trình độ đầu vào

Hệ thống cập nhật trình độ đầu vào mới của học viên trên LMS theo chương trình tương ứng. Ví dụ: Deal CFA cập nhật từ **Chưa tham dự Test** sang **Nhóm IA** → hệ thống cập nhật trình độ đầu vào CFA từ **NOT\_ATTENDED** sang **IA**.
{% endstep %}
{% endstepper %}

### Xử lý khi đồng bộ thất bại

{% stepper %}
{% step %}
## Kiểm tra Trạng thái đồng bộ

TVTS/Admin kiểm tra property **Trạng thái đồng bộ** trên Deal. Nếu hiển thị **Đồng bộ thất bại**, dữ liệu chưa được đồng bộ thành công sang LMS.
{% endstep %}

{% step %}
## Kiểm tra lại thông tin bắt buộc

TVTS/Admin kiểm tra họ tên học viên, email, số điện thoại, lớp đăng ký chính, lớp tặng kèm (nếu có) và trình độ đầu vào.
{% endstep %}

{% step %}
## Liên hệ IT (nếu cần)

TVTS/Admin liên hệ IT nếu không xác định được nguyên nhân lỗi. IT kiểm tra nguyên nhân và hướng dẫn xử lý.
{% endstep %}

{% step %}
## Cập nhật lại Đồng bộ lại

TVTS/Admin cập nhật lại property **Trạng thái đồng bộ = Đồng bộ lại** sau khi lỗi đã được xử lý. Hệ thống thực hiện lại luồng đồng bộ.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Tính năng này chỉ xử lý đồng bộ dữ liệu từ **Deal trên HubSpot sang LMS**.
2. Deal cần ở trạng thái **WON** để kích hoạt đồng bộ lần đầu.
3. Khi thay đổi thông tin trên Deal sau khi WON, cần chọn **Trạng thái đồng bộ = Đồng bộ lại** để hệ thống cập nhật sang LMS.
4. Email học viên là thông tin quan trọng để xác định tài khoản trên LMS; nếu email đã tồn tại, hệ thống dùng tài khoản hiện có (không tạo trùng).
5. Hệ thống xử lý cả lớp đăng ký chính và lớp đăng ký tặng kèm.
6. Khi thêm mã lớp mới trên Deal: hệ thống thêm học viên vào lớp mới tương ứng trên LMS.
7. Khi xóa mã lớp **chưa khai giảng** khỏi Deal: hệ thống xóa học viên khỏi lớp. Khi xóa mã lớp **đã khai giảng**: hệ thống không tự xóa mà gửi email và tạo task để xử lý thủ công.
8. Nếu đồng bộ thất bại, cần kiểm tra nguyên nhân trước khi chạy lại đồng bộ.

### Quy tắc đồng bộ lần đầu Deal → LMS

| Quy tắc                         | Mô tả                                                                               |
| ------------------------------- | ----------------------------------------------------------------------------------- |
| Trigger đồng bộ                 | Deal được chuyển sang trạng thái WON.                                               |
| Thông tin bắt buộc              | Deal cần có họ tên học viên, email, số điện thoại, lớp đăng ký và trình độ đầu vào. |
| Tạo tài khoản LMS               | Nếu email chưa tồn tại trên LMS, hệ thống tạo tài khoản học viên mới.               |
| Không tạo trùng tài khoản       | Nếu email đã tồn tại, hệ thống dùng tài khoản hiện có.                              |
| Thêm học viên vào lớp           | Hệ thống thêm học viên vào lớp chính và lớp tặng kèm theo Deal.                     |
| Lớp chưa tồn tại/chưa có Course | Hệ thống ghi nhận thông tin để thêm học viên sau khi dữ liệu lớp được hoàn thiện.   |

### Quy tắc đồng bộ lại Deal → LMS

| Trường hợp                                   | Quy tắc xử lý                                                                    |
| -------------------------------------------- | -------------------------------------------------------------------------------- |
| Deal đã từng đồng bộ thành công              | Cho phép đồng bộ lại khi người dùng chọn **Đồng bộ lại**.                        |
| Deal chưa từng đồng bộ thành công            | Hệ thống xử lý theo logic đồng bộ lần đầu nếu Deal đủ điều kiện.                 |
| Thêm mã lớp mới trên Deal                    | Hệ thống thêm học viên vào lớp mới hoặc ghi nhận chờ nếu lớp chưa đủ dữ liệu.    |
| Xóa mã lớp đã đồng bộ và lớp chưa khai giảng | Hệ thống xóa học viên khỏi lớp trên LMS.                                         |
| Xóa mã lớp đã đồng bộ và lớp đã khai giảng   | Hệ thống không xóa học viên khỏi lớp, gửi email và tạo task để TVTS/CX kiểm tra. |
| Cập nhật trình độ đầu vào                    | Hệ thống cập nhật trình độ đầu vào mới trên LMS theo chương trình tương ứng.     |

### Quy tắc trạng thái đồng bộ trên Deal

| Trạng thái         | Quy tắc                                                 |
| ------------------ | ------------------------------------------------------- |
| Chưa đồng bộ       | Deal chưa được đồng bộ sang LMS.                        |
| Đồng bộ lại        | Người dùng kích hoạt hệ thống chạy lại luồng đồng bộ.   |
| Đồng bộ thành công | Dữ liệu Deal đã được đồng bộ thành công sang LMS.       |
| Đồng bộ thất bại   | Hệ thống gặp lỗi, dữ liệu chưa được đồng bộ thành công. |

### Quy tắc xử lý lớp đã khai giảng khi bị xóa khỏi Deal

| Trường hợp          | Quy tắc                                                                                                                |
| ------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| Lớp chưa khai giảng | Hệ thống xóa học viên khỏi lớp trên LMS.                                                                               |
| Lớp đã khai giảng   | Hệ thống không xóa học viên khỏi lớp.                                                                                  |
| Lớp đã khai giảng   | Hệ thống gửi email thông báo cho TVTS/CX.                                                                              |
| Lớp đã khai giảng   | Hệ thống tạo task trên HubSpot để đội phụ trách kiểm tra và xử lý thủ công.                                            |
| Trạng thái đồng bộ  | Trường hợp lớp đã khai giảng và hệ thống đã gửi email/tạo task thành công vẫn được ghi nhận là **Đồng bộ thành công**. |

### Mẹo sử dụng

1. Trước khi chuyển Deal sang WON, nên kiểm tra đầy đủ họ tên, email, số điện thoại, lớp đăng ký và trình độ đầu vào.
2. Khi cập nhật lớp học trên Deal, cần chỉnh sửa đúng property **\[TVTS] Lớp đăng ký chính** hoặc **\[TVTS] Lớp đăng ký tặng kèm**.
3. Sau khi chỉnh sửa Deal, cần chọn **Trạng thái đồng bộ = Đồng bộ lại** để hệ thống cập nhật dữ liệu mới sang LMS.
4. Nếu xóa mã lớp khỏi Deal, nên kiểm tra lớp đó đã khai giảng hay chưa để dự đoán hệ thống sẽ xóa tự động hay tạo task xử lý thủ công.
5. Nếu **Trạng thái đồng bộ** hiển thị **Đồng bộ thất bại**, không nên thao tác lặp nhiều lần liên tục mà cần kiểm tra nguyên nhân lỗi trước.
6. Sau khi đồng bộ thành công, nên kiểm tra lại thông tin học viên và danh sách lớp trên LMS để đảm bảo dữ liệu đã đúng.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                      | Nguyên nhân                                                         | Cách xử lý                                                               |
| ----------------------------------------------------- | ------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| Deal không đồng bộ sang LMS                           | Deal chưa WON hoặc thiếu thông tin bắt buộc                         | Kiểm tra trạng thái Deal và các property cần đồng bộ                     |
| Học viên không được tạo tài khoản mới                 | Email đã tồn tại trên LMS                                           | Kiểm tra tài khoản LMS hiện có của học viên                              |
| Học viên không được thêm vào lớp                      | Mã lớp chưa tồn tại hoặc lớp chưa có Course                         | Kiểm tra Class/Course trên LMS và hoàn thiện dữ liệu lớp                 |
| Đồng bộ lại không chạy                                | Chưa chọn **Đồng bộ lại** tại property Trạng thái đồng bộ trên Deal | Cập nhật lại property và chờ hệ thống xử lý                              |
| Trạng thái đồng bộ = Đồng bộ thất bại                 | Có lỗi dữ liệu hoặc lỗi hệ thống                                    | Liên hệ IT kiểm tra nguyên nhân và chạy lại sau khi xử lý                |
| Xóa mã lớp khỏi Deal nhưng học viên vẫn còn trong lớp | Lớp đã khai giảng nên hệ thống không xóa tự động                    | Kiểm tra email/task được tạo và xử lý thủ công theo quy trình            |
| Trình độ đầu vào không cập nhật                       | Chưa chọn **Đồng bộ lại** hoặc giá trị trên Deal chưa đúng mapping  | Kiểm tra property **\[TVTS] Phân loại Test đầu vào** và chạy lại đồng bộ |
