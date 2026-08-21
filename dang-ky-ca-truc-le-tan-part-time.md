# Đăng ký ca trực (Lễ tân Part-time)

## Record of changes

\*A - Add M - Modify D - Delete

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |
| May 18, 2026   |               |       |                                |         |

## I. Thông tin chung

**Dành cho:** Receptionist Part-time, Facility Manager, Admin/Ops User

**Đường dẫn:** Customer Experience → Receptionist → Receptionist Shift

### Phạm vi & Module liên quan

* **Module chính:** Customer Experience / Receptionist
* **Chức năng chính:** Receptionist Shift / Register Shift
* **Module liên quan:** Facility, Classroom, Class Calendar, Receptionist Shift Management

### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản người dùng là **Receptionist Part-time**.
* Tài khoản có quyền truy cập chức năng **Receptionist Shift** và quyền **Register Shift**.
* Người dùng thực hiện đăng ký trong thời gian hệ thống cho phép.

{% hint style="info" %}
Nút **Register Shift** chỉ hiển thị với tài khoản **Receptionist Part-time** trong các ngày hệ thống cho phép đăng ký: từ ngày \*\*01–\*\***26** hàng tháng. Ngoài các ngày trên, hệ thống không hiển thị nút Register Shift.
{% endhint %}

## II. Hướng dẫn chi tiết

### Đăng ký ca trực

{% stepper %}
{% step %}
## Truy cập màn hình Receptionist Shift

Lễ tân Part-time truy cập **Customer Experience → Receptionist → Receptionist Shift** trên thanh menu.

![](<.gitbook/assets/image (726)>)

Hệ thống hiển thị màn hình danh sách lịch trực.
{% endstep %}

{% step %}
## Chọn Register Shift

Lễ tân Part-time chọn **Register Shift** tại màn hình **Receptionist Shift**.

![](<.gitbook/assets/image (727)>)

Hệ thống mở màn hình đăng ký ca trực nếu người dùng đang trong thời gian được phép đăng ký.

![](<.gitbook/assets/image (729)>)
{% endstep %}

{% step %}
## Chọn Facility

Lễ tân Part-time chọn **Facility** tại vùng bộ lọc nếu cần xem lịch trực theo cơ sở.
{% endstep %}

{% step %}
## Chọn Search

Lễ tân Part-time chọn **Search**. Hệ thống hiển thị danh sách ca trực thuộc cơ sở đã chọn.
{% endstep %}

{% step %}
## Chuyển tuần (nếu cần)

Lễ tân Part-time chọn nút mũi tên trái/phải nếu cần chuyển sang tuần khác. Hệ thống hiển thị danh sách ca trực theo tuần tương ứng.
{% endstep %}

{% step %}
## Tick checkbox đăng ký ca

Lễ tân Part-time tick checkbox tại ca trực muốn đăng ký. Hệ thống ghi nhận ca trực được chọn.
{% endstep %}

{% step %}
## Bỏ tick để hủy đăng ký (nếu cần)

Lễ tân Part-time bỏ tick checkbox tại ca trực đã đăng ký nếu muốn hủy đăng ký ca đó.
{% endstep %}

{% step %}
## Chọn Save

Lễ tân Part-time chọn **Save**. Hệ thống kiểm tra số lượng ca đăng ký và lưu thông tin nếu dữ liệu hợp lệ.
{% endstep %}
{% endstepper %}

### Hủy thao tác đăng ký ca trực

{% stepper %}
{% step %}
## Chọn Cancel

Lễ tân Part-time chọn **Cancel** tại màn hình **Register Shift**.

![](<.gitbook/assets/image (731)>)

Hệ thống hiển thị popup xác nhận hủy thao tác.

![](<.gitbook/assets/image (734)>)
{% endstep %}

{% step %}
## Xác nhận hủy

