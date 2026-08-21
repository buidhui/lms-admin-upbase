# Đồng bộ Hubspot Contact - LMS

## Record of changes

{% updates format="full" %}
{% update date="2026-05-29" %}
##

* **Update Person:** Lê Xuân Mai
* **A,M,D:** M
* **Change Description:** Chuẩn hóa nội dung lên GitBook
* **Version:** 4.7.0
{% endupdate %}

{% update date="2026-06-18" %}
##

* **Update Person:** Nhà BA
* **A,M,D:** M
* **Change Description:** Chuẩn hóa component theo template User guide mới nhất
* **Version:** 4.8.0
{% endupdate %}
{% endupdates %}

## I. Thông tin chung

**Dành cho:** Admin LMS/OPS, CX / CX Admin, SX / Study Experience, TVTS / HubSpot User, IT/System Admin

**Đường dẫn:** HubSpot Contact ↔ LMS/OPS (Student Profile)

#### Phạm vi & Module liên quan

* **Module chính:** Student Profile / Student Information Synchronization
* **Hệ thống liên quan:** HubSpot Contact, LMS, OPS
* **Đối tượng dữ liệu liên quan:** Student Account, User Profile, User Contact, Program Information, Exam Information

#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào HubSpot hoặc LMS/OPS và có quyền xem/chỉnh sửa thông tin học viên.
* Học viên trên LMS đã có liên kết với HubSpot Contact thông qua **HubSpot Contact ID**.
* Đồng bộ từ HubSpot về LMS: Contact cần tồn tại và có dữ liệu hợp lệ.
* Đồng bộ từ LMS/OPS lên HubSpot: học viên cần có **HubSpot Contact ID** hợp lệ.
* Đồng bộ thủ công: người dùng cần có quyền chỉnh sửa property **Trạng thái đồng bộ** trên Contact.
* Đồng bộ thất bại: liên hệ IT kiểm tra nguyên nhân trước khi chạy lại.

**Ba chiều đồng bộ:** HubSpot Contact → LMS/OPS; LMS/OPS → HubSpot Contact; HubSpot Merge Contact → LMS. Property **Trạng thái đồng bộ** trên Contact: **Tiến hành đồng bộ, Đồng bộ thành công, Đồng bộ thất bại**.

## II. Hướng dẫn chi tiết

### Đồng bộ thủ công từ HubSpot Contact về LMS/OPS

{% stepper %}
{% step %}
## Mở Contact của học viên trên HubSpot

Người dùng mở **Contact** của học viên trên HubSpot.
{% endstep %}

{% step %}
## Kiểm tra/cập nhật thông tin cần thay đổi

Người dùng cập nhật các thông tin cần thay đổi (họ tên, email, số điện thoại, ngày sinh, trường đại học, chuyên ngành, lĩnh vực công ty, cấp bậc, kỳ thi hoặc kết quả thi).
{% endstep %}

{% step %}
## Chọn Trạng thái đồng bộ = Tiến hành đồng bộ

Người dùng cập nhật property **Trạng thái đồng bộ** thành **Tiến hành đồng bộ**. Hệ thống nhận yêu cầu và bắt đầu cập nhật dữ liệu về LMS/OPS.
{% endstep %}

{% step %}
## Hệ thống xử lý đồng bộ

Hệ thống xác định học viên tương ứng trên LMS/OPS theo HubSpot Contact ID và cập nhật các trường thông tin phù hợp.
{% endstep %}

{% step %}
## Kiểm tra lại Trạng thái đồng bộ

Nếu thành công, property = **Đồng bộ thành công**; nếu lỗi, = **Đồng bộ thất bại**.
{% endstep %}
{% endstepper %}

### Đồng bộ tự động khi thay đổi field trên HubSpot Contact

{% stepper %}
{% step %}
## Cập nhật một trường trên Contact

Người dùng cập nhật một trường thông tin trên HubSpot Contact (ví dụ: số điện thoại, ngày sinh, trường đại học hoặc kết quả thi).
{% endstep %}

{% step %}
## HubSpot gửi thông tin thay đổi về LMS/OPS

Hệ thống nhận dữ liệu thay đổi kèm HubSpot Contact ID.
{% endstep %}

