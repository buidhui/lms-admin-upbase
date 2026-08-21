# Subject Category

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin

**Đường dẫn:** Academic Management → Course & Materials → Subject Category

#### Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Subject Category
* **Module liên quan:** Program Category, Course, Course 4 Level, Class

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Tài khoản có quyền truy cập menu **Subject Category** và quyền thao tác với Subject.

## II. Hướng dẫn chi tiết

### Xem danh sách Subject Category

{% stepper %}
{% step %}
## Mở màn hình Subject Category

Màn hình hiển thị danh sách Subject như sau:

![](<.gitbook/assets/image (554)>)
{% endstep %}

{% step %}
## Tìm kiếm/lọc danh sách Subject

Tại màn hình Subject Category, Admin có thể tìm kiếm/lọc danh sách Subject theo tên, Program hoặc ngày tạo tại khu vực tìm kiếm.

![](<.gitbook/assets/image (557)>)

Các thông tin hiển thị trong danh sách Subject:

| Thông tin    | Mô tả                            |
| ------------ | -------------------------------- |
| Subject name | Tên môn học                      |
| Code         | Mã môn học                       |
| Program      | Chương trình học gán với môn học |
| Updated at   | Thời gian cập nhật gần nhất      |
{% endstep %}
{% endstepper %}

### Tạo một Subject

{% stepper %}
{% step %}
## Click Add Subject

Admin click button **Add Subject** tại màn hình.

![](<.gitbook/assets/image (559)>)
{% endstep %}

{% step %}
## Nhập thông tin Subject

Admin nhập thông tin vào form tạo mới Subject hiển thị phía bên phải:

![](<.gitbook/assets/image (561)>)

* **Tên Subject:** trường bắt buộc phải nhập để có thể tạo mới.
* **Code:** trường không bắt buộc, người dùng nhập mã của môn học.
* **Program:** chương trình học gán với môn học.
{% endstep %}

{% step %}
## Click Save để lưu

Admin click button **Save** để lưu Subject mới. Sau khi lưu, màn hình hiển thị message thông báo tạo mới Subject thành công.
{% endstep %}
{% endstepper %}

### Chỉnh sửa một Subject

{% stepper %}
{% step %}
## Chọn Action → Edit

Để chỉnh sửa Subject đã tạo, Admin click vào biểu tượng **Action** tại Subject muốn chỉnh sửa rồi chọn **Edit**.

![](<.gitbook/assets/image (563)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin Subject

Thông tin của Subject hiển thị phía bên phải. Admin chỉnh sửa:

![](<.gitbook/assets/image (565)>)

* **Tên Subject**
* **Code:** Admin có thể nhập/xóa code của Subject.
* **Program**
{% endstep %}

{% step %}
## Click Save để lưu

Sau khi chỉnh sửa, Admin click **Save** để lưu thông tin mới. Màn hình hiển thị message thông báo lưu thông tin thành công.
{% endstep %}
{% endstepper %}

{% hint style="warning" %}
Subject đã gán với khóa học thì không thể xóa.
{% endhint %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Subject là môn học thuộc một Program; Admin cần chọn đúng Program khi tạo mới hoặc chỉnh sửa Subject.
2. Trường **Name** là trường bắt buộc.
3. Trường **Code** dùng để định danh Subject, nên đặt ngắn gọn và dễ nhận diện.
4. Một Subject có thể được sử dụng để cấu hình Course.
5. Subject đã được gán với khóa học thì **không thể xóa**.
6. Khi chọn **Delete**, hệ thống kiểm tra ràng buộc dữ liệu giữa Subject và Course.
7. Nếu Subject đang được sử dụng, nên chỉnh sửa thông tin thay vì xóa.

#### Mẹo sử dụng

1. Nên đặt tên Subject rõ ràng, đúng tên môn học và thống nhất theo quy chuẩn nội bộ.
2. Nên nhập **Code** theo format dễ nhận diện, ví dụ tên viết tắt hoặc slug không dấu.
3. Khi danh sách Subject nhiều, nên dùng bộ lọc **Program** để thu hẹp phạm vi tìm kiếm.
4. Nên kiểm tra kỹ Subject đã được gán vào Course hay chưa trước khi thực hiện xóa.
5. Với Subject đã sử dụng trong khóa học, nên hạn chế chỉnh sửa Program để tránh ảnh hưởng đến việc phân loại Course.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                          | Nguyên nhân                             | Cách xử lý                                                             |
| ----------------------------------------- | --------------------------------------- | ---------------------------------------------------------------------- |
| Không tạo/lưu được Subject                | Chưa nhập Tên Subject (trường bắt buộc) | Nhập đầy đủ Tên Subject rồi bấm Save                                   |
| Không gán được Subject vào Program        | Program chưa tồn tại trên hệ thống      | Tạo Program tương ứng trước, sau đó gán Subject                        |
| Không tìm thấy Subject                    | Sai điều kiện tìm kiếm/lọc              | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định             |
| Không xóa được Subject                    | Subject đã được gán với khóa học        | Gỡ Subject khỏi các Course liên quan trước, hoặc chỉnh sửa thay vì xóa |
| Không thực hiện được thao tác tạo/sửa/xóa | Tài khoản chưa được cấp quyền tương ứng | Liên hệ quản trị để được cấp quyền với Subject Category                |
