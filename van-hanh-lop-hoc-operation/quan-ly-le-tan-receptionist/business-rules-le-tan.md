# Business Rules — Lễ tân

### 1. Quy tắc chung

| Mã rule    | Business Rule                                                                                                 |
| ---------- | ------------------------------------------------------------------------------------------------------------- |
| BR-REC-001 | Người dùng chỉ được truy cập module **Receptionist** khi đã đăng nhập thành công vào hệ thống LMS Operations. |
| BR-REC-002 | Người dùng chỉ được xem, đăng ký, chỉnh sửa lịch trực hoặc xử lý đơn nếu tài khoản có quyền tương ứng.        |
| BR-REC-003 | Module Receptionist bao gồm các nhóm chức năng chính: **Receptionist Shift** và **Receptionist Request**.     |
| BR-REC-004 | Dữ liệu lịch trực được quản lý theo **Facility**, **Date**, **Shift** và **On-call person**.                  |
| BR-REC-005 | Lịch trực có liên quan đến lịch sử dụng phòng học, lịch lớp học, lịch thuê phòng và cơ sở học.                |
| BR-REC-006 | Nút **Reset** tại các màn hình chỉ làm mới/xóa điều kiện tìm kiếm, không xóa dữ liệu lịch trực hoặc đề xuất.  |

***

### 2. Quy tắc xem danh sách lịch trực

| Mã rule           | Business Rule                                                                                                                         |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| BR-SHIFT-VIEW-001 | Người dùng phải có quyền xem lịch trực mới được truy cập màn hình **Receptionist Shift**.                                             |
| BR-SHIFT-VIEW-002 | Người dùng truy cập danh sách lịch trực tại **Customer Experience → Receptionist → Receptionist Shift**.                              |
| BR-SHIFT-VIEW-003 | Khi tìm kiếm lịch trực, trường **Facility** là bắt buộc.                                                                              |
| BR-SHIFT-VIEW-004 | Khi tìm kiếm lịch trực, trường **Start date - End date** là bắt buộc.                                                                 |
| BR-SHIFT-VIEW-005 | Trường **On-call person** không bắt buộc; dùng để lọc lịch trực theo một Lễ tân cụ thể.                                               |
| BR-SHIFT-VIEW-006 | Nếu nhân viên có gắn Facility, hệ thống mặc định hiển thị Facility đầu tiên của nhân viên tại bộ lọc.                                 |
| BR-SHIFT-VIEW-007 | Danh sách lịch trực hiển thị các thông tin: Date, Shift, On-call person, Room holder, Section, Teacher, Classroom, Attendant và Note. |
| BR-SHIFT-VIEW-008 | Nếu ca trực chưa đủ người trực, cột **On-call person** hiển thị “-------------” tương ứng với số lượng Lễ tân còn thiếu.              |
| BR-SHIFT-VIEW-009 | Thông tin **Attendant** và **Note** được cập nhật tại chức năng chỉnh sửa lịch trực.                                                  |
| BR-SHIFT-VIEW-010 | Kết quả lịch trực của tháng tiếp theo được hệ thống cập nhật vào ngày **21 hàng tháng**.                                              |

***

### 3. Quy tắc hiển thị ca trực theo loại Lễ tân

| Mã rule              | Business Rule                                                                                                                                    |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| BR-SHIFT-DISPLAY-001 | Với tài khoản **Receptionist Full-time**, hệ thống hiển thị toàn bộ ca sáng, chiều, tối từ thứ hai đến Chủ nhật.                                 |
| BR-SHIFT-DISPLAY-002 | Với tài khoản **Receptionist Part-time**, từ thứ hai đến thứ sáu hệ thống mặc định chỉ hiển thị ca tối.                                          |
| BR-SHIFT-DISPLAY-003 | Với tài khoản **Receptionist Part-time**, thứ bảy và Chủ nhật hệ thống hiển thị cả ba ca sáng, chiều, tối.                                       |
| BR-SHIFT-DISPLAY-004 | Với ca sáng và ca chiều từ thứ hai đến thứ sáu, hệ thống chỉ hiển thị cho Receptionist Part-time nếu người đó đã được gắn với ca trực tương ứng. |