{% step %}
## Hệ thống kiểm tra Contact ID

Nếu Contact ID tồn tại, hệ thống xác định học viên tương ứng để cập nhật. Nếu không tồn tại, hệ thống kết thúc luồng đồng bộ.
{% endstep %}

{% step %}
## Hệ thống cập nhật trường tương ứng

Hệ thống chỉ cập nhật dữ liệu liên quan đến field vừa thay đổi, không cập nhật lại toàn bộ hồ sơ nếu không cần thiết.
{% endstep %}
{% endstepper %}

### Xem thông tin học viên đã đồng bộ trên OPS

{% stepper %}
{% step %}
## Truy cập Student Profile

Người dùng truy cập màn hình **Student Profile** trên OPS.
{% endstep %}

{% step %}
## Mở hồ sơ học viên

Người dùng tìm kiếm và mở hồ sơ học viên cần kiểm tra.
{% endstep %}

{% step %}
## Xem Overview / Personal Information

Hệ thống hiển thị thông tin chung: họ tên, email, số điện thoại, ngày sinh, trường, chuyên ngành, lĩnh vực công ty, cấp bậc, lớp đăng ký chính và lớp bảo lưu/học lại.
{% endstep %}

{% step %}
## Xem thông tin theo chương trình CFA/ACCA/CMA

Người dùng chuyển sang tab/chương trình tương ứng. Hệ thống hiển thị level, kỳ thi, kết quả thi và account ID.
{% endstep %}
{% endstepper %}

### Cập nhật thông tin học viên trên OPS để đồng bộ lên HubSpot

{% stepper %}
{% step %}
## Mở Student Profile trên OPS

Người dùng mở **Student Profile** của học viên trên OPS.
{% endstep %}

{% step %}
## Chọn chỉnh sửa thông tin

Người dùng chọn chỉnh sửa thông tin học viên nếu có quyền. Hệ thống hiển thị các trường được phép chỉnh sửa.
{% endstep %}

{% step %}
## Cập nhật thông tin cần thay đổi

Các trường có thể đồng bộ lên HubSpot gồm Full Name, Email, Phone, D.O.B, University, Major, Field of Work, Position và một số thông tin theo chương trình.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin trên LMS/OPS và đồng bộ các trường tương ứng lên HubSpot Contact.
{% endstep %}

{% step %}
## Kiểm tra lại trên HubSpot (nếu cần)

Nếu đồng bộ thất bại, hệ thống có thể gửi thông báo lỗi cho IT để kiểm tra.
{% endstep %}
{% endstepper %}

### Cập nhật thông tin học viên trên LMS

{% stepper %}
{% step %}
## Mở hồ sơ học viên trên LMS

Người dùng mở màn hình thông tin cá nhân/hồ sơ học viên trên LMS.
{% endstep %}

{% step %}
## Cập nhật trường được phép

Người dùng cập nhật trường được phép chỉnh sửa. Theo phạm vi hiện tại, LMS chủ yếu cho phép cập nhật **Full Name**.
{% endstep %}

{% step %}
## Lưu thông tin

Người dùng lưu thông tin. Hệ thống cập nhật trên LMS và đồng bộ trường tương ứng lên HubSpot Contact nếu học viên có HubSpot Contact ID hợp lệ.
{% endstep %}
{% endstepper %}

### Cập nhật kỳ thi và kết quả thi

{% stepper %}
{% step %}
## Mở Student Profile trên OPS

Người dùng mở **Student Profile** trên OPS.
{% endstep %}

{% step %}
## Chuyển sang chương trình CFA/ACCA/CMA

Người dùng chuyển sang phần thông tin chương trình tương ứng.
{% endstep %}

{% step %}
## Cập nhật Exam

Người dùng cập nhật **Exam** nếu kỳ thi chưa phải kỳ thi chính thức và field cho phép chỉnh sửa. Nếu đã là kỳ thi chính thức, hệ thống không cho phép chỉnh sửa và có thể hiển thị tag **Registered**.
{% endstep %}

{% step %}
## Cập nhật Result

