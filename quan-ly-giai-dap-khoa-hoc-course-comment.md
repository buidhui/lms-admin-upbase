# Quản lý giải đáp khóa học (Course Comment)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

**Dành cho:** Admin/Ops User, Study Experience, Customer Support/CX, Supporter

**Đường dẫn:** Comments → Supporter Group List

#### Phạm vi & Module liên quan

* **Module chính:** Comments
* **Chức năng chính:** Supporter Group List / Create Supporter Group / Edit Supporter Group
* **Module liên quan:** Course, Class, Program, Subject, Student Account, LMS Comment

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập module **Comments** và quyền xem danh sách **Supporter Group**.
* Với thao tác tạo mới/chỉnh sửa/xóa nhóm: tài khoản cần có quyền tương ứng.
* Các tài khoản được thêm vào nhóm cần là tài khoản học viên được đánh dấu **Staff Account / Test Account = Yes**.
* Hệ thống đã có dữ liệu Program và Subject để cấu hình nhóm hỗ trợ.

Mỗi **Supporter Group** được cấu hình theo **Department + Program + Subject**. Các thành viên cùng nhóm dùng chung **Display Name** và **Group Avatar** khi trả lời bình luận trên LMS học viên. Màn hình chi tiết gồm 2 tab: **Group Settings** và **Supporters**.

## II. Hướng dẫn chi tiết

### Xem danh sách Supporter Group

{% stepper %}
{% step %}
## Mở màn hình Supporter Group List

Người dùng chọn **Supporter Group List** tại menu **Comments**. Hệ thống hiển thị màn hình danh sách Supporter Group.
{% endstep %}

{% step %}
## Xem thông tin nhóm

Người dùng xem thông tin tại bảng **Supporter Group List**: Group Name, Program, Subject, Department, Supporters, Created date và Updated date.
{% endstep %}
{% endstepper %}

### Tìm kiếm/lọc Supporter Group