***

### 4. Quy tắc đăng ký ca trực của Lễ tân Part-time

| Mã rule          | Business Rule                                                                                           |
| ---------------- | ------------------------------------------------------------------------------------------------------- |
| BR-SHIFT-REG-001 | Chức năng **Register Shift** chỉ áp dụng cho tài khoản **Receptionist Part-time**.                      |
| BR-SHIFT-REG-002 | Người dùng phải có quyền đăng ký ca trực mới nhìn thấy hoặc sử dụng được nút **Register Shift**.        |
| BR-SHIFT-REG-003 | Theo logic hiện tại, Receptionist Part-time được đăng ký ca trực từ ngày **01 đến ngày 15** hàng tháng. |
| BR-SHIFT-REG-004 | Theo logic hiện tại, Receptionist Part-time được đăng ký ca trực vào ngày **25 và ngày 26** hàng tháng. |
| BR-SHIFT-REG-005 | Ngoài các ngày **01–15** và **25–26** hàng tháng, hệ thống không hiển thị nút **Register Shift**.       |
| BR-SHIFT-REG-006 | Màn hình Register Shift hiển thị lịch trực theo tuần, từ thứ hai đến Chủ nhật.                          |
| BR-SHIFT-REG-007 | Người dùng có thể lọc lịch trực theo **Facility** khi đăng ký ca trực.                                  |
| BR-SHIFT-REG-008 | Người dùng có thể dùng nút mũi tên trái/phải để chuyển tuần đăng ký.                                    |
| BR-SHIFT-REG-009 | Người dùng tick checkbox để đăng ký ca trực.                                                            |
| BR-SHIFT-REG-010 | Người dùng bỏ tick checkbox để hủy đăng ký ca trực đã chọn.                                             |
| BR-SHIFT-REG-011 | Các ca đã đăng ký thành công trước đó hiển thị checkbox đã được tick.                                   |
| BR-SHIFT-REG-012 | Người dùng phải chọn **Save** để lưu thay đổi đăng ký ca trực.                                          |
| BR-SHIFT-REG-013 | Nếu người dùng chọn **Cancel** và xác nhận thoát, các thay đổi chưa lưu sẽ không được ghi nhận.         |

***

### 5. Quy tắc số lượng ca đăng ký của Lễ tân Part-time

| Mã rule              | Business Rule                                                                                                                                                                                |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BR-SHIFT-REG-QTY-001 | Receptionist Part-time cần đăng ký tối thiểu **04 ca/tuần**.                                                                                                                                 |
| BR-SHIFT-REG-QTY-002 | Receptionist Part-time không được đăng ký vượt quá số ca tối đa theo tuần do hệ thống tính toán.                                                                                             |
| BR-SHIFT-REG-QTY-003 | Số ca đăng ký tối đa/tuần = `(Tổng số người trực cần có của tuần - Số ca trực Receptionist Full-time đã đăng ký) / Số lượng Receptionist Part-time của cơ sở`, làm tròn lên đến hàng đơn vị. |
| BR-SHIFT-REG-QTY-004 | Nếu Receptionist Part-time chưa đăng ký đủ số ca tối thiểu khi chọn Save, hệ thống hiển thị popup: **“Bạn chưa đăng ký đủ số lượng ca tối thiểu. Bạn có chắc chắn lưu đăng ký không?”**      |
| BR-SHIFT-REG-QTY-005 | Nếu người dùng chọn **Yes** tại popup chưa đủ số ca tối thiểu, hệ thống vẫn lưu thông tin đăng ký.                                                                                           |
| BR-SHIFT-REG-QTY-006 | Nếu người dùng chọn **No** tại popup chưa đủ số ca tối thiểu, hệ thống quay lại màn hình đăng ký ca trực.                                                                                    |