Người dùng cập nhật **Result** nếu field cho phép. Hệ thống lưu kết quả thi tương ứng và đồng bộ lên HubSpot nếu nằm trong phạm vi đồng bộ.
{% endstep %}
{% endstepper %}

### Xử lý khi HubSpot Contact được merge

{% stepper %}
{% step %}
## Merge Contact trên HubSpot

Người dùng thực hiện merge Contact trên HubSpot.
{% endstep %}

{% step %}
## HubSpot gửi webhook merge về LMS

HubSpot gửi webhook merge contact về LMS.
{% endstep %}

{% step %}
## Hệ thống kiểm tra tài khoản tương ứng

Hệ thống LMS kiểm tra các tài khoản học viên tương ứng với các HubSpot Contact ID liên quan.
{% endstep %}

{% step %}
## Hệ thống xác định tài khoản chính

Hệ thống ưu tiên tài khoản có lớp, email chính, source type và thời gian tạo theo logic hệ thống.
{% endstep %}

{% step %}
## Hệ thống merge các tài khoản đủ điều kiện

Nếu tài khoản liên quan đã tồn tại trong lớp và không đủ điều kiện merge, hệ thống không merge và có thể gửi cảnh báo cho IT/Admin.
{% endstep %}

{% step %}
## Hệ thống ghi nhận lịch sử merge

Hệ thống ghi nhận lịch sử merge và cập nhật dữ liệu học viên sau merge.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Tính năng này chỉ áp dụng cho đồng bộ thông tin giữa **HubSpot Contact** và **LMS/OPS** (không dùng cho luồng Deal → LMS).
2. Học viên cần có **HubSpot Contact ID** hợp lệ để đồng bộ hai chiều; nếu Contact ID không tồn tại trong LMS/OPS, hệ thống không xác định được học viên để cập nhật.
3. Một số trường chỉ hiển thị, không cho phép chỉnh sửa trực tiếp trên LMS/OPS: Main Class, Deferred/Retake Class, Account ID, thông tin Deal.
4. Khi chỉnh sửa Email trên LMS/OPS và đồng bộ lên HubSpot, email được cập nhật thành **Primary Email**.
5. Khi cập nhật Exam, nếu đổi kỳ thi thì Result tương ứng có thể bị reset theo rule hệ thống; khi chỉ cập nhật Result, hệ thống không tác động ngược lại thông tin kỳ thi.
6. Nếu đồng bộ lên HubSpot bị lỗi, dữ liệu có thể vẫn được lưu trên LMS/OPS nhưng hệ thống gửi thông báo lỗi cho IT.
7. Nếu đồng bộ từ HubSpot về LMS thất bại, property **Trạng thái đồng bộ** trên Contact = **Đồng bộ thất bại**.

### Các trường thông tin chung

| Trường trên LMS/OPS   | Property trên HubSpot     | Ghi chú                                                                |
| --------------------- | ------------------------- | ---------------------------------------------------------------------- |
| Full Name             | First name                | Có thể đồng bộ hai chiều tùy màn hình thao tác                         |
| Email                 | Email                     | Khi cập nhật từ LMS/OPS lên HubSpot, được cập nhật thành Primary Email |
| Phone                 | Phone number              | Có thể đồng bộ hai chiều                                               |
| D.O.B                 | D.O.B                     | Đồng bộ giữa HubSpot và LMS/OPS                                        |
| Gender                | Gender                    | Tùy cấu hình hiện tại của hệ thống                                     |
| Main Class            | \[TVTS] Lớp đăng ký chính | Chỉ hiển thị, không chỉnh sửa trực tiếp tại Student Profile            |
| Deferred/Retake Class | Lớp bảo lưu/học lại       | Chỉ hiển thị, không chỉnh sửa trực tiếp tại Student Profile            |
| University            | \[TVTS] Trường Đại học    | Đồng bộ giữa HubSpot và LMS/OPS                                        |
| Major                 | \[TVTS] Chuyên ngành học  | Đồng bộ giữa HubSpot và LMS/OPS                                        |
| Field of Work         | \[TVTS] Lĩnh vực Công ty  | Đồng bộ giữa HubSpot và LMS/OPS                                        |
| Position              | \[TVTS] Cấp bậc           | Đồng bộ giữa HubSpot và LMS/OPS                                        |

