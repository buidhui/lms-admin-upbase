# Chỉnh sửa lịch trực

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin/Ops User, Facility Manager, Receptionist Full-time, Receptionist Part-time

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Shift

#### Phạm vi & Module liên quan

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Edit Shift
* **Module liên quan:** Facility, Classroom, Class Calendar, Classroom Calendar, Receptionist Shift Management

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Receptionist Shift**.
* Tài khoản có quyền chỉnh sửa lịch trực của Lễ tân.

Màn hình chỉnh sửa gồm 3 nhóm thông tin: **Shift Information** (Date, Shift), **On-call Person** (danh sách Lễ tân trực), **Room Holder Information** (Room Holder, Attendant, Note). Chỉ **On-call Person, Attendant, Note** được chỉnh sửa; **Date, Shift, Room Holder** chỉ để xem.

## II. Hướng dẫn chi tiết

### Chỉnh sửa lịch trực

{% stepper %}
{% step %}
## Truy cập màn hình Receptionist Shift

Người dùng truy cập **Customer Experience → Receptionist → Receptionist Shift** trên thanh menu.

![](<.gitbook/assets/image (728)>)

Hệ thống hiển thị màn hình danh sách lịch trực.

![](<.gitbook/assets/image (730)>)
{% endstep %}

{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng chọn **Facility** và **Start date - End date** để hiển thị danh sách lịch trực cần chỉnh sửa.
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách lịch trực thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
## Chọn Action → Edit

Người dùng chọn **Action → Edit** tại ca trực cần chỉnh sửa.

![](<.gitbook/assets/image (732)>)

Hệ thống mở màn hình chỉnh sửa lịch trực.

![](<.gitbook/assets/image (733)>)
{% endstep %}

{% step %}
## Kiểm tra Date và Shift

Người dùng kiểm tra thông tin **Date** và **Shift** (thông tin chỉ xem, không thể chỉnh sửa).
{% endstep %}

{% step %}
## Chỉnh sửa On-call Person (nếu được phép)

Người dùng chỉnh sửa **On-call Person** nếu tài khoản được phép — có thể tìm kiếm, chọn thêm nhiều Lễ tân hoặc xóa Lễ tân đang có trong ca trực.
{% endstep %}

{% step %}
## Nhập Attendant

Người dùng nhập **Attendant** tại phần **Room Holder Information** nếu cần cập nhật số lượng học viên thực tế.
{% endstep %}

{% step %}
## Nhập Note

Người dùng nhập **Note** tại phần **Room Holder Information** nếu cần bổ sung ghi chú cho ca trực.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save**. Hệ thống lưu thông tin đã chỉnh sửa và quay lại màn hình danh sách lịch trực.
{% endstep %}
{% endstepper %}

### Hủy thao tác chỉnh sửa lịch trực

{% stepper %}
{% step %}
## Chọn Cancel

Người dùng chọn **Cancel** tại màn hình chỉnh sửa lịch trực. Hệ thống hiển thị popup xác nhận hủy thao tác.
{% endstep %}

{% step %}
## Xác nhận hủy

Người dùng chọn **Yes** để kết thúc thao tác chỉnh sửa và quay lại màn hình danh sách lịch trực; chọn **No** để đóng popup và quay lại màn hình chỉnh sửa.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền chỉnh sửa lịch trực để sử dụng chức năng **Edit Receptionist Shift**.
2. Tài khoản **Receptionist Full-time** có thể chỉnh sửa tất cả các ca trực có trên hệ thống theo phạm vi được phân quyền.
3. Tài khoản **Receptionist Part-time** chỉ có thể chỉnh sửa các ca trực có chính họ trong danh sách người trực.
4. Trường **Date**, **Shift** và **Room Holder** không được phép chỉnh sửa.
5. Trường **Attendant** dùng để cập nhật số lượng học viên thực tế.
6. Khi chọn quá số lượng Lễ tân cần có trong một ca, hệ thống hiển thị cảnh báo **"Too many receptionists scheduled for this shift."** nhưng vẫn cho phép lưu.
7. Nếu chọn **Cancel** khi đang chỉnh sửa, các thay đổi chưa lưu sẽ không được ghi nhận nếu người dùng xác nhận thoát.

### Quy tắc chỉnh sửa theo loại tài khoản

| Loại tài khoản         | Quy tắc                                                                                               |
| ---------------------- | ----------------------------------------------------------------------------------------------------- |
| Receptionist Full-time | Được phép chỉnh sửa tất cả các ca trực có trên hệ thống theo phạm vi được phân quyền.                 |
| Receptionist Full-time | Được phép chỉnh sửa trường **On-call Person**.                                                        |
| Receptionist Full-time | Có thể gán Lễ tân Part-time vào ca trực kể cả khi Lễ tân Part-time đó đã đạt số lượng ca trực tối đa. |
| Receptionist Part-time | Chỉ được chỉnh sửa các ca trực có chính họ trong danh sách người trực.                                |
| Receptionist Part-time | Không được chỉnh sửa trường **On-call Person**.                                                       |
| Receptionist Part-time | Có thể cập nhật các thông tin được phép như Attendant và Note nếu ca trực có chính họ.                |

### Quy tắc số lượng Lễ tân cần có trong một ca

| Facility      | Số phòng trong ca  | Số lượng Lễ tân cần có |
| ------------- | ------------------ | ---------------------- |
| NEU           | 1 - 2 phòng        | 1 Lễ tân               |
| NEU           | 3 - 4 phòng        | 2 Lễ tân               |
| NEU           | 5 - 6 phòng        | 3 Lễ tân               |
| Facility khác | 1 - 2 phòng        | 1 Lễ tân               |
| Facility khác | Từ 3 phòng trở lên | 2 Lễ tân               |

### Quy tắc cảnh báo khi vượt số lượng Lễ tân

| Trường hợp                                                    | Quy tắc xử lý                                                                     |
| ------------------------------------------------------------- | --------------------------------------------------------------------------------- |
| Người dùng chọn số lượng Lễ tân vượt số lượng cần có trong ca | Hệ thống hiển thị cảnh báo **"Too many receptionists scheduled for this shift."** |
| Sau khi hiển thị cảnh báo                                     | Hệ thống vẫn cho phép người dùng lưu thông tin ca trực.                           |
| Người dùng muốn điều chỉnh lại                                | Người dùng xóa bớt On-call Person trước khi chọn Save.                            |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                                     | Nguyên nhân                                                   | Cách xử lý                                                                 |
| -------------------------------------------------------------------- | ------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Không thấy nút Edit                                                  | Tài khoản chưa có quyền chỉnh sửa lịch trực                   | Liên hệ Admin hệ thống để kiểm tra phân quyền                              |
| Không mở được màn hình chỉnh sửa                                     | Ca trực không thuộc phạm vi được phép chỉnh sửa               | Kiểm tra quyền và loại tài khoản                                           |
| Receptionist Part-time không sửa được On-call Person                 | Theo rule hệ thống, Part-time không được chỉnh sửa trường này | Chỉ cập nhật các trường được phép hoặc liên hệ Facility Manager            |
| Hệ thống cảnh báo "Too many receptionists scheduled for this shift." | Số lượng Lễ tân được chọn vượt số lượng cần có trong ca       | Kiểm tra lại số phòng và số người trực cần có; có thể lưu nếu vẫn muốn giữ |
| Attendant không chính xác                                            | Người dùng nhập sai số lượng học viên thực tế                 | Chỉnh sửa lại Attendant và chọn Save                                       |
| Chọn Cancel bị mất thay đổi                                          | Người dùng xác nhận thoát mà chưa lưu                         | Chọn Save trước khi thoát nếu muốn lưu thay đổi                            |
| Không thấy ca cần chỉnh sửa                                          | Bộ lọc Facility hoặc thời gian chưa đúng                      | Chọn lại điều kiện tìm kiếm và bấm Search                                  |
