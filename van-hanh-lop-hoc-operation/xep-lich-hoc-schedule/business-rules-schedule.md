---
description: >-
  (Quy tắc check trùng lịch phòng; logic tự động theo Learning Schedule; điều
  kiện hiển thị phòng học)
---

# Business Rules — Schedule

***

<details>

<summary>Quy tắc check trùng lịch phòng</summary>

| Mã rule                  | Business Rule                                                                                                                                                            |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| BR-SCH-ROOM-CONFLICT-001 | Khi người dùng chọn phòng học cho một buổi học, hệ thống phải kiểm tra lịch sử dụng phòng trong cùng khoảng thời gian của buổi học đó.                                   |
| BR-SCH-ROOM-CONFLICT-002 | Với buổi học được tạo **thủ công**, hệ thống chỉ hiển thị các phòng **không trùng lịch** với buổi học đang tạo/chỉnh sửa.                                                |
| BR-SCH-ROOM-CONFLICT-003 | Với lớp đã được **xếp lịch tự động**, khi thêm phòng học cho toàn bộ lịch lớp, hệ thống cho phép hiển thị các phòng có số buổi trùng lịch nhỏ hơn hoặc bằng **03 buổi**. |
| BR-SCH-ROOM-CONFLICT-004 | Với lịch tự động, danh sách phòng học được sắp xếp theo số lượng buổi trùng lịch từ **ít nhất đến nhiều nhất**.                                                          |
| BR-SCH-ROOM-CONFLICT-005 | Nếu phòng học bị trùng lịch vượt quá số buổi cho phép, phòng học đó không được hiển thị trong danh sách chọn.                                                            |
| BR-SCH-ROOM-CONFLICT-006 | Nếu không có phòng học nào thỏa mãn điều kiện, hệ thống hiển thị thông báo **No matching records found.**                                                                |
| BR-SCH-ROOM-CONFLICT-007 | Khi chỉnh sửa Classroom của một buổi học, hệ thống phải kiểm tra lại điều kiện trùng lịch phòng theo **Lesson Date**, **Start Time** và **End Time** mới.                |
| BR-SCH-ROOM-CONFLICT-008 | Nếu người dùng thay đổi ngày học hoặc khung giờ học, danh sách phòng học cần được tính toán lại theo lịch mới.                                                           |
| BR-SCH-ROOM-CONFLICT-009 | Khi buổi học bị hủy, hệ thống ẩn hoặc giải phóng lịch phòng học tương ứng để các buổi học khác có thể được xếp vào thời gian đó.                                         |
| BR-SCH-ROOM-CONFLICT-010 | Khi buổi học bị xóa, hệ thống xóa lịch phòng học gắn với buổi học đó.                                                                                                    |

</details>

<details>

<summary>Logic tự động theo Learning Schedule</summary>