### Các trường theo chương trình CFA/ACCA/CMA

| Trường trên LMS/OPS | Nguồn đồng bộ     | Ghi chú                                                                                          |
| ------------------- | ----------------- | ------------------------------------------------------------------------------------------------ |
| Level               | Contact           | Đồng bộ theo từng chương trình CFA/ACCA/CMA                                                      |
| Exam                | Contact / LMS/OPS | Kỳ thi thực tế theo từng môn của từng chương trình                                               |
| Result              | Contact / LMS/OPS | Kết quả thi tương ứng với từng môn/kỳ thi                                                        |
| Account ID          | Contact           | Ví dụ ACCA Registration Number, Username CFA, Username CMA; thường chỉ hiển thị, không chỉnh sửa |

### Quy tắc đồng bộ từ HubSpot Contact về LMS/OPS

| Quy tắc                   | Mô tả                                                                                                                            |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| Trigger từng field        | Khi một field được cấu hình đồng bộ trên Contact thay đổi, HubSpot gửi webhook về LMS/OPS.                                       |
| Trigger đồng bộ toàn bộ   | Khi chọn **Trạng thái đồng bộ = Tiến hành đồng bộ** trên Contact, hệ thống đồng bộ lại toàn bộ thông tin trong phạm vi cấu hình. |
| Xác định học viên         | Hệ thống dùng HubSpot Contact ID để tìm học viên tương ứng trên LMS/OPS.                                                         |
| Không tìm thấy Contact ID | Hệ thống kết thúc luồng đồng bộ và không cập nhật dữ liệu.                                                                       |
| Đồng bộ thành công        | Hệ thống cập nhật dữ liệu trên LMS/OPS và cập nhật trạng thái thành công.                                                        |
| Đồng bộ thất bại          | Hệ thống cập nhật trạng thái thất bại và ghi nhận/gửi lỗi để IT kiểm tra.                                                        |

### Quy tắc đồng bộ từ LMS/OPS lên HubSpot Contact

| Quy tắc            | Mô tả                                                                                            |
| ------------------ | ------------------------------------------------------------------------------------------------ |
| Điều kiện đồng bộ  | Học viên cần có HubSpot Contact ID hợp lệ.                                                       |
| Nguồn thay đổi     | Dữ liệu được cập nhật từ Student Profile trên OPS hoặc màn thông tin học viên trên LMS.          |
| Field được đồng bộ | Chỉ các field nằm trong phạm vi cấu hình mới được cập nhật lên HubSpot.                          |
| Email              | Khi đồng bộ từ LMS/OPS lên HubSpot, Email được cập nhật thành Primary Email.                     |
| Lỗi HubSpot        | Nếu cập nhật HubSpot thất bại, hệ thống gửi thông báo lỗi cho IT.                                |
| Dữ liệu LMS/OPS    | Dữ liệu đã lưu trên LMS/OPS không nhất thiết bị rollback nếu lỗi xảy ra khi đồng bộ lên HubSpot. |

### Quy tắc kỳ thi và kết quả thi

| Trường hợp                       | Quy tắc                                                            |
| -------------------------------- | ------------------------------------------------------------------ |
| Exam chưa phải kỳ thi chính thức | Có thể chỉnh sửa nếu người dùng có quyền.                          |
| Exam đã là kỳ thi chính thức     | Không được chỉnh sửa, hệ thống hiển thị tag **Registered** nếu có. |
| Đổi Exam                         | Result tương ứng có thể được đưa về rỗng theo logic hệ thống.      |
| Có Result nhưng chưa có Exam     | Khi thêm Exam lần đầu, Result có thể được giữ nguyên.              |
| Đổi Exam lần tiếp theo           | Result tương ứng được đưa về rỗng.                                 |
| Chỉ đổi Result                   | Không tác động đến thông tin Exam.                                 |

### Quy tắc merge Contact từ HubSpot về LMS

