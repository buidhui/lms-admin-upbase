# Đồng bộ Hubspot Ticket - LMS

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version | Effective Date |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- | -------------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   | May 18, 2026   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   | Jun 18, 2026   |

## I. Thông tin chung

**Dành cho:** CX, Ticket Owner, Ops/Admin LMS, IT/System Admin

**Đường dẫn:** HubSpot Ticket (bảo lưu/học lại) · LMS: Class List → Class Detail → Students (chuyển nhượng)

#### Phạm vi & Module liên quan

* **Hệ thống thao tác chính:** HubSpot, LMS Operations
* **Module liên quan trên LMS:** Class List, Class Detail, Students
* **Đối tượng dữ liệu liên quan:** HubSpot Ticket, HubSpot Contact, Student, Class, Class Student Status

#### Điều kiện tiên quyết:

* HubSpot đã có Ticket xử lý yêu cầu của học viên, thuộc loại yêu cầu phù hợp (bảo lưu/học lại) và có thông tin học viên tương ứng.
* CX đã trao đổi và xác nhận mã lớp hiện tại và mã lớp mới (nếu có).
* Người dùng có quyền cập nhật trạng thái Ticket trên HubSpot và xem Contact HubSpot.
* LMS đã có dữ liệu lớp hiện tại của học viên.
* Với nghiệp vụ chuyển nhượng: người dùng có quyền truy cập **Class List → Class Detail → Students**.

{% hint style="info" %}
Bảo lưu, học lại, chuyển đổi thao tác trên **Ticket HubSpot** (có đồng bộ về Contact/LMS). Riêng **chuyển nhượng** không đồng bộ HubSpot, xử lý trực tiếp trên LMS. Trạng thái đồng bộ trên Ticket: **Đồng bộ thành công / Đồng bộ thất bại**.
{% endhint %}

## II. Hướng dẫn chi tiết

### Xử lý Ticket bảo lưu / học lại

{% stepper %}
{% step %}
## Mở Ticket trên HubSpot

CX mở Ticket yêu cầu bảo lưu/học lại của học viên trên HubSpot.
{% endstep %}

{% step %}
## Chuyển sang Hỗ trợ chính sách

CX chuyển trạng thái Ticket từ **Tiếp nhận yêu cầu** sang **Hỗ trợ chính sách**, trao đổi với học viên để xác nhận mã lớp hiện tại và mã lớp mới (nếu đã chốt).
{% endstep %}

{% step %}
## Chuyển sang Closed Success

CX chuyển trạng thái Ticket sang **Closed Success**. Hệ thống hiển thị popup yêu cầu nhập thông tin mã lớp.
{% endstep %}

{% step %}
## Nhập Lớp đăng ký chính

CX nhập **Lớp đăng ký chính** (lớp hiện tại học viên muốn bảo lưu/học lại/chuyển đổi). Cần kiểm tra với property **Lớp đăng ký chính** trên Contact của học viên.
{% endstep %}

{% step %}
## Nhập Lớp mới (nếu có)

CX nhập **Lớp mới** nếu học viên đã chốt. Nếu nhập nhiều mã lớp, ngăn cách bằng dấu phẩy — ví dụ: `F102.01, CFA03.25`.
{% endstep %}

{% step %}
## Chọn Save

CX chọn **Save**. Hệ thống bắt đầu đồng bộ thông tin từ Ticket sang Contact và về LMS.
{% endstep %}

{% step %}
## Chờ và load lại trang

CX chờ khoảng **20-30 giây**, sau đó load lại trang Ticket.
{% endstep %}

{% step %}
## Kiểm tra Trạng thái đồng bộ LMS

CX kiểm tra property **Trạng thái đồng bộ LMS**. Nếu **Đồng bộ thành công**: Ticket đã xử lý xong. Nếu **Đồng bộ thất bại**: kiểm tra email để xem lý do lỗi và xử lý lại.
{% endstep %}
{% endstepper %}

### Kết quả xử lý đối với bảo lưu

Khi Ticket bảo lưu đồng bộ thành công:

| Thông tin                         | Cách xử lý                                                                          |
| --------------------------------- | ----------------------------------------------------------------------------------- |
| **Lớp đăng ký chính trên Ticket** | Được thay thế bằng mã lớp có hậu tố `R` trên Contact. Ví dụ: `F203.03` → `F203.03R` |
| **Lớp cũ trên LMS**               | Học viên chuyển trạng thái từ **Normal** sang **Reserved**                          |
| **Hiển thị trên LMS Pro**         | Khóa học cũ bị ẩn trên LMS Pro của học viên                                         |
| **Lớp mới trên Ticket**           | Được cập nhật vào trường **Lớp bảo lưu/học lại** trên Contact                       |
| **Lớp mới trên LMS**              | Học viên được thêm vào lớp mới với trạng thái **Reassigned**                        |
| **Quyền học lớp mới**             | Học viên có thể tham gia lớp mới bình thường trên LMS Pro                           |

{% hint style="warning" %}
Người dùng không thể xóa học viên có trạng thái **Reserved** ra khỏi lớp.
{% endhint %}

### Kết quả xử lý đối với học lại

Khi Ticket học lại đồng bộ thành công:

| Thông tin                         | Cách xử lý                                                      |
| --------------------------------- | --------------------------------------------------------------- |
| **Lớp đăng ký chính trên Ticket** | Được giữ nguyên trong trường **Lớp đăng ký chính** trên Contact |
| **Lớp cũ trên LMS**               | Học viên chuyển trạng thái từ **Normal** sang **Retook**        |
| **Hiển thị trên LMS Pro**         | Khóa học cũ bị ẩn trên LMS Pro của học viên                     |
| **Lớp mới trên Ticket**           | Được cập nhật vào trường **Lớp bảo lưu/học lại** trên Contact   |
| **Lớp mới trên LMS**              | Học viên được thêm vào lớp mới với trạng thái **Retaking**      |
| **Quyền học lớp mới**             | Học viên có thể tham gia lớp mới bình thường trên LMS Pro       |

{% hint style="warning" %}
Người dùng không thể xóa học viên có trạng thái **Retook** ra khỏi lớp.
{% endhint %}

### Xử lý lại khi Ticket đồng bộ thất bại

{% stepper %}
{% step %}
## Cách 1 — Xử lý lại trên Ticket hiện tại

1. CX xóa giá trị trong property **Trạng thái đồng bộ LMS** trên Ticket.
2. CX kéo Ticket về trạng thái **Hỗ trợ chính sách**.
3. CX kéo lại Ticket sang trạng thái **Closed Success**.
4. CX nhập lại thông tin chính xác trong popup (chỉ chỉnh sửa mã lớp bị sai, các mã lớp khác giữ nguyên và không xóa).
5. CX chọn **Save** để hệ thống chạy lại quá trình xử lý Ticket.
{% endstep %}

{% step %}
## Cách 2 — Clone Ticket để xử lý lại

1. CX clone Ticket hiện tại sang một Ticket mới.
2. CX điền property **Phân loại yêu cầu dịch vụ** trên Ticket mới.
3. CX kéo Ticket mới sang trạng thái **Closed Success**.
4. CX nhập đầy đủ **Lớp đăng ký chính** và **Lớp mới** (nhập đúng mã lớp theo Ticket cần xử lý lại, chỉ sửa mã bị sai). Ví dụ: Ticket cũ có Lớp đăng ký chính = `F1, F2` và Lớp mới = `F3, F4`; nếu `F2` sai cần sửa thành `F0` thì Ticket mới nhập Lớp đăng ký chính = `F1, F0` và Lớp mới = `F3, F4`.
5. CX chọn **Save** để hệ thống xử lý Ticket mới.
{% endstep %}
{% endstepper %}

### Trường hợp học viên chưa chốt lớp mới

{% stepper %}
{% step %}
## Kéo Ticket sang Closed Success

CX kéo Ticket sang trạng thái **Closed Success**.
{% endstep %}