Lễ tân Part-time chọn **Yes** để kết thúc thao tác đăng ký và quay lại màn hình danh sách lịch trực; chọn **No** để đóng popup và quay lại màn hình **Register Shift**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Chức năng **Register Shift** chỉ áp dụng cho tài khoản **Receptionist Part-time**.
2. Lễ tân Part-time chỉ được đăng ký ca trực trong các ngày hệ thống cho phép: từ ngày **01–15** và ngày **25–26** hàng tháng.
3. Ngoài thời gian trên, hệ thống không hiển thị nút **Register Shift**.
4. Các ca đã đăng ký thành công trước đó sẽ hiển thị checkbox đã được tick.
5. Người dùng có thể bỏ tick checkbox để hủy đăng ký ca trực tương ứng.

### Quy tắc thời gian đăng ký ca trực

| Quy tắc               | Mô tả                                           |
| --------------------- | ----------------------------------------------- |
| Ngày 01–15 hàng tháng | Lễ tân Part-time được đăng ký ca trực.          |
| Ngày 25–26 hàng tháng | Lễ tân Part-time được đăng ký ca trực.          |
| Ngoài các ngày trên   | Hệ thống không hiển thị nút **Register Shift**. |

### Quy tắc hiển thị ca trực với Lễ tân Part-time

| Thời gian                            | Quy tắc hiển thị                                              |
| ------------------------------------ | ------------------------------------------------------------- |
| Thứ hai đến Thứ sáu                  | Mặc định chỉ hiển thị ca tối.                                 |
| Thứ bảy, Chủ nhật                    | Hiển thị cả ba ca sáng, chiều và tối.                         |
| Ca sáng/chiều từ Thứ hai đến Thứ sáu | Chỉ hiển thị nếu Lễ tân Part-time đã được gắn với ca trực đó. |

### Quy tắc số lượng ca đăng ký

| Quy tắc                 | Mô tả                                                                                                                                                |
| ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| Số ca tối thiểu/tuần    | Lễ tân Part-time cần đăng ký tối thiểu **04 ca/tuần**.                                                                                               |
| Số ca tối đa/tuần       | Không được vượt quá số ca tối đa do hệ thống tính theo từng cơ sở và từng tuần.                                                                      |
| Công thức số ca tối đa  | `(Tổng số người trực cần có của tuần - Số ca trực Lễ tân Full-time đã đăng ký) / Số lượng Lễ tân Part-time của cơ sở`, làm tròn lên đến hàng đơn vị. |
| Chưa đủ số ca tối thiểu | Khi chọn Save, hệ thống hiển thị popup cảnh báo: _"Bạn chưa đăng ký đủ số lượng ca tối thiểu. Bạn có chắc chắn lưu đăng ký không?"_                  |
| Chọn Yes tại popup      | Hệ thống vẫn lưu thông tin ca đăng ký.                                                                                                               |
| Chọn No tại popup       | Hệ thống quay lại màn hình đăng ký ca trực.                                                                                                          |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                          | Nguyên nhân                                                                              | Cách xử lý                                            |
| ----------------------------------------- | ---------------------------------------------------------------------------------------- | ----------------------------------------------------- |
| Không thấy nút Register Shift             | Không trong thời gian được phép đăng ký hoặc tài khoản không phải Receptionist Part-time | Kiểm tra ngày hiện tại và loại tài khoản              |
| Không thấy lịch trực để đăng ký           | Chưa chọn đúng cơ sở hoặc tuần cần xem chưa có dữ liệu                                   | Chọn lại Facility, chuyển tuần hoặc bấm Search        |
| Không lưu được đăng ký                    | Dữ liệu đăng ký không hợp lệ hoặc vượt rule số ca tối đa                                 | Kiểm tra lại số ca đã chọn theo tuần                  |
| Hệ thống cảnh báo chưa đủ số ca tối thiểu | Người dùng đăng ký dưới 04 ca/tuần                                                       | Chọn thêm ca hoặc chọn Yes nếu vẫn muốn lưu           |
| Checkbox đã được tick sẵn                 | Ca trực đã được đăng ký trước đó                                                         | Giữ nguyên nếu vẫn muốn đăng ký, bỏ tick nếu muốn hủy |
| Bấm Cancel nhưng chưa lưu thay đổi        | Người dùng thoát khỏi màn hình đăng ký                                                   | Chọn No để quay lại đăng ký hoặc Yes để hủy thao tác  |