***

### 6. Quy tắc chỉnh sửa lịch trực

| Mã rule           | Business Rule                                                                                                                             |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| BR-SHIFT-EDIT-001 | Người dùng phải có quyền chỉnh sửa lịch trực mới được sử dụng chức năng **Edit Receptionist Shift**.                                      |
| BR-SHIFT-EDIT-002 | Người dùng chọn **Action → Edit** tại ca trực cần chỉnh sửa để mở màn hình chỉnh sửa lịch trực.                                           |
| BR-SHIFT-EDIT-003 | Trường **Date** không được phép chỉnh sửa.                                                                                                |
| BR-SHIFT-EDIT-004 | Trường **Shift** không được phép chỉnh sửa.                                                                                               |
| BR-SHIFT-EDIT-005 | Trường **Room Holder** không được phép chỉnh sửa.                                                                                         |
| BR-SHIFT-EDIT-006 | Trường **Attendant** được phép chỉnh sửa để cập nhật số lượng học viên thực tế.                                                           |
| BR-SHIFT-EDIT-007 | Trường **Note** được phép chỉnh sửa để ghi nhận thông tin phát sinh trong ca trực.                                                        |
| BR-SHIFT-EDIT-008 | Trường **On-call Person** được chỉnh sửa theo quyền và loại tài khoản người dùng.                                                         |
| BR-SHIFT-EDIT-009 | Tài khoản **Receptionist Full-time** được phép chỉnh sửa tất cả các ca trực theo phạm vi được phân quyền.                                 |
| BR-SHIFT-EDIT-010 | Tài khoản **Receptionist Full-time** được phép chỉnh sửa trường **On-call Person**.                                                       |
| BR-SHIFT-EDIT-011 | Tài khoản **Receptionist Full-time** được phép gán Receptionist Part-time vào ca trực kể cả khi Part-time đã đạt số lượng ca trực tối đa. |
| BR-SHIFT-EDIT-012 | Tài khoản **Receptionist Part-time** chỉ được chỉnh sửa các ca trực có chính họ trong danh sách người trực.                               |
| BR-SHIFT-EDIT-013 | Tài khoản **Receptionist Part-time** không được chỉnh sửa trường **On-call Person**.                                                      |
| BR-SHIFT-EDIT-014 | Khi chọn quá số lượng Lễ tân cần có trong một ca, hệ thống hiển thị cảnh báo **“Too many receptionists scheduled for this shift.”**       |
| BR-SHIFT-EDIT-015 | Sau khi hiển thị cảnh báo vượt số lượng Lễ tân, hệ thống vẫn cho phép lưu.                                                                |
| BR-SHIFT-EDIT-016 | Người dùng chọn **Save** để lưu thông tin chỉnh sửa và quay lại màn danh sách lịch trực.                                                  |
| BR-SHIFT-EDIT-017 | Người dùng chọn **Cancel** để hủy thao tác chỉnh sửa; hệ thống hiển thị popup xác nhận trước khi thoát.                                   |

***

### 7. Quy tắc số lượng Lễ tân cần có trong một ca

| Mã rule            | Facility      |  Số phòng trong ca | Số lượng Lễ tân cần có |
| ------------------ | ------------- | -----------------: | ---------------------: |
| BR-SHIFT-STAFF-001 | NEU           |        1 - 2 phòng |               1 Lễ tân |
| BR-SHIFT-STAFF-002 | NEU           |        3 - 4 phòng |               2 Lễ tân |
| BR-SHIFT-STAFF-003 | NEU           |        5 - 6 phòng |               3 Lễ tân |
| BR-SHIFT-STAFF-004 | Facility khác |        1 - 2 phòng |               1 Lễ tân |
| BR-SHIFT-STAFF-005 | Facility khác | Từ 3 phòng trở lên |               2 Lễ tân |

***

### 8. Quy tắc xem danh sách Receptionist Request

