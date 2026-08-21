# Lịch phòng học (Classroom Calendar)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 29, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Thông tin chung

**Dành cho:** Admin, CX/Admin cơ sở

**Đường dẫn:** Department Operations → Share Services → Classroom Booking

#### Phạm vi & Module liên quan

* **Module chính:** Operation
* **Chức năng chính:** Classroom Calendar
* **Module liên quan:** Classroom List, Facility, Classroom Booking, Class Calendar, Holiday Schedules

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập chức năng **Classroom Calendar** và quyền xem lịch phòng học.
* Với thao tác tạo, chỉnh sửa hoặc xóa lịch thuê: tài khoản cần có quyền tương ứng.

Giao diện Calendar chỉ hiển thị lịch của **từng phòng học** — cần chọn **Room** để xem lịch phòng mong muốn. Các loại lịch hiển thị: **lịch nghỉ lễ**, **lịch thuê**, **lịch học**. Chức năng này chỉ cho phép tạo/sửa/xóa **lịch thuê**; lịch học và lịch nghỉ lễ chỉ để xem.

## II. Hướng dẫn chi tiết

### Xem lịch phòng học

{% stepper %}
{% step %}
## Mở màn hình Classroom Calendar

Người dùng chọn **Classroom Booking** tại menu **Department Operations**.

![](<.gitbook/assets/image (660)>)

Hệ thống hiển thị màn hình **Classroom Calendar** ở chế độ **Month**.

![](<.gitbook/assets/image (662)>)
{% endstep %}

{% step %}
## Chọn điều kiện tìm kiếm

Người dùng chọn điều kiện tại vùng bộ lọc (**Mode, Facility, Room**).

![](<.gitbook/assets/image (665)>)
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị lịch của phòng học được chọn.
{% endstep %}

{% step %}
## Chọn Reset (nếu cần)

Người dùng chọn **Reset** nếu muốn xóa điều kiện tìm kiếm. Hệ thống xóa toàn bộ điều kiện lọc đã nhập.
{% endstep %}
{% endstepper %}

### Chuyển chế độ xem lịch

{% stepper %}
{% step %}
## Xem theo tháng (Month)

Người dùng chọn **Month** nếu muốn xem lịch theo tháng (chế độ mặc định).

![](<.gitbook/assets/image (666)>)
{% endstep %}

{% step %}
## Xem theo tuần (Week)

Người dùng chọn **Week** nếu muốn xem lịch theo tuần.

![](<.gitbook/assets/image (669)>)
{% endstep %}

{% step %}
## Chuyển tuần/tháng trước-sau

Người dùng chọn nút chuyển trước/sau nếu muốn xem tuần/tháng khác.

![](<.gitbook/assets/image (670)>)
{% endstep %}

{% step %}
## Quay về ngày hiện tại (Today)

Người dùng chọn **Today** nếu muốn quay về ngày hiện tại. Hệ thống hiển thị lịch tại thời điểm hiện tại.
{% endstep %}
{% endstepper %}

### Xem danh sách đầy đủ sự kiện trong ngày

{% stepper %}
{% step %}
## Di chuột vào +x more

Người dùng di chuột vào **+x more** tại ngày có nhiều sự kiện trên màn hình **Classroom Calendar**.

![](<.gitbook/assets/image (672)>)

Hệ thống hiển thị danh sách đầy đủ các sự kiện trong ngày đó.
{% endstep %}
{% endstepper %}

### Xem chi tiết lịch phòng học

{% stepper %}
{% step %}
## Tìm kiếm lịch phòng học

Người dùng tìm kiếm lịch phòng học tại màn hình **Classroom Calendar**. Hệ thống hiển thị lịch theo phòng học được chọn.
{% endstep %}

{% step %}
## Nhấp vào sự kiện cần xem

Người dùng nhấp vào sự kiện cần xem trên lịch.

![](<.gitbook/assets/image (674)>)