{% stepper %}
{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng nhập hoặc chọn điều kiện tại màn hình **Supporter Group List** (Group Name, Program, Subject, Department, Sort by, From Date - To Date).
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách nhóm hỗ trợ thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
## Chọn Reset

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại danh sách nhóm theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

### Xem chi tiết Supporter Group

{% stepper %}
{% step %}
## Mở chi tiết nhóm

Người dùng nhấp vào **Group Name** tại màn hình **Supporter Group List**. Hệ thống mở màn hình chi tiết Supporter Group.
{% endstep %}

{% step %}
## Xem tab Group Settings

Người dùng xem thông tin tại tab **Group Settings**: Group Avatar, Group Name, Display Name, Department, Program và Subject.
{% endstep %}

{% step %}
## Xem tab Supporters

Người dùng chọn tab **Supporters** để xem danh sách thành viên thuộc nhóm.
{% endstep %}

{% step %}
## Tìm kiếm thành viên (nếu cần)

Người dùng nhập tên hoặc email thành viên và chọn **Search** tại tab **Supporters**. Hệ thống hiển thị danh sách thành viên thỏa mãn điều kiện.
{% endstep %}
{% endstepper %}

### Tạo mới Supporter Group

{% stepper %}
{% step %}
## Chọn Create Supporter Group

Người dùng chọn **Create Supporter Group** tại màn hình **Supporter Group List** hoặc trên menu **Comments**. Hệ thống mở màn hình tạo mới tại bước **Group Settings**.
{% endstep %}

{% step %}
## Nhập Group Name và Display Name

Người dùng nhập **Group Name** và **Display Name** tại màn hình **Group Settings**.
{% endstep %}

{% step %}
## Upload Group Avatar (nếu cần)

Người dùng upload **Group Avatar** tại màn hình **Group Settings** nếu cần. Ảnh này hiển thị chung cho các thành viên trong nhóm khi trả lời bình luận.
{% endstep %}

{% step %}
## Chọn Department, Program và Subject

Người dùng chọn **Department, Program** và **Subject** — 3 thông tin này xác định phạm vi hỗ trợ bình luận của nhóm.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Group Settings**. Hệ thống lưu thông tin cài đặt nhóm và chuyển sang bước thêm thành viên.
{% endstep %}

{% step %}
## Chọn Add Member và tick chọn tài khoản

Người dùng chọn **Add Member** tại màn hình **Add Supporter**, tick chọn một hoặc nhiều tài khoản cần thêm. Danh sách hiển thị là các tài khoản học viên có **Staff Account / Test Account = Yes**.
{% endstep %}

{% step %}
## Chọn Add và Finish

Người dùng chọn **Add** để thêm tài khoản đã chọn vào danh sách Supporter, sau đó chọn **Finish**. Hệ thống hoàn tất tạo mới và hiển thị nhóm vừa tạo tại danh sách.
{% endstep %}
{% endstepper %}

### Chỉnh sửa Supporter Group

{% stepper %}
{% step %}
## Mở màn hình chỉnh sửa

Người dùng chọn **Action → Edit** tại nhóm cần chỉnh sửa hoặc nhấp vào **Group Name**. Hệ thống mở màn hình chỉnh sửa Supporter Group.
{% endstep %}

{% step %}
## Chỉnh sửa tab Group Settings

Nếu nhóm chưa có thành viên: chỉnh sửa toàn bộ thông tin. Nếu nhóm đã có thành viên: chỉ được chỉnh sửa Group Avatar, Group Name và Display Name.
{% endstep %}

{% step %}
## Chỉnh sửa danh sách thành viên (tab Supporters)

Người dùng chọn tab **Supporters**. Hệ thống hiển thị danh sách thành viên hiện tại của nhóm.
{% endstep %}

{% step %}
## Thêm thành viên (nếu cần)

Người dùng chọn **Add Member** tại tab **Supporters** nếu cần thêm thành viên mới. Hệ thống mở danh sách tài khoản đủ điều kiện.
{% endstep %}

{% step %}
## Xóa thành viên (nếu cần)

Người dùng chọn biểu tượng **Delete** tại thành viên cần xóa → chọn **Yes** tại popup xác nhận. Hệ thống xóa thành viên khỏi nhóm và cập nhật phạm vi hiển thị bình luận của tài khoản đó.
{% endstep %}

{% step %}
## Chọn Finish

Người dùng chọn **Finish** để hoàn tất chỉnh sửa. Hệ thống lưu thay đổi và quay lại màn hình danh sách Supporter Group.
{% endstep %}
{% endstepper %}

### Xóa Supporter Group

{% stepper %}
{% step %}
## Chọn Action → Delete

Người dùng chọn **Action → Delete** tại nhóm cần xóa trên màn hình **Supporter Group List**. Hệ thống hiển thị popup xác nhận xóa nhóm.
{% endstep %}

{% step %}
## Xác nhận xóa

Người dùng chọn **Yes** tại popup xác nhận. Hệ thống xóa Supporter Group khỏi danh sách nếu người dùng có quyền xóa.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền tương ứng để xem, tạo, chỉnh sửa hoặc xóa Supporter Group.
2. Supporter Group được xác định theo tổ hợp **Department + Program + Subject**; không thể tạo 2 nhóm trùng đồng thời cả 3 thông tin (ví dụ: không thể cùng lúc tồn tại 2 nhóm CFA Level I thuộc đội SX).
3. Các thành viên trong cùng nhóm dùng chung **Display Name** và **Group Avatar** khi trả lời bình luận trên LMS học viên.
4. Thành viên được thêm vào nhóm sẽ được tự động thêm vào các lớp gắn với khóa học có **Program** và **Subject** tương ứng (mỗi khóa học chỉ thêm vào 1 lớp duy nhất); thời hạn học được gia hạn liên tục mỗi năm một lần.
5. Tài khoản được thêm vào nhóm phải là tài khoản học viên có **Staff Account / Test Account = Yes**.
6. Không được thêm cùng một tài khoản vào các nhóm có cùng **Program** và **Subject**.
7. Khi xóa thành viên khỏi nhóm: tài khoản không còn dùng Display Name/Group Avatar chung và bị xóa khỏi các lớp thuộc Program/Subject đã thêm trước đó.
8. Khi xóa Supporter Group: toàn bộ thành viên không còn dùng thông tin hiển thị chung và bị xóa khỏi các lớp thuộc Program/Subject tương ứng.

### Quy tắc tạo Supporter Group

| Quy tắc          | Mô tả                                                                                       |
| ---------------- | ------------------------------------------------------------------------------------------- |
| Group Name       | Tên nhóm hỗ trợ, dùng để quản lý trên hệ thống Operations.                                  |
| Display Name     | Tên hiển thị chung trên giao diện LMS học viên khi thành viên trong nhóm trả lời bình luận. |
| Group Avatar     | Ảnh đại diện chung khi thành viên trong nhóm trả lời bình luận.                             |
| Department       | Phòng ban phụ trách, ví dụ CX hoặc SX.                                                      |
| Program          | Chương trình học nhóm phụ trách.                                                            |
| Subject          | Môn học nhóm phụ trách.                                                                     |
| Không trùng nhóm | Không được tạo 2 nhóm có cùng Department, Program và Subject.                               |

### Quy tắc thêm thành viên vào nhóm

| Quy tắc                     | Mô tả                                                                                 |
| --------------------------- | ------------------------------------------------------------------------------------- |
| Điều kiện tài khoản         | Chỉ hiển thị tài khoản học viên được đánh dấu **Staff Account / Test Account = Yes**. |
| Chọn nhiều thành viên       | Người dùng có thể chọn nhiều tài khoản trong một lần thêm.                            |
| Không trùng Program/Subject | Không được thêm cùng một tài khoản vào các nhóm có cùng Program và Subject.           |
| Tự động thêm vào lớp        | Thành viên được thêm vào các lớp gắn với khóa học có Program và Subject tương ứng.    |
| Thời hạn học                | Tài khoản hỗ trợ trong lớp được gia hạn liên tục mỗi năm một lần.                     |

### Quy tắc chỉnh sửa Supporter Group

| Trường hợp              | Quy tắc                                                                                        |
| ----------------------- | ---------------------------------------------------------------------------------------------- |
| Nhóm chưa có thành viên | Người dùng được chỉnh sửa toàn bộ thông tin nhóm.                                              |
| Nhóm đã có thành viên   | Chỉ được chỉnh sửa Group Avatar, Group Name và Display Name.                                   |
| Thêm thành viên         | Có thể thêm thành viên tại tab Supporters nếu tài khoản đủ điều kiện.                          |
| Xóa thành viên          | Thành viên bị xóa khỏi nhóm và bị xóa khỏi các lớp đã được thêm theo Program/Subject của nhóm. |

### Quy tắc xóa Supporter Group

| Quy tắc          | Mô tả                                                                               |
| ---------------- | ----------------------------------------------------------------------------------- |
| Điều kiện xóa    | Người dùng cần có quyền xóa Supporter Group.                                        |
| Xác nhận xóa     | Hệ thống hiển thị popup xác nhận trước khi xóa.                                     |
| Sau khi xóa nhóm | Toàn bộ thành viên không còn dùng Display Name/Group Avatar chung khi bình luận.    |
| Sau khi xóa nhóm | Toàn bộ thành viên bị xóa khỏi các lớp thuộc Program/Subject đã được thêm trước đó. |

### Mẹo sử dụng

1. Nên đặt Group Name theo cấu trúc dễ nhận diện, ví dụ: "SX - CFA Level I" hoặc "CX - ACCA FR".
2. Display Name nên ngắn gọn, rõ vai trò hỗ trợ để học viên dễ nhận biết khi nhận phản hồi.
3. Trước khi tạo nhóm mới, nên tìm kiếm theo Department, Program và Subject để tránh tạo trùng.
4. Trước khi thêm thành viên, cần kiểm tra tài khoản đã được đánh dấu Staff Account/Test Account hay chưa.
5. Không nên thêm một tài khoản vào nhiều nhóm có cùng Program và Subject để tránh xung đột phạm vi hỗ trợ.
6. Trước khi xóa thành viên hoặc xóa nhóm, cần kiểm tra tác động vì tài khoản sẽ bị xóa khỏi các lớp tương ứng.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                                     | Nguyên nhân                                                            | Cách xử lý                                                                  |
| ---------------------------------------------------- | ---------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| Không thấy menu Comments/Supporter Group List        | Tài khoản chưa có quyền truy cập chức năng                             | Liên hệ Admin để kiểm tra phân quyền                                        |
| Không tạo được Supporter Group                       | Nhóm bị trùng Department, Program và Subject với nhóm đã tồn tại       | Kiểm tra nhóm hiện có và chọn lại thông tin khác                            |
| Không thấy tài khoản cần thêm vào nhóm               | Tài khoản chưa được đánh dấu Staff Account/Test Account = Yes          | Cập nhật thông tin tài khoản trước khi thêm vào nhóm                        |
| Không thêm được thành viên                           | Tài khoản đã thuộc nhóm khác có cùng Program và Subject                | Kiểm tra nhóm hiện tại của tài khoản                                        |
| Không chỉnh sửa được Program/Subject/Department      | Nhóm đã có thành viên nên các trường này bị khóa                       | Xóa thành viên trước nếu cần thay đổi phạm vi nhóm theo quy trình được phép |
| Thành viên không hiển thị tên/ảnh nhóm khi bình luận | Tài khoản chưa được thêm đúng nhóm hoặc đã bị xóa khỏi nhóm            | Kiểm tra lại danh sách thành viên trong Supporter Group                     |
| Thành viên không được thêm vào lớp tương ứng         | Program/Subject của nhóm chưa khớp khóa học hoặc hệ thống chưa đồng bộ | Kiểm tra Program/Subject và liên hệ Admin/IT nếu cần                        |
| Không xóa được nhóm                                  | Tài khoản không có quyền xóa                                           | Kiểm tra phân quyền người dùng                                              |