| Mã rule         | Business Rule                                                                                                                                                |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BR-REQ-VIEW-001 | Người dùng phải có quyền xem đề xuất của Lễ tân mới được truy cập màn hình **Receptionist Request**.                                                         |
| BR-REQ-VIEW-002 | Người dùng truy cập danh sách đề xuất tại **Customer Experience → Receptionist → Receptionist Request**.                                                     |
| BR-REQ-VIEW-003 | Người dùng chỉ xem được đề xuất nếu là **người tạo đề xuất**, **người duyệt đề xuất** hoặc **người thay thế/Substitute** trong đề xuất.                      |
| BR-REQ-VIEW-004 | Danh sách đề xuất hiển thị các thông tin: Request name, Request type, Status, Receptionist, Facility, Shift, Reason, Substitute, Create date và Update date. |
| BR-REQ-VIEW-005 | Người dùng có thể tìm kiếm đề xuất theo Request name, Request type, Status và khoảng thời gian tạo.                                                          |
| BR-REQ-VIEW-006 | Người dùng có thể xem chi tiết đề xuất bằng cách nhấp vào **Request Name** hoặc chọn **Action → View**.                                                      |

***

### 9. Quy tắc trạng thái Receptionist Request

| Mã rule           | Trạng thái | Business Rule                                                           |
| ----------------- | ---------- | ----------------------------------------------------------------------- |
| BR-REQ-STATUS-001 | Pending    | Đề xuất đang chờ Facility Manager duyệt.                                |
| BR-REQ-STATUS-002 | Approved   | Đề xuất đã được Facility Manager chấp thuận.                            |
| BR-REQ-STATUS-003 | Rejected   | Đề xuất đã bị Facility Manager từ chối.                                 |
| BR-REQ-STATUS-004 | Cancelled  | Đề xuất đã được duyệt trước đó nhưng sau đó bị hủy.                     |
| BR-REQ-STATUS-005 | Pending    | Có thể chỉnh sửa hoặc xóa nếu người dùng là người tạo đề xuất.          |
| BR-REQ-STATUS-006 | Approved   | Có thể hủy bằng cách chuyển trạng thái sang Cancelled nếu đủ điều kiện. |
| BR-REQ-STATUS-007 | Rejected   | Không được chỉnh sửa, hủy hoặc xóa.                                     |
| BR-REQ-STATUS-008 | Cancelled  | Không được tiếp tục xử lý.                                              |

***

### 10. Quy tắc tạo Receptionist Request

| Mã rule           | Business Rule                                                                                 |
| ----------------- | --------------------------------------------------------------------------------------------- |
| BR-REQ-CREATE-001 | Chức năng tạo đề xuất chỉ áp dụng cho tài khoản có **Job Title = Receptionist Part-time**.    |
| BR-REQ-CREATE-002 | Người dùng phải có quyền tạo đề xuất mới được sử dụng nút **Create Request**.                 |
| BR-REQ-CREATE-003 | Có 2 loại đề xuất: **Timeoff** và **Shift Change**.                                           |
| BR-REQ-CREATE-004 | Sau khi tạo thành công, đề xuất có trạng thái mặc định là **Pending**.                        |
| BR-REQ-CREATE-005 | Người duyệt đề xuất là **Facility Manager** của Facility được chọn trong đề xuất.             |
| BR-REQ-CREATE-006 | Người dùng được tạo tối đa **03 request cùng loại trong 01 tháng**.                           |
| BR-REQ-CREATE-007 | Sau khi tạo đề xuất thành công, hệ thống gửi email thông báo cho Facility Manager.            |
| BR-REQ-CREATE-008 | Nếu đề xuất có chọn Substitute, hệ thống gửi email thông báo cho người thay thế/người đổi ca. |
| BR-REQ-CREATE-009 | Tài liệu đính kèm là không bắt buộc.                                                          |
| BR-REQ-CREATE-010 | Mỗi đề xuất được upload tối đa **03 file**.                                                   |
| BR-REQ-CREATE-011 | Dung lượng mỗi file đính kèm tối đa **10MB**.                                                 |
| BR-REQ-CREATE-012 | Định dạng file được hỗ trợ gồm **pdf, jpg, png, doc, docx**.                                  |