Hệ thống hiển thị thông tin chi tiết của sự kiện.
{% endstep %}

{% step %}
## Kiểm tra thông tin chi tiết

Người dùng kiểm tra thông tin chi tiết.

![](<.gitbook/assets/image (676)>)

_Lịch nghỉ lễ_

![](<.gitbook/assets/image (678)>)

_Lịch học_

![](<.gitbook/assets/image (679)>)

_Lịch thuê_

Thông tin hiển thị khác nhau theo loại lịch: lịch nghỉ lễ, lịch học hoặc lịch thuê.
{% endstep %}
{% endstepper %}

### Tạo mới lịch thuê phòng học

{% stepper %}
{% step %}
## Chọn Add Event

Người dùng chọn **Add Event** tại màn hình **Classroom Calendar**.

![](<.gitbook/assets/image (681)>)

Hệ thống mở màn hình **Add Event**.

![](<.gitbook/assets/image (682)>)

Nếu đang xem lịch của một phòng học cụ thể, hệ thống tự điền phòng học đó tại trường **Classroom**.
{% endstep %}

{% step %}
## Nhập Event Name

Người dùng nhập **Event Name** tại màn hình **Add Event**.
{% endstep %}

{% step %}
## Kiểm tra Event Type

Hệ thống hiển thị giá trị ban đầu là **Lịch cho thuê**; người dùng có thể chuyển sang loại khác là **Lịch Inactive**.

![](<.gitbook/assets/image (684)>)
{% endstep %}

{% step %}
## Nhập/chọn Lessee

Người dùng nhập text để thêm mới bên thuê hoặc chọn một giá trị đã lưu tại trường **Lessee**.

![](<.gitbook/assets/image (686)>)
{% endstep %}

{% step %}
## Chọn Time

Người dùng chọn Start Date và End Date của lịch thuê tại trường **Time**.

![](<.gitbook/assets/image (688)>)
{% endstep %}

{% step %}
## Chọn Repeat

Người dùng chọn một trong các giá trị lặp lại do hệ thống hỗ trợ tại trường **Repeat**.

![](<.gitbook/assets/image (690)>)
{% endstep %}

{% step %}
## Chọn End on (nếu Repeat khác Does not repeat)

Người dùng chọn **End on**. Ngày kết thúc lịch lặp tối đa là 2 năm kể từ Start Date.

![](<.gitbook/assets/image (691)>)
{% endstep %}

{% step %}
## Chọn Classroom (nếu chưa tự điền)

Người dùng chọn **Classroom** nếu hệ thống chưa tự điền.

![](<.gitbook/assets/image (693)>)
{% endstep %}

{% step %}
## Nhập Description và Save

Người dùng nhập **Description** nếu cần, sau đó chọn **Save**. Hệ thống lưu lịch thuê và hiển thị sự kiện trên Calendar nếu thông tin hợp lệ.
{% endstep %}
{% endstepper %}

### Chỉnh sửa lịch thuê phòng học

{% stepper %}
{% step %}
## Mở chi tiết lịch thuê

Người dùng nhấp vào lịch thuê cần chỉnh sửa trên màn hình **Classroom Calendar**. Hệ thống hiển thị thông tin chi tiết lịch thuê.
{% endstep %}

{% step %}
## Chọn Edit Event

Người dùng chọn **Edit Event** tại màn hình chi tiết lịch thuê.

![](<.gitbook/assets/image (695)>)

Hệ thống mở màn hình **Edit Event**.

![](<.gitbook/assets/image (697)>)
{% endstep %}

{% step %}
## Chỉnh sửa thông tin

Người dùng chỉnh sửa **Event Name, Time, Repeat** và **Description**. (Không sửa được Event Type và Lessee.)
{% endstep %}

{% step %}
## Chọn phạm vi chỉnh sửa (nếu lịch lặp)

Người dùng có thể chọn **This event** hoặc **This and following events** tùy loại thông tin cần chỉnh sửa.
{% endstep %}