{% step %}
## Nhập Lớp đăng ký chính, bỏ trống Lớp mới

CX nhập **Lớp đăng ký chính** tại popup và bỏ trống trường **Lớp mới** nếu học viên chưa chốt lớp.
{% endstep %}

{% step %}
## Chọn Save

CX chọn **Save**. Hệ thống vẫn cập nhật Contact, cập nhật trạng thái học viên trong lớp cũ và ẩn lớp cũ trên LMS Pro. Sau khi học viên chốt lớp mới, người dùng thêm học viên vào lớp mới trực tiếp trên LMS và cập nhật mã lớp mới trên Contact.
{% endstep %}
{% endstepper %}

### Trường hợp lớp mới chưa có trên OPS

{% stepper %}
{% step %}
## Kéo Ticket sang Closed Success

CX kéo Ticket sang trạng thái **Closed Success**.
{% endstep %}

{% step %}
## Nhập Lớp đăng ký chính và Lớp mới

CX nhập **Lớp đăng ký chính** và **Lớp mới** tại popup.
{% endstep %}

{% step %}
## Chọn Save

CX chọn **Save**. Hệ thống ghi nhận học viên vào danh sách chờ và gửi email thông báo cho **Ticket Owner**. Khi lớp mới được tạo trên OPS, hệ thống tự động thêm học viên vào lớp đó.
{% endstep %}
{% endstepper %}

### Trường hợp học viên chuyển đổi nhiều lần

{% stepper %}
{% step %}
## Xóa học viên khỏi lớp trung gian

Ops/CX xóa học viên khỏi lớp B trên OPS nếu lớp B đang là lớp hiện tại cần chuyển đi.
{% endstep %}

{% step %}
## Tạo Ticket mới

CX tạo một Ticket mới trên HubSpot.
{% endstep %}

{% step %}
## Kéo Ticket sang Closed Success

CX kéo Ticket mới sang trạng thái **Closed Success**.
{% endstep %}

{% step %}
## Nhập lớp hiện tại và lớp mới

CX nhập **Lớp đăng ký chính = Lớp B** và **Lớp mới = Lớp C** trong popup.
{% endstep %}

{% step %}
## Chọn Save

CX chọn **Save**. Hệ thống xử lý và thêm học viên vào lớp C theo logic chuyển đổi thông thường.
{% endstep %}
{% endstepper %}

### Thêm chuyển nhượng cho học viên (trên LMS)

{% stepper %}
{% step %}
## Truy cập danh sách học viên trong lớp

Ops/Admin truy cập **Class List → chọn lớp cần xử lý → Students**.
{% endstep %}

{% step %}
## Chọn Action → Transfer to

Ops/Admin chọn **Action → Transfer to** tại học viên cần chuyển nhượng. Hệ thống điều hướng đến màn hình chọn người nhận chuyển nhượng.
{% endstep %}

{% step %}
## Chọn người nhận chuyển nhượng

Ops/Admin chọn một học viên là người nhận chuyển nhượng. Danh sách chỉ hiển thị các học viên trong lớp đủ điều kiện.
{% endstep %}

{% step %}
## Chọn Add

Ops/Admin chọn **Add** để xác nhận. Nếu chưa chọn học viên mà nhấn Save, hệ thống hiển thị lỗi yêu cầu chọn người nhận.
{% endstep %}

{% step %}
## Kiểm tra kết quả

Sau khi hoàn tất: học viên chuyển nhượng chuyển từ Normal sang **Transferred to**; học viên nhận chuyển nhượng chuyển từ Normal sang **Be transferred**.
{% endstep %}
{% endstepper %}

### Hủy chuyển nhượng cho học viên (trên LMS)

{% stepper %}
{% step %}
## Truy cập danh sách học viên trong lớp

Ops/Admin truy cập **Class List → chọn lớp cần xử lý → Students**.
{% endstep %}

{% step %}
## Chọn Action → Hủy chuyển nhượng

Ops/Admin chọn **Action → Hủy chuyển nhượng** tại học viên đã chuyển nhượng. Hệ thống hiển thị popup xác nhận.
{% endstep %}