***

### 11. Quy tắc tạo đề xuất Timeoff

| Mã rule            | Business Rule                                                                   |
| ------------------ | ------------------------------------------------------------------------------- |
| BR-REQ-TIMEOFF-001 | Khi tạo Timeoff, trường **Request Name** là bắt buộc.                           |
| BR-REQ-TIMEOFF-002 | Khi tạo Timeoff, trường **Request Type** là bắt buộc và có giá trị **Timeoff**. |
| BR-REQ-TIMEOFF-003 | Khi tạo Timeoff, trường **Facility** là bắt buộc.                               |
| BR-REQ-TIMEOFF-004 | Khi tạo Timeoff, trường **Shift** là bắt buộc.                                  |
| BR-REQ-TIMEOFF-005 | Danh sách Shift chỉ hiển thị các ca trực của người tạo tại Facility đã chọn.    |
| BR-REQ-TIMEOFF-006 | Trường **Substitute** không bắt buộc đối với đề xuất Timeoff.                   |
| BR-REQ-TIMEOFF-007 | Trường **Reason** là bắt buộc.                                                  |
| BR-REQ-TIMEOFF-008 | Người dùng có thể chọn **Add Timeoff** để thêm ca xin nghỉ trong cùng đề xuất.  |
| BR-REQ-TIMEOFF-009 | Một đề xuất Timeoff được thêm tối đa **02 khoảng thời gian/ca xin nghỉ**.       |
| BR-REQ-TIMEOFF-010 | Người dùng có thể chọn **Delete Timeoff** để xóa ca xin nghỉ đã thêm.           |

***

### 12. Quy tắc tạo đề xuất Shift Change

| Mã rule       | Business Rule                                                                                            |
| ------------- | -------------------------------------------------------------------------------------------------------- |
| BR-REQ-SC-001 | Khi tạo Shift Change, trường **Request Name** là bắt buộc.                                               |
| BR-REQ-SC-002 | Khi tạo Shift Change, trường **Request Type** là bắt buộc và có giá trị **Shift Change**.                |
| BR-REQ-SC-003 | Khi tạo Shift Change, trường **Facility** là bắt buộc.                                                   |
| BR-REQ-SC-004 | Khi tạo Shift Change, trường **Shift** là bắt buộc và là ca trực gốc của người tạo tại Facility đã chọn. |
| BR-REQ-SC-005 | Khi tạo Shift Change, trường **Substitute Shift** là bắt buộc.                                           |
| BR-REQ-SC-006 | Substitute Shift là ca trực mà người tạo muốn đổi sang.                                                  |
| BR-REQ-SC-007 | Khi tạo Shift Change, trường **Substitute** là bắt buộc.                                                 |
| BR-REQ-SC-008 | Substitute là người đang trực tại Substitute Shift đã chọn.                                              |
| BR-REQ-SC-009 | Substitute chỉ có thể là **Receptionist Part-time**.                                                     |
| BR-REQ-SC-010 | Trường **Reason** là bắt buộc.                                                                           |

***

### 13. Quy tắc chỉnh sửa Receptionist Request

