# Gắn chứng chỉ cho khóa học (Certificate)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

**Dành cho:** Admin, SX

**Đường dẫn:** https://ops.sapp.edu.vn/course-full/undefined

#### Phạm vi & Module liên quan

* **Module chính:** Academic Management / Course & Materials
* **Chức năng chính:** Course 4 Level / Certificate
* **Module liên quan:**
  * Course Info
  * Course Content
  * Resource
  * Certificate Template
  * LMS học viên

#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản người dùng có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công tại bước **Course Info**.

## II. Hướng dẫn chi tiết

### Gán chứng chỉ cho khóa học

{% stepper %}
{% step %}
## Chọn bước Certificate

**Admin chọn bước Certificate trên thanh process hoặc tiếp tục từ bước Resource.**

![](<.gitbook/assets/image (494)>)
{% endstep %}

{% step %}
## Mở danh sách mẫu chứng chỉ

**Admin chọn Choose Template để mở danh sách mẫu chứng chỉ.**

![](<.gitbook/assets/image (495)>)
{% endstep %}

{% step %}
## Chọn mẫu chứng chỉ

**Hệ thống hiển thị popup Choose Certificate Template với danh sách các mẫu chứng chỉ có thể chọn.**

![](<.gitbook/assets/image (496)>)

**Admin tick chọn mẫu chứng chỉ muốn gán cho khóa học.**

Mỗi mẫu chứng chỉ hiển thị thông tin preview và tên template để Admin kiểm tra trước khi chọn.
{% endstep %}

{% step %}
## Xác nhận mẫu chứng chỉ

**Admin chọn Confirm để xác nhận mẫu chứng chỉ đã chọn.**

Sau khi xác nhận, hệ thống đóng popup và gán mẫu chứng chỉ vào khóa học.

![](<.gitbook/assets/image (497)>)
{% endstep %}
{% endstepper %}

### Thay đổi mẫu chứng chỉ đã gán

{% stepper %}
{% step %}
## Truy cập bước Certificate

**Admin mở khóa học cần chỉnh sửa và truy cập bước Certificate.**
{% endstep %}

{% step %}
## Mở danh sách mẫu chứng chỉ

**Admin chọn Icon đổi chứng chỉ để mở lại danh sách mẫu chứng chỉ.**

![](<.gitbook/assets/image (498)>)
{% endstep %}

{% step %}
## Chọn mẫu chứng chỉ mới

**Admin tick chọn mẫu chứng chỉ mới muốn sử dụng.**
{% endstep %}

{% step %}
## Xác nhận cập nhật

**Admin chọn Confirm để cập nhật mẫu chứng chỉ.**
{% endstep %}

{% step %}
## Lưu thay đổi

**Admin chọn Finish hoặc Save theo giao diện hệ thống để lưu thay đổi.**
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. **Certificate** là bước cuối cùng trong quy trình tạo khóa học.
2. Admin cần chọn mẫu chứng chỉ phù hợp với chương trình/khóa học.
3. Nếu chưa có Certificate Template phù hợp, Admin cần tạo hoặc yêu cầu tạo template trước trong chức năng **Certificates**.
4. Việc thay đổi chứng chỉ của khóa học có thể ảnh hưởng đến chứng chỉ học viên nhận được sau khi hoàn thành khóa học.

### Mẹo sử dụng

1. Nên kiểm tra trước tên và hình ảnh preview của Certificate Template trước khi chọn.
2. Nên đặt tên Certificate Template rõ ràng theo chương trình, môn học hoặc loại khóa học để dễ nhận diện.
3. Nếu danh sách template nhiều, nên kiểm tra kỹ template cần chọn để tránh gán nhầm chứng chỉ.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                   | Nguyên nhân                                                                   | Cách xử lý                                                                      |
| ---------------------------------- | ----------------------------------------------------------------------------- | ------------------------------------------------------------------------------- |
| Không thấy nút Choose Template     | Tài khoản chưa có quyền chỉnh sửa khóa học hoặc giao diện chưa tải đủ dữ liệu | Kiểm tra quyền tài khoản, tải lại trang hoặc liên hệ Admin                      |
| Danh sách template trống           | Chưa có Certificate Template khả dụng trên hệ thống                           | Tạo mới template trong chức năng Certificates hoặc kiểm tra trạng thái template |
| Không chọn được template           | Template không khả dụng hoặc người dùng chưa có quyền thao tác                | Kiểm tra trạng thái template và quyền tài khoản                                 |
| Chọn template nhưng chưa được lưu  | Người dùng chưa bấm **Confirm** hoặc chưa bấm **Finish**                      | Chọn lại template, bấm **Confirm**, sau đó bấm **Finish**                       |
| Gán nhầm template                  | Chọn sai mẫu chứng chỉ trong popup                                            | Truy cập lại bước Certificate và chọn lại template đúng                         |
| Học viên không nhận đúng chứng chỉ | Course đang gán sai template hoặc template chưa được cập nhật                 | Kiểm tra lại template đang gán trong bước Certificate                           |