{% step %}
## Xác nhận hủy chuyển nhượng

Ops/Admin chọn **Hủy chuyển nhượng** tại popup. Hệ thống chuyển trạng thái của cả học viên chuyển nhượng và học viên nhận chuyển nhượng về **Normal**. (Chọn **Đóng** để không thực hiện.)
{% endstep %}

{% step %}
## Kiểm tra kết quả

Sau khi hoàn tất: học viên chuyển nhượng và học viên nhận chuyển nhượng đều về trạng thái **Normal**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Với bảo lưu, học lại và chuyển đổi: thao tác trên **Ticket HubSpot**; hệ thống tự đồng bộ về Contact và LMS.
2. Cần kiểm tra mã lớp hiện tại với property **Lớp đăng ký chính** trên Contact trước khi xử lý Ticket.
3. Khi nhập nhiều mã lớp trong cùng một property, các mã lớp phải được ngăn cách bằng dấu phẩy.
4. Sau khi chọn **Save** tại popup Ticket, chờ khoảng **20-30 giây** rồi load lại trang để kiểm tra **Trạng thái đồng bộ LMS**.
5. Nếu Ticket đồng bộ thất bại, kiểm tra email để xem lý do lỗi; khi xử lý lại chỉ chỉnh sửa mã lớp bị sai, không xóa các mã lớp đúng.
6. Học viên ở trạng thái **Reserved, Retook** hoặc **Moved out** không thể bị xóa khỏi lớp.
7. Chuyển nhượng không đồng bộ với HubSpot, chỉ xử lý trực tiếp trên LMS.
8. Nút **Transfer to** / **Hủy chuyển nhượng** chỉ hiển thị nếu học viên đủ điều kiện.

### Quy tắc bảo lưu

| Quy tắc              | Mô tả                                                    |
| -------------------- | -------------------------------------------------------- |
| Lớp cũ trên Contact  | Mã lớp đăng ký chính được đổi sang mã có hậu tố `R`      |
| Lớp cũ trên LMS      | Học viên chuyển từ Normal sang Reserved                  |
| Lớp cũ trên LMS Pro  | Bị ẩn với học viên                                       |
| Lớp mới trên Contact | Được cập nhật vào trường Lớp bảo lưu/học lại             |
| Lớp mới trên LMS     | Học viên được thêm vào lớp mới với trạng thái Reassigned |
| Xóa khỏi lớp cũ      | Không cho phép xóa học viên Reserved khỏi lớp            |

### Quy tắc học lại

| Quy tắc              | Mô tả                                                  |
| -------------------- | ------------------------------------------------------ |
| Lớp cũ trên Contact  | Mã lớp đăng ký chính được giữ nguyên                   |
| Lớp cũ trên LMS      | Học viên chuyển từ Normal sang Retook                  |
| Lớp cũ trên LMS Pro  | Bị ẩn với học viên                                     |
| Lớp mới trên Contact | Được cập nhật vào trường Lớp bảo lưu/học lại           |
| Lớp mới trên LMS     | Học viên được thêm vào lớp mới với trạng thái Retaking |
| Xóa khỏi lớp cũ      | Không cho phép xóa học viên Retook khỏi lớp            |

### Quy tắc chuyển đổi/chuyển lớp

| Quy tắc              | Mô tả                                                 |
| -------------------- | ----------------------------------------------------- |
| Lớp cũ trên Contact  | Mã lớp cũ bị xóa khỏi trường Lớp đăng ký chính        |
| Lớp cũ trên LMS      | Học viên chuyển từ Normal sang Moved out              |
| Lớp cũ trên LMS Pro  | Bị ẩn với học viên                                    |
| Lớp mới trên Contact | Được cập nhật vào trường Lớp đăng ký chính            |
| Lớp mới trên LMS     | Học viên được thêm vào lớp mới với trạng thái Move in |
| Xóa khỏi lớp cũ      | Không cho phép xóa học viên Moved out khỏi lớp        |