| Mã rule         | Business Rule                                                                                                                             |
| --------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| BR-REQ-EDIT-001 | Người dùng phải có quyền chỉnh sửa đề xuất mới được chỉnh sửa Receptionist Request.                                                       |
| BR-REQ-EDIT-002 | Người dùng chỉ được chỉnh sửa đề xuất do chính mình tạo.                                                                                  |
| BR-REQ-EDIT-003 | Chỉ đề xuất có trạng thái **Pending** mới được chỉnh sửa nội dung.                                                                        |
| BR-REQ-EDIT-004 | Với Timeoff Pending, người dùng được chỉnh sửa Request Name, Shift, Substitute, Reason, Attached Document, Add Timeoff và Delete Timeoff. |
| BR-REQ-EDIT-005 | Với Shift Change Pending, người dùng được chỉnh sửa Request Name, Shift, Substitute Shift, Substitute, Reason và Attached Document.       |
| BR-REQ-EDIT-006 | Đề xuất Approved không được chỉnh sửa nội dung đề xuất.                                                                                   |
| BR-REQ-EDIT-007 | Với đề xuất Approved, người tạo chỉ có thể hủy bằng cách chuyển trạng thái sang **Cancelled** nếu đủ điều kiện.                           |
| BR-REQ-EDIT-008 | Đề xuất Rejected hoặc Cancelled không được chỉnh sửa.                                                                                     |

***

### 14. Quy tắc hủy Receptionist Request đã duyệt

| Mã rule           | Business Rule                                                                                                                                                         |
| ----------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BR-REQ-CANCEL-001 | Chỉ đề xuất có trạng thái **Approved** mới có thể chuyển sang **Cancelled**.                                                                                          |
| BR-REQ-CANCEL-002 | Chỉ người tạo đề xuất mới được hủy đề xuất đã duyệt nếu có quyền.                                                                                                     |
| BR-REQ-CANCEL-003 | Khi người dùng chuyển trạng thái Approved sang Cancelled, hệ thống hiển thị popup xác nhận.                                                                           |
| BR-REQ-CANCEL-004 | Nếu người dùng chọn **Yes**, hệ thống chuyển trạng thái đề xuất từ **Approved** sang **Cancelled**.                                                                   |
| BR-REQ-CANCEL-005 | Nếu người dùng chọn **No**, hệ thống giữ nguyên trạng thái Approved.                                                                                                  |
| BR-REQ-CANCEL-006 | Với request Timeoff, nếu ca trực trong đề xuất vẫn trống Lễ tân, hệ thống điền lại tên Lễ tân đã hủy đề xuất vào ca trực.                                             |
| BR-REQ-CANCEL-007 | Với request Timeoff, nếu ca trực trong đề xuất đã được gắn với Lễ tân khác, hệ thống giữ nguyên thông tin Lễ tân hiện tại.                                            |
| BR-REQ-CANCEL-008 | Với request Timeoff, nếu tất cả ca trực trong đề xuất đều đã có Lễ tân thay thế, hệ thống không cho phép hủy và hiển thị lỗi **“Các ca trực đã có lễ tân thay thế”**. |
| BR-REQ-CANCEL-009 | Với request Shift Change, hệ thống đổi ngược lại ca trực, Lễ tân trực đúng ca như ban đầu trước khi đề xuất được duyệt.                                               |

***

### 15. Quy tắc xóa Receptionist Request

| Mã rule           | Business Rule                                                                         |
| ----------------- | ------------------------------------------------------------------------------------- |
| BR-REQ-DELETE-001 | Người dùng phải có quyền xóa đề xuất mới được xóa Receptionist Request.               |
| BR-REQ-DELETE-002 | Người dùng chỉ được xóa đề xuất do chính mình tạo.                                    |
| BR-REQ-DELETE-003 | Chỉ đề xuất có trạng thái **Pending** mới được phép xóa.                              |
| BR-REQ-DELETE-004 | Khi xóa đề xuất, hệ thống hiển thị popup xác nhận.                                    |
| BR-REQ-DELETE-005 | Nếu người dùng chọn **Yes**, hệ thống xóa đề xuất khỏi danh sách.                     |
| BR-REQ-DELETE-006 | Nếu người dùng chọn **No**, hệ thống hủy thao tác xóa và giữ nguyên đề xuất.          |
| BR-REQ-DELETE-007 | Sau khi xóa đề xuất thành công, hệ thống gửi email thông báo cho người duyệt đề xuất. |

***

### 16. Quy tắc duyệt / từ chối Receptionist Request

