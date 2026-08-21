# Xem và quản lý phòng học (Classroom)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |
| May 18, 2026   |               |       |                                |         |

## I. Thông tin chung

**Dành cho:** Admin, CX/Admin cơ sở

**Đường dẫn:** Department Operations → Share Services → Classroom List

#### Phạm vi & Module liên quan

* **Module chính:** Operation
* **Chức năng chính:** Classroom
* **Module liên quan:** Facility, Class, Calendar, Classroom Booking, Learning Schedule

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập menu **Classroom List**.

Màn hình **Room Detail** gồm các tab: **Overview, Settings, Inactive Period**. Phòng học có 2 Mode: **Physical** (vật lý, gắn Facility) và **Virtual** (ảo, dùng cho lớp Live Online).

## II. Hướng dẫn chi tiết

### Xem danh sách phòng học

{% stepper %}
{% step %}
## Mở màn hình Classroom List

Người dùng chọn **Classroom List** tại menu **Share Services**.

![](<.gitbook/assets/image (704)>)

Hệ thống hiển thị màn hình **Classroom List**.

![](<.gitbook/assets/image (705)>)
{% endstep %}

{% step %}
## Xem thông tin phòng học

Người dùng xem thông tin tại bảng danh sách: Code, Name, Facility, Type, Capacity, Mode và Status của từng phòng học.
{% endstep %}
{% endstepper %}

### Tìm kiếm/lọc phòng học