| Trường hợp                             | Quy tắc                                                                                    |
| -------------------------------------- | ------------------------------------------------------------------------------------------ |
| HubSpot merge Contact                  | HubSpot gửi webhook sang LMS để xử lý merge user tương ứng.                                |
| Một trong hai Contact có user trên LMS | Hệ thống lấy user đang tồn tại trên LMS làm cơ sở xử lý và đồng bộ lại dữ liệu.            |
| Cả hai Contact không có user trên LMS  | Hệ thống kết thúc luồng merge, không xử lý thêm.                                           |
| Nhiều user cùng Contact ID             | Hệ thống chọn user chính theo thứ tự ưu tiên.                                              |
| User đã tồn tại trong lớp              | User có lớp được ưu tiên làm user chính; user khác có lớp có thể không được merge tự động. |
| User không tồn tại trong lớp           | Có thể được merge vào user chính nếu đủ điều kiện.                                         |
| Lịch sử merge                          | Hệ thống ghi nhận log merge để phục vụ kiểm tra sau này.                                   |

### Mẹo sử dụng

1. Khi cần cập nhật dữ liệu học viên từ HubSpot về LMS/OPS ngay, nên dùng property **Trạng thái đồng bộ = Tiến hành đồng bộ** trên Contact.
2. Trước khi chạy đồng bộ thủ công, nên kiểm tra các thông tin quan trọng trên Contact (email, số điện thoại, ngày sinh, trường, chuyên ngành, kỳ thi).
3. Với các trường danh mục (University, Major, Field of Work, Position), nên chọn đúng giá trị đã có trong hệ thống để tránh lỗi mapping.
4. Khi chỉnh sửa thông tin trên OPS, nên kiểm tra học viên có HubSpot Contact ID hay chưa để đảm bảo đồng bộ được lên HubSpot.
5. Với thông tin kỳ thi/kết quả thi, cần kiểm tra kỹ trước khi đổi Exam vì Result có thể bị reset.
6. Khi thấy dữ liệu LMS và HubSpot lệch nhau, nên kiểm tra lần cập nhật gần nhất và trạng thái đồng bộ trước khi báo lỗi.
7. Với trường hợp merge Contact, nên hạn chế thao tác thủ công song song trên LMS trong khi hệ thống đang xử lý merge.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                             | Nguyên nhân                                                                         | Cách xử lý                                           |
| -------------------------------------------- | ----------------------------------------------------------------------------------- | ---------------------------------------------------- |
| Contact cập nhật nhưng LMS không đổi         | HubSpot Contact ID không tồn tại trên LMS hoặc field chưa nằm trong phạm vi đồng bộ | Kiểm tra Contact ID và field mapping                 |
| Chọn Tiến hành đồng bộ nhưng thất bại        | Dữ liệu Contact lỗi, thiếu mapping hoặc lỗi hệ thống                                | Kiểm tra lại dữ liệu Contact và liên hệ IT           |
| Thông tin trên OPS không đồng bộ lên HubSpot | Học viên chưa có HubSpot Contact ID hoặc lỗi cập nhật HubSpot                       | Kiểm tra Contact ID và báo IT nếu cần                |
| Email không cập nhật đúng trên HubSpot       | Email trùng, không hợp lệ hoặc xung đột với Contact/User khác                       | Kiểm tra email chính/phụ trên HubSpot và LMS         |
| Không chỉnh sửa được Main Class              | Trường Main Class chỉ hiển thị, không chỉnh sửa trực tiếp tại Student Profile       | Cập nhật thông tin lớp theo đúng nghiệp vụ liên quan |
| Không chỉnh sửa được Deferred/Retake Class   | Trường này chỉ hiển thị, không chỉnh sửa trực tiếp                                  | Kiểm tra nghiệp vụ bảo lưu/học lại tương ứng         |
| Đổi Exam làm mất Result                      | Theo rule hệ thống, Result có thể reset khi thay đổi Exam                           | Kiểm tra lại kỳ thi và nhập/cập nhật Result nếu cần  |
| Merge Contact nhưng LMS không merge user     | Không đủ điều kiện merge hoặc cả hai Contact không có user LMS                      | Liên hệ IT kiểm tra merge log                        |
| Dữ liệu enum không hiển thị đúng             | Giá trị từ HubSpot chưa có mapping tương ứng trên LMS/OPS                           | Báo Admin/IT kiểm tra danh mục mapping               |
