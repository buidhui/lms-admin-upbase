# Program Category

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin

**Đường dẫn:** Course & Materials → Program Category
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Course & Materials
* **Chức năng chính:** Program Category
* **Module liên quan:** Course
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành.
* Tài khoản có quyền truy cập menu **Program Category** và quyền xem danh sách Program Category.
* Tạo mới: cần quyền tạo Program Category.
* Chỉnh sửa: cần quyền chỉnh sửa Program Category.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách Program Category</summary>

{% stepper %}
{% step %}
**Mở màn hình Program Category**

Màn hình hiển thị danh sách Program như sau:

<figure><img src="../../.gitbook/assets/image (61).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm/lọc danh sách**

Tại màn hình Program Category, Admin có thể tìm kiếm/lọc danh sách theo tên hoặc ngày tạo tại khu vực tìm kiếm.

<figure><img src="../../.gitbook/assets/image (62).png" alt=""><figcaption></figcaption></figure>

Các thông tin hiển thị trong danh sách Program:

| **Thông tin** | **Mô tả**                      |
| ------------- | ------------------------------ |
| Category name | Tên loại chương trình học      |
| Description   | Mô tả chương trình học         |
| Created       | Thời gian tạo chương trình học |
| Updated       | Thời gian cập nhật gần nhất    |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo một Program</summary>

{% stepper %}
{% step %}
**Click Add Category**

Admin click button **Add Category** tại màn hình.

<figure><img src="../../.gitbook/assets/image (63).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin Program**

Admin nhập thông tin vào form tạo mới Program hiển thị phía bên phải:

<figure><img src="../../.gitbook/assets/image (64).png" alt=""><figcaption></figcaption></figure>

* **Tên Program:** trường bắt buộc, không được phép trùng với Program đã tồn tại.
* **Mô tả:** trường không bắt buộc, Admin có thể điền hoặc để trống.
{% endstep %}

{% step %}
**Click Save để lưu**

Admin click button **Save** để lưu Program mới. Sau khi lưu, màn hình hiển thị message thông báo tạo mới Program thành công.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa một Program</summary>

{% stepper %}
{% step %}
**Chọn Action → Edit**

Để chỉnh sửa Program đã tạo, Admin click vào biểu tượng **Action** tại Program muốn chỉnh sửa rồi chọn **Edit**.

<figure><img src="../../.gitbook/assets/image (65).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin Program**

Thông tin của Program hiển thị phía bên phải. Admin chỉnh sửa:

<figure><img src="../../.gitbook/assets/image (66).png" alt=""><figcaption></figcaption></figure>

* **Tên Program:** đảm bảo không trùng với Program đã tồn tại.
* **Mô tả Program:** Admin có thể nhập/xóa nội dung mô tả.
{% endstep %}

{% step %}
**Click Save để lưu**

Sau khi chỉnh sửa, Admin click **Save** để lưu thông tin mới. Màn hình hiển thị message thông báo lưu thông tin thành công.

{% hint style="warning" %}
Program đã tạo thì không thể xóa khỏi danh sách.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Admin cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa Program Category.
2. Tên Program Category không được phép trùng với Program Category đã tồn tại.
3. Trường **Description** không bắt buộc, Admin có thể nhập hoặc để trống.
4. Program Category đã tạo thì **không thể xóa khỏi danh sách**.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Trước khi tạo mới, nên tìm kiếm theo tên để kiểm tra Program Category đã tồn tại hay chưa.
2. Nên đặt tên ngắn gọn, rõ nghĩa và thống nhất theo quy chuẩn đặt tên của hệ thống.
3. Nên nhập mô tả để người dùng khác hiểu rõ Program Category dùng cho nhóm chương trình học nào.
4. Với Program Category tạo sai hoặc không còn dùng (do không hỗ trợ xóa), nên cân nhắc chỉnh sửa tên/mô tả theo quy ước nội bộ, ví dụ thêm ghi chú "Không sử dụng" nếu được phép.
5. Khi chỉnh sửa tên, cần kiểm tra kỹ để tránh ảnh hưởng đến việc nhận diện nhóm chương trình học ở các màn hình liên quan.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                           | Nguyên nhân                                       | Cách xử lý                                                        |
| ------------------------------------------ | ------------------------------------------------- | ----------------------------------------------------------------- |
| Không tạo/lưu được Program Category        | Chưa nhập Tên Program (trường bắt buộc)           | Nhập đầy đủ Tên Program rồi bấm Save                              |
| Báo lỗi tên bị trùng                       | Tên Program trùng với Program Category đã tồn tại | Đặt tên khác, không trùng với Program đã có                       |
| Không tìm thấy Program Category            | Sai điều kiện tìm kiếm/lọc                        | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định        |
| Muốn xóa Program Category nhưng không được | Hệ thống không hỗ trợ xóa Program Category đã tạo | Chỉnh sửa tên/mô tả theo quy ước nội bộ (vd thêm "Không sử dụng") |
| Không thực hiện được thao tác tạo/sửa      | Tài khoản chưa được cấp quyền tương ứng           | Liên hệ quản trị để được cấp quyền tạo/chỉnh sửa Program Category |