{% stepper %}
{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng nhập hoặc chọn điều kiện tại màn hình **Classroom List** (tên/mã phòng học, Mode, Facility, Type hoặc Status).

![](<.gitbook/assets/image (706)>)
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách phòng học thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
## Chọn Reset

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại danh sách phòng học theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết phòng học

{% stepper %}
{% step %}
## Mở Room Detail

Người dùng nhấp vào **tên phòng học** tại màn hình **Classroom List**.

![](<.gitbook/assets/image (707)>)

Hệ thống mở màn hình **Room Detail**.

![](<.gitbook/assets/image (708)>)
{% endstep %}

{% step %}
## Xem thông tin tại tab Overview

Người dùng xem thông tin phòng học tại tab **Overview**. Hệ thống hiển thị thông tin chi tiết tương ứng với Mode của phòng học (Physical: Name, Code, Mode, Facility, Type, Status, Floor, Capacity; Virtual: Name, Code, Mode, Additional Information).
{% endstep %}
{% endstepper %}

### Tạo mới phòng học

{% stepper %}
{% step %}
## Chọn Create Room

Người dùng chọn **Create Room** tại màn hình **Classroom List**.

![](<.gitbook/assets/image (709)>)

Hệ thống mở màn hình **Create Classroom**.

![](<.gitbook/assets/image (710)>)
{% endstep %}

{% step %}
## Chọn Mode

Người dùng chọn **Mode**: **Physical** (phòng học vật lý) hoặc **Virtual** (phòng học ảo).

![](<.gitbook/assets/image (711)>)
{% endstep %}

{% step %}
## Nhập thông tin theo Mode

* Phòng học **Physical**: nhập Name, Facility, Type, Floor và Capacity.
* Phòng học **Virtual**: nhập Name và Additional Information nếu có.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Create Classroom**. Hệ thống lưu thông tin và tự động tạo mã phòng học theo quy tắc hệ thống.
{% endstep %}
{% endstepper %}

### Tạo phòng học từ Facility Detail

{% stepper %}
{% step %}
## Mở Facility Detail

Người dùng mở màn hình **Facility Detail** của cơ sở cần tạo phòng học.
{% endstep %}

{% step %}
## Chọn tab Classroom List

Người dùng chọn tab **Classroom List** tại màn hình Facility Detail.
{% endstep %}

{% step %}
## Chọn Create Classroom

Người dùng chọn **Create Classroom** tại tab **Classroom List**.

![](<.gitbook/assets/image (712)>)

Hệ thống mở màn hình tạo mới phòng học và có thể tự động gắn phòng học với Facility hiện tại.

![](<.gitbook/assets/image (713)>)
{% endstep %}

{% step %}
## Nhập thông tin và Save

Người dùng nhập thông tin phòng học và chọn **Save**. Hệ thống tạo mới phòng học thuộc cơ sở đang xem.
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin phòng học từ Classroom List

{% stepper %}
{% step %}
## Chọn Action → Edit

Người dùng chọn **Action → Edit** tại phòng học cần chỉnh sửa trên màn hình **Classroom List**.

![](<.gitbook/assets/image (714)>)

Hệ thống mở màn hình chỉnh sửa phòng học.

![](<.gitbook/assets/image (715)>)
{% endstep %}

{% step %}
## Cập nhật thông tin

Người dùng cập nhật thông tin tại màn hình **Edit Classroom**, chỉnh sửa các trường được phép theo Mode và điều kiện sử dụng của phòng học.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Edit Classroom**. Hệ thống lưu thông tin mới của phòng học.
{% endstep %}
{% endstepper %}

### Chỉnh sửa thông tin phòng học từ Room Detail

{% stepper %}
{% step %}
## Mở Room Detail

Người dùng mở màn hình **Room Detail** của phòng học cần chỉnh sửa.
{% endstep %}

{% step %}
## Chọn tab Settings

Người dùng chọn tab **Settings** tại màn hình **Room Detail**.

![](<.gitbook/assets/image (716)>)

Hệ thống hiển thị màn hình **Edit Classroom**.
{% endstep %}

{% step %}
## Cập nhật thông tin và Save

Người dùng cập nhật thông tin cần chỉnh sửa, sau đó chọn **Save** để lưu thông tin mới.
{% endstep %}
{% endstepper %}

### Cập nhật trạng thái phòng học tại Classroom List

{% stepper %}
{% step %}
## Chọn dropdown Status

Người dùng chọn dropdown **Status** tại dòng phòng học cần cập nhật trên màn hình **Classroom List**.

![](<.gitbook/assets/image (717)>)
{% endstep %}

{% step %}
## Chọn trạng thái mới

Người dùng chọn trạng thái mới cho phòng học. Hệ thống cập nhật trạng thái nếu phòng học đủ điều kiện thay đổi trạng thái.
{% endstep %}
{% endstepper %}

### Xem danh sách Inactive Period của phòng học

{% stepper %}
{% step %}
## Mở Room Detail

Người dùng mở màn hình **Room Detail** của phòng học cần xem.
{% endstep %}

{% step %}
## Chọn tab Inactive Period

Người dùng chọn tab **Inactive Period**.

![](<.gitbook/assets/image (718)>)

Hệ thống hiển thị danh sách khoảng thời gian không hoạt động của phòng học (From, To, Reason, Action).
{% endstep %}
{% endstepper %}

### Thêm Inactive Period cho phòng học

{% stepper %}
{% step %}
## Chọn Add Inactive Period

Người dùng chọn **Add Inactive Period** tại tab **Inactive Period**.

![](<.gitbook/assets/image (719)>)

Hệ thống mở popup/màn hình thêm khoảng thời gian không hoạt động.

![](<.gitbook/assets/image (720)>)
{% endstep %}

{% step %}
## Nhập From, To, Reason

Người dùng nhập **From**, **To** và **Reason**.
{% endstep %}

{% step %}
## Chọn Save / Add

Người dùng chọn **Save** hoặc **Add** để lưu.

![](<.gitbook/assets/image (721)>)

Hệ thống thêm khoảng thời gian không hoạt động vào danh sách Inactive Period và chuyển sang màn **Check room schedule** để kiểm tra ai đang mượn phòng vào khoảng thời gian đó.
{% endstep %}
{% endstepper %}

### Xóa Inactive Period của phòng học

{% stepper %}
{% step %}
## Chọn biểu tượng Delete

Người dùng chọn biểu tượng **Delete** tại dòng Inactive Period cần xóa.

![](<.gitbook/assets/image (722)>)

Hệ thống hiển thị popup xác nhận xóa nếu có.

![](<.gitbook/assets/image (723)>)
{% endstep %}

{% step %}
## Xác nhận xóa

Người dùng chọn **Yes** để xác nhận xóa. Hệ thống xóa khoảng thời gian không hoạt động khỏi danh sách.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền tương ứng để xem, tạo, chỉnh sửa, cập nhật trạng thái hoặc xóa phòng học.
2. Phòng học có 2 Mode chính: **Physical** (vật lý, gắn Facility) và **Virtual** (ảo, dùng cho buổi Live Online).
3. Tên phòng học mới không được trùng với tên của các phòng học đã tạo.
4. Với phòng học Physical: **Capacity** là sức chứa tối đa; trường **Floor** chỉ cần nhập số tầng.
5. Những phòng học đang được sử dụng (đã được đặt lịch trong tương lai) không được phép chỉnh sửa **Status**.

### Quy tắc tạo phòng học

| Quy tắc            | Mô tả                                                      |
| ------------------ | ---------------------------------------------------------- |
| Name               | Tên phòng học không được trùng với phòng học đã tồn tại.   |
| Mode               | Bắt buộc chọn Physical hoặc Virtual.                       |
| Physical Classroom | Cần nhập Name, Facility, Type, Floor và Capacity.          |
| Virtual Classroom  | Cần nhập Name và Additional Information nếu có.            |
| Floor              | Người dùng chỉ nhập số tầng, ví dụ 1, 2, 3.                |
| Capacity           | Với phòng vật lý, dùng để xác định sức chứa của phòng học. |
| Save               | Sau khi lưu thành công, hệ thống tự động tạo mã phòng học. |

### Quy tắc sinh mã phòng học

| Loại phòng học     | Quy tắc sinh mã                             |
| ------------------ | ------------------------------------------- |
| Physical Classroom | `CR` + mã cơ sở + `.` + số thứ tự phòng học |
| Virtual Classroom  | `CRO` + `.` + số thứ tự phòng học           |

### Quy tắc tìm kiếm/lọc phòng học

| Điều kiện | Quy tắc                                                    |
| --------- | ---------------------------------------------------------- |
| Search    | Tìm theo Classroom name hoặc Classroom code.               |
| Mode      | Chọn một trong các giá trị Physical hoặc Virtual.          |
| Facility  | Chỉ áp dụng khi Mode = Physical.                           |
| Type      | Chỉ áp dụng khi Mode = Physical.                           |
| Status    | Chọn một trong các trạng thái hệ thống hỗ trợ.             |
| Reset     | Xóa điều kiện tìm kiếm và hiển thị lại danh sách mặc định. |

### Quy tắc chỉnh sửa phòng học

| Quy tắc                                    | Mô tả                                                                              |
| ------------------------------------------ | ---------------------------------------------------------------------------------- |
| Physical Classroom                         | Có thể chỉnh sửa Name, Facility, Type, Floor, Capacity và Status nếu đủ điều kiện. |
| Virtual Classroom                          | Có thể chỉnh sửa Name, Additional Information và Status nếu đủ điều kiện.          |
| Phòng học đã được đặt lịch trong tương lai | Không được chỉnh sửa Status.                                                       |
| Save                                       | Sau khi lưu thành công, hệ thống cập nhật thông tin phòng học.                     |

### Quy tắc Inactive Period

| Quy tắc                     | Mô tả                                                                                                   |
| --------------------------- | ------------------------------------------------------------------------------------------------------- |
| From                        | Thời gian bắt đầu phòng học không hoạt động.                                                            |
| To                          | Thời gian kết thúc phòng học không hoạt động.                                                           |
| Reason                      | Lý do phòng học không hoạt động.                                                                        |
| From/To                     | Thời gian To phải lớn hơn hoặc bằng thời gian From.                                                     |
| Hiển thị phòng khi xếp lịch | Phòng học đang thuộc Inactive Period có thể không được hiển thị để chọn lịch trong khoảng thời gian đó. |
| Xóa Inactive Period         | Người dùng có thể xóa Inactive Period nếu có quyền và dữ liệu đủ điều kiện.                             |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                | Nguyên nhân                                           | Cách xử lý                                                 |
| ------------------------------- | ----------------------------------------------------- | ---------------------------------------------------------- |
| Không tạo/lưu được phòng học    | Tên phòng học bị trùng hoặc thiếu thông tin theo Mode | Đặt tên không trùng, nhập đủ thông tin theo Mode rồi Save  |
| Không đổi được Status phòng học | Phòng học đã được đặt lịch trong tương lai            | Không thể chỉnh sửa Status khi phòng đang được sử dụng     |
| Không xóa được phòng học        | Phòng học đã được đặt lịch trong tương lai            | Phòng đã đặt lịch không được phép xóa                      |
| Không tìm thấy phòng học        | Sai điều kiện tìm kiếm/lọc                            | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định |
| Facility/Type không chọn được   | Mode đang là Virtual                                  | Facility và Type chỉ áp dụng khi Mode = Physical           |
| Lỗi khi thêm Inactive Period    | Thời gian To nhỏ hơn From                             | Nhập To ≥ From; kiểm tra lại From/To/Reason                |