{% step %}
## Chọn Save

Người dùng chọn **Save** tại màn hình **Edit Event**. Hệ thống kiểm tra trùng lịch và lưu thông tin nếu dữ liệu hợp lệ.
{% endstep %}
{% endstepper %}

### Xóa lịch thuê phòng học

{% stepper %}
{% step %}
## Mở chi tiết lịch thuê

Người dùng nhấp vào lịch thuê cần xóa trên màn hình **Classroom Calendar**. Hệ thống hiển thị thông tin chi tiết lịch thuê.
{% endstep %}

{% step %}
## Chọn Delete

Người dùng chọn **Delete** tại màn hình chi tiết lịch thuê.

![](<.gitbook/assets/image (698)>)

Hệ thống hiển thị popup xác nhận xóa.

![](<.gitbook/assets/image (700)>)
{% endstep %}

{% step %}
## Chọn phạm vi xóa (nếu lịch lặp)

Với lịch lặp, người dùng có thể chọn **This event** hoặc **This and following events**.
{% endstep %}

{% step %}
## Xác nhận xóa

Người dùng chọn **Yes** để xác nhận xóa lịch (hệ thống xóa theo phạm vi đã chọn); chọn **No** để giữ nguyên lịch thuê.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Giao diện Calendar chỉ hiển thị lịch của từng phòng học, vì vậy cần chọn **Room** để xem lịch phòng mong muốn.
2. Lịch nghỉ lễ và lịch học chỉ cho phép xem chi tiết, không chỉnh sửa/xóa tại Classroom Calendar.
3. Khi tạo lịch thuê, **Event Type** mặc định là **Lịch thuê**.
4. Khi chỉnh sửa lịch thuê, không được chỉnh sửa **Event Type** và **Lessee**.
5. Chỉ được chỉnh sửa hoặc xóa lịch thuê khi phòng học có trạng thái **Active**.
6. Khi tạo/chỉnh sửa thời gian lịch thuê, hệ thống kiểm tra trùng lịch với các lịch đã tồn tại trong cùng phòng học; nếu trùng, hệ thống báo lỗi và không lưu.

### Quy tắc Repeat khi tạo lịch thuê

| Giá trị Repeat                 | Mô tả                                   |
| ------------------------------ | --------------------------------------- |
| Does not repeat                | Không lặp lại. Đây là giá trị mặc định. |
| Daily                          | Lặp lại hằng ngày.                      |
| Every weekday Monday to Friday | Lặp lại từ thứ 2 đến thứ 6.             |
| Custom                         | Người dùng tự cấu hình chu kỳ lặp.      |

### Quy tắc Custom Repeat

| Trường               | Quy tắc                                                                                                               |
| -------------------- | --------------------------------------------------------------------------------------------------------------------- |
| Repeat every - Day   | Nhập số nguyên dương từ 1 đến 31.                                                                                     |
| Repeat every - Week  | Nhập số nguyên dương từ 1 đến 52.                                                                                     |
| Repeat every - Month | Nhập số nguyên dương từ 1 đến 12.                                                                                     |
| Repeat every - Years | Nhập số nguyên dương từ 1 đến 2.                                                                                      |
| Repeat on            | Hiển thị khi Repeat Every = Week. Mặc định là thứ của Start Date, có thể chọn thêm Mon, Tue, Wed, Thu, Fri, Sat, Sun. |
| End on               | Hiển thị khi Repeat khác Does not repeat. Ngày kết thúc tối đa 2 năm kể từ Start Date.                                |

### Quy tắc chỉnh sửa lịch thuê không lặp