| Mã rule         | Business Rule                                                                                                                                                                           |
| --------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BR-SCH-AUTO-001 | Hệ thống chỉ cho phép xếp lịch học tự động khi Course của lớp đã có **Learning Schedule**.                                                                                              |
| BR-SCH-AUTO-002 | Learning Schedule là dữ liệu đầu vào để hệ thống xác định danh sách buổi học cần tạo cho lớp.                                                                                           |
| BR-SCH-AUTO-003 | Mỗi buổi học trong Learning Schedule sẽ được hệ thống chuyển thành một buổi học trên Class Calendar khi người dùng chọn **Generate Schedule**.                                          |
| BR-SCH-AUTO-004 | Hệ thống tạo lịch tự động dựa trên các thông tin: **Learning Schedule**, **Start Date**, **Standard Schedule** và **Holiday Schedule**.                                                 |
| BR-SCH-AUTO-005 | Với các buổi học **Offline/Live Online**, hệ thống tự động xếp lịch liên tiếp theo Standard Schedule đã cấu hình.                                                                       |
| BR-SCH-AUTO-006 | Lịch học tự động không được xếp trùng với ngày nghỉ lễ.                                                                                                                                 |
| BR-SCH-AUTO-007 | Nếu ngày học dự kiến trùng với ngày nghỉ lễ, hệ thống tự động lùi buổi học sang ngày học tiếp theo theo Standard Schedule.                                                              |
| BR-SCH-AUTO-008 | Với buổi học **Online LMS** không chứa Midterm/Final Test, hệ thống tự động xếp ngay sau buổi Offline/Live Online liền trước.                                                           |
| BR-SCH-AUTO-009 | Deadline của buổi Online LMS được hệ thống tự động đặt trước buổi học tiếp theo, đồng thời bỏ qua buổi Test nếu có.                                                                     |
| BR-SCH-AUTO-010 | Nếu không có ngày trống để xếp buổi Online LMS do hai buổi Offline/Live Online quá gần nhau, hệ thống tự động lùi buổi Offline/Live Online phía sau để chèn buổi Online LMS vào lịch.   |
| BR-SCH-AUTO-011 | Với buổi Test Online chỉ gồm **Midterm/Final Test**, hệ thống tự động xếp ngay sau buổi Offline hoặc Online trước đó.                                                                   |
| BR-SCH-AUTO-012 | Khi người dùng chỉnh sửa một buổi học tự động và không tick **Don’t Reschedule**, hệ thống tự động sắp xếp lại các buổi học phía sau theo logic Learning Schedule và Standard Schedule. |
| BR-SCH-AUTO-013 | Khi người dùng tick **Don’t Reschedule**, hệ thống không sắp xếp lại toàn bộ lịch lớp và chuyển buổi học đó từ lịch tự động sang lịch thủ công nếu người dùng xác nhận.                 |
| BR-SCH-AUTO-014 | Sau khi một buổi học tự động được chuyển thành lịch thủ công, các lần chỉnh sửa sau của buổi học đó áp dụng theo rule của lịch thủ công.                                                |

</details>

<details>

<summary>Điều kiện hiển thị phòng học</summary>

| Mã rule                 | Business Rule                                                                                                                                                              |
| ----------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BR-SCH-ROOM-DISPLAY-001 | Hệ thống chỉ hiển thị phòng học khi người dùng đã có đủ thông tin ngày học và khung giờ học cần xếp.                                                                       |
| BR-SCH-ROOM-DISPLAY-002 | Với buổi học có Learning Mode = **Live Online**, hệ thống chỉ hiển thị phòng học có **Mode = Virtual**.                                                                    |
| BR-SCH-ROOM-DISPLAY-003 | Với buổi học có Learning Mode = **Offline**, hệ thống chỉ hiển thị phòng học có **Mode = Physical**.                                                                       |
| BR-SCH-ROOM-DISPLAY-004 | Với lớp có Construction Mode = **Offline/Blended**, phòng học vật lý phải thuộc **Facility** của lớp.                                                                      |
| BR-SCH-ROOM-DISPLAY-005 | Hệ thống chỉ hiển thị các phòng học có **Status = Active**.                                                                                                                |
| BR-SCH-ROOM-DISPLAY-006 | Với phòng học vật lý, sức chứa phòng học phải lớn hơn hoặc bằng số lượng học viên của lớp.                                                                                 |
| BR-SCH-ROOM-DISPLAY-007 | Với buổi học Live Online, trường filter **Type** của phòng học bị disable.                                                                                                 |
| BR-SCH-ROOM-DISPLAY-008 | Người dùng có thể tìm kiếm phòng học theo **Name** hoặc **Code**.                                                                                                          |
| BR-SCH-ROOM-DISPLAY-009 | Người dùng có thể lọc phòng học theo **Type** nếu Learning Mode không phải Live Online.                                                                                    |
| BR-SCH-ROOM-DISPLAY-010 | Với lớp Live Online, sau khi chọn phòng học ảo thành công, hệ thống hiển thị và bắt buộc nhập trường **Link Meeting**.                                                     |
| BR-SCH-ROOM-DISPLAY-011 | Khi người dùng chọn phòng học và bấm **Add**, hệ thống ghi nhận phòng học cho buổi học hoặc cho lịch học tự động của lớp.                                                  |
| BR-SCH-ROOM-DISPLAY-012 | Khi người dùng chỉnh sửa Classroom của lớp Live Online hoặc Hybrid, hệ thống có thể yêu cầu nhập lại **Link Meeting** để đảm bảo thông tin phòng học trực tuyến chính xác. |

</details>