### Quy tắc chuyển nhượng

| Quy tắc                        | Mô tả                                                                |
| ------------------------------ | -------------------------------------------------------------------- |
| Đồng bộ HubSpot                | Không đồng bộ với HubSpot                                            |
| Nơi thao tác                   | Thực hiện trực tiếp trên LMS tại Class Detail → Students             |
| Điều kiện hiển thị Transfer to | Loại lớp = Lesson, trạng thái học viên = Normal, Progress = 0%       |
| Người nhận chuyển nhượng       | Là học viên trong lớp đủ điều kiện, Progress = 0%, trạng thái Normal |
| Sau khi chuyển nhượng          | Người chuyển nhượng = Transferred to, người nhận = Be transferred    |
| Điều kiện hủy chuyển nhượng    | Loại lớp = Lesson, học viên có trạng thái Transferred to             |
| Sau khi hủy chuyển nhượng      | Cả hai học viên được chuyển về Normal                                |

### Mẹo sử dụng

1. Trước khi kéo Ticket sang **Closed Success**, nên kiểm tra kỹ mã lớp hiện tại và mã lớp mới để tránh đồng bộ lỗi.
2. Nếu nhập nhiều mã lớp, nên dùng đúng dấu phẩy để phân tách.
3. Nếu học viên chưa chốt lớp mới, có thể bỏ trống trường **Lớp mới** để hệ thống chỉ xử lý lớp cũ trước.
4. Nếu lớp mới chưa có trên OPS, vẫn có thể nhập mã lớp mới để hệ thống đưa học viên vào danh sách chờ.
5. Khi Ticket đồng bộ thất bại, nên ưu tiên xử lý lại trên Ticket hiện tại nếu lỗi đơn giản; clone Ticket nếu cần tạo luồng xử lý mới.
6. Với chuyển nhượng, cần kiểm tra Progress của cả người chuyển và người nhận trước khi thao tác.
7. Sau khi xử lý xong, nên kiểm tra lại cả Contact HubSpot và danh sách Students trên LMS.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                           | Nguyên nhân                                                         | Cách xử lý                                                                                |
| ------------------------------------------ | ------------------------------------------------------------------- | ----------------------------------------------------------------------------------------- |
| Ticket đồng bộ thất bại                    | Nhập sai mã lớp hoặc dữ liệu không hợp lệ                           | Kiểm tra email lỗi, sửa mã lớp và xử lý lại Ticket                                        |
| Không thấy trạng thái đồng bộ LMS cập nhật | Hệ thống chưa xử lý xong hoặc chưa load lại trang                   | Chờ 20-30 giây rồi load lại trang                                                         |
| Nhập nhiều mã lớp nhưng hệ thống xử lý sai | Các mã lớp không được phân tách đúng bằng dấu phẩy                  | Kiểm tra lại format mã lớp                                                                |
| Học viên không được thêm vào lớp mới       | Lớp mới chưa tồn tại trên OPS                                       | Hệ thống đưa vào danh sách chờ; kiểm tra email gửi Ticket Owner                           |
| Không xóa được học viên khỏi lớp cũ        | Học viên đang ở trạng thái Reserved, Retook hoặc Moved out          | Đây là logic đúng của hệ thống                                                            |
| Không thấy nút Transfer to                 | Học viên không đủ điều kiện chuyển nhượng                           | Kiểm tra loại lớp, trạng thái học viên và Progress                                        |
| Không thấy người nhận chuyển nhượng        | Không có học viên đủ điều kiện trong lớp                            | Kiểm tra trạng thái và Progress của học viên nhận                                         |
| Không hủy được chuyển nhượng               | Học viên không ở trạng thái Transferred to hoặc không đúng loại lớp | Kiểm tra trạng thái học viên và loại lớp                                                  |
| Chuyển đổi nhiều lần bị sai lớp            | Chưa xử lý lớp trung gian đúng cách                                 | Xóa học viên khỏi lớp hiện tại trên OPS, tạo Ticket mới và nhập lớp hiện tại/lớp mới đúng |