| Thao tác                                     | Quy tắc                                                            |
| -------------------------------------------- | ------------------------------------------------------------------ |
| Sửa Event Name                               | Người dùng chỉnh sửa và chọn Save để lưu.                          |
| Sửa Description                              | Người dùng chỉnh sửa và chọn Save để lưu.                          |
| Sửa Time                                     | Hệ thống kiểm tra trùng lịch trước khi lưu.                        |
| Sửa Repeat từ Does not repeat sang loại khác | Hệ thống kiểm tra trùng lịch cho các lịch lặp mới trước khi lưu.   |
| Nếu trùng lịch                               | Hệ thống hiển thị thông báo trùng lịch và không lưu thông tin mới. |
| Nếu không trùng lịch                         | Hệ thống lưu thông tin thành công.                                 |

### Quy tắc chỉnh sửa lịch thuê có lặp

| Thao tác                                     | Quy tắc                                                                                                                               |
| -------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------- |
| Sửa Event Name / Description                 | Có thể chọn áp dụng cho **This event** hoặc **This and following events**.                                                            |
| Sửa Time cho This event                      | Hệ thống kiểm tra trùng lịch cho event đang chọn.                                                                                     |
| Sửa Time cho This and following events       | Hệ thống kiểm tra trùng lịch cho event đang chọn và các event lặp phía sau.                                                           |
| Đổi Repeat sang Does not repeat              | Mặc định áp dụng **This and following events** và không cho phép thay đổi. Hệ thống xóa các lịch lặp phía sau tính từ lịch đang chọn. |
| Đổi từ một loại Repeat sang loại Repeat khác | Mặc định áp dụng **This and following events** và không cho phép thay đổi. Hệ thống kiểm tra trùng lịch trước khi lưu.                |
| Nếu trùng ≤ 3 lịch                           | Hệ thống hiển thị thông báo trùng lịch và liệt kê các lịch trùng. Thông tin mới không được lưu.                                       |
| Nếu trùng > 3 lịch                           | Hệ thống hiển thị thông báo trùng lịch. Thông tin mới không được lưu.                                                                 |
| Nếu không trùng lịch                         | Hệ thống lưu thông tin thành công.                                                                                                    |

### Quy tắc xóa lịch thuê

| Trường hợp                | Quy tắc                                        |
| ------------------------- | ---------------------------------------------- |
| Lịch thuê không lặp       | Hệ thống hiển thị popup xác nhận xóa.          |
| Người dùng chọn Yes       | Hệ thống xóa lịch thuê.                        |
| Người dùng chọn No        | Hệ thống giữ nguyên lịch thuê.                 |
| Lịch thuê có lặp          | Hệ thống cho phép chọn phạm vi xóa.            |
| This event                | Chỉ xóa event đang chọn.                       |
| This and following events | Xóa event đang chọn và các event lặp phía sau. |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống            | Nguyên nhân                                                  | Cách xử lý                                  |
| --------------------------- | ------------------------------------------------------------ | ------------------------------------------- |
| Không thấy lịch phòng học   | Chưa chọn Room hoặc bộ lọc chưa đúng                         | Chọn Room và bấm Search                     |
| Không tạo được lịch thuê    | Thiếu trường bắt buộc hoặc tài khoản không có quyền          | Kiểm tra các trường có dấu \* và phân quyền |
| Không chỉnh sửa được lịch   | Event không phải Lịch thuê hoặc phòng học không Active       | Kiểm tra Event Type và trạng thái phòng học |
| Không chỉnh sửa được Lessee | Lessee không được phép chỉnh sửa sau khi tạo lịch            | Tạo lịch thuê mới nếu cần đổi bên thuê      |
| Không lưu được Time mới     | Thời gian mới bị trùng lịch phòng học                        | Chọn thời gian khác hoặc phòng học khác     |
| Không xóa được lịch         | Event không phải Lịch thuê hoặc tài khoản không có quyền xóa | Kiểm tra Event Type và quyền người dùng     |
| Repeat Custom bị lỗi        | Giá trị Repeat every không nằm trong khoảng cho phép         | Nhập lại số nguyên dương theo đúng giới hạn |
| Lịch lặp tạo ra quá dài     | End on vượt quá giới hạn cho phép                            | Chọn End on tối đa 2 năm kể từ Start Date   |