| Mã rule            | Business Rule                                                                                       |
| ------------------ | --------------------------------------------------------------------------------------------------- |
| BR-REQ-APPROVE-001 | Người dùng phải có quyền duyệt/từ chối đề xuất mới được sử dụng nút **Approve** hoặc **Reject**.    |
| BR-REQ-APPROVE-002 | Người duyệt phải là **Facility Manager** của Facility diễn ra ca trực trong đề xuất.                |
| BR-REQ-APPROVE-003 | Chỉ đề xuất có trạng thái **Pending** mới được duyệt hoặc từ chối.                                  |
| BR-REQ-APPROVE-004 | Khi Facility Manager chọn **Approve**, hệ thống chuyển trạng thái đề xuất từ Pending sang Approved. |
| BR-REQ-APPROVE-005 | Khi Facility Manager chọn **Reject**, hệ thống chuyển trạng thái đề xuất từ Pending sang Rejected.  |
| BR-REQ-APPROVE-006 | Sau khi đề xuất được duyệt hoặc từ chối, hệ thống gửi email thông báo cho người tạo đề xuất.        |
| BR-REQ-APPROVE-007 | Với đề xuất bị từ chối, hệ thống không thay đổi lịch trực hiện tại.                                 |
| BR-REQ-APPROVE-008 | Đề xuất Approved, Rejected hoặc Cancelled không thể duyệt/từ chối lại.                              |

***

### 17. Quy tắc tác động đến lịch trực khi duyệt đề xuất

| Mã rule           | Loại đề xuất | Business Rule                                                                                                      |
| ----------------- | ------------ | ------------------------------------------------------------------------------------------------------------------ |
| BR-REQ-IMPACT-001 | Timeoff      | Nếu Timeoff có Substitute, hệ thống cập nhật người thay thế vào ca trực tương ứng sau khi đề xuất được duyệt.      |
| BR-REQ-IMPACT-002 | Timeoff      | Nếu Timeoff không có Substitute, hệ thống ghi nhận người tạo đề xuất nghỉ ca; ca trực có thể còn thiếu người trực. |
| BR-REQ-IMPACT-003 | Shift Change | Sau khi Shift Change được duyệt, hệ thống đổi ca giữa người tạo đề xuất và Substitute.                             |
| BR-REQ-IMPACT-004 | Shift Change | Người thay thế nhận ca trực gốc của người tạo đề xuất.                                                             |
| BR-REQ-IMPACT-005 | Shift Change | Người tạo đề xuất nhận ca trực muốn chuyển sang.                                                                   |
| BR-REQ-IMPACT-006 | Rejected     | Nếu đề xuất bị từ chối, lịch trực không thay đổi.                                                                  |

***

### 18. Quy tắc thông báo

| Mã rule         | Business Rule                                                                                                  |
| --------------- | -------------------------------------------------------------------------------------------------------------- |
| BR-REC-NOTI-001 | Hệ thống gửi email cho Receptionist Part-time khi mở đợt đăng ký ca trực nếu có cấu hình thông báo.            |
| BR-REC-NOTI-002 | Hệ thống gửi email nhắc Receptionist Part-time khi gần kết thúc đợt đăng ký ca trực nếu có cấu hình thông báo. |
| BR-REC-NOTI-003 | Hệ thống gửi email cho Facility Manager để kiểm tra lịch trực theo lịch cấu hình.                              |
| BR-REC-NOTI-004 | Khi Receptionist Request được tạo thành công, hệ thống gửi email cho Facility Manager.                         |
| BR-REC-NOTI-005 | Khi Receptionist Request có Substitute, hệ thống gửi email cho Substitute.                                     |
| BR-REC-NOTI-006 | Khi Receptionist Request bị xóa, hệ thống gửi email thông báo cho người duyệt.                                 |
| BR-REC-NOTI-007 | Khi Receptionist Request được duyệt hoặc từ chối, hệ thống gửi email thông báo cho người tạo đề xuất.          |

***
