# Quản lý lịch nghỉ lễ (Holiday Schedules)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version | Effective Date |
| -------------- | ------------- | ----- | ------------------------------ | ------- | -------------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   | May 18, 2026   |

## I. Thông tin chung

**Dành cho:** Admin, CX Admin

**Đường dẫn:** Department Operations → Customer Experience → Holiday Schedules

#### Phạm vi & Module liên quan

* **Module chính:** Operation
* **Chức năng chính:** Holiday Schedules
* **Màn hình liên quan:** Import Report
* **Module liên quan:** Class, Calendar, Learning Schedule, Program, Import Log

#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập menu **Customer Experience → Holiday Schedules**.
* Tài khoản có quyền tạo lịch nghỉ lễ bằng file import.

{% hint style="info" %}
Theo thay đổi hiện tại, người dùng cần chọn **Program** trước khi import file. Các ngày nghỉ lễ trong file sẽ được áp dụng cho **Program đã chọn**, thay vì áp dụng chung cho toàn bộ Program.
{% endhint %}

## II. Hướng dẫn chi tiết

### Xem danh sách file import lịch nghỉ lễ

{% stepper %}
{% step %}
## Mở màn hình Import Report

Người dùng chọn **Holiday Schedules** tại menu **Customer Experience**. Hệ thống mở màn hình **Import Report**.

![](<../.gitbook/assets/image (284)>)
{% endstep %}

{% step %}
## Xem danh sách file import

Người dùng xem danh sách file import tại bảng **Import Report**. Hệ thống hiển thị các thông tin: Program, Import file, Importer, Date và Status của từng file.
{% endstep %}
{% endstepper %}

### Tìm kiếm/lọc file import

{% stepper %}
{% step %}
## Nhập/chọn điều kiện tìm kiếm

Người dùng nhập hoặc chọn điều kiện tại vùng tìm kiếm của màn hình **Import Report** (Search, Status hoặc Program).

![](<../.gitbook/assets/image (285)>)
{% endstep %}

{% step %}
## Chọn Search

Người dùng chọn **Search**. Hệ thống hiển thị danh sách file import thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
## Chọn Reset

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại danh sách file import theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

### Tạo lịch nghỉ lễ bằng file import

{% stepper %}
{% step %}
## Chọn Create Holiday Schedule

Người dùng chọn **Create Holiday Schedule** tại màn hình **Import Report**.

![](<../.gitbook/assets/image (286)>)

Hệ thống hiển thị popup **Create Holiday Schedule**.

![](<../.gitbook/assets/image (287)>)
{% endstep %}

{% step %}
## Chọn Program

Người dùng chọn **Program** tại popup. Đây là Program sẽ được áp dụng lịch nghỉ lễ trong file import. (Trường bắt buộc)
{% endstep %}

{% step %}
## Chọn file để import

Người dùng chọn **Browse** hoặc kéo thả file vào vùng upload. Hệ thống chỉ hỗ trợ file định dạng **CSV** hoặc **XLSX**.
{% endstep %}

{% step %}
## Chọn đúng file lịch nghỉ lễ

Người dùng chọn đúng file cần import từ thiết bị. Mỗi lần tạo lịch nghỉ lễ, chỉ nên chọn file đúng template hệ thống cung cấp.
{% endstep %}

{% step %}
## Chọn Create

Người dùng chọn **Create** tại popup. Hệ thống upload file và xử lý dữ liệu lịch nghỉ lễ cho Program đã chọn.
{% endstep %}

{% step %}
## Xem kết quả import

Hệ thống hiển thị kết quả import: tên file, số lượng dữ liệu, số dòng thành công và số dòng lỗi nếu có.
{% endstep %}
{% endstepper %}

### Tải file mẫu lịch nghỉ lễ

{% stepper %}
{% step %}
## Chọn Create Holiday Schedule

Người dùng chọn **Create Holiday Schedule** tại màn hình **Import Report**. Hệ thống hiển thị popup **Create Holiday Schedule**.
{% endstep %}

{% step %}
## Chọn link file mẫu

Người dùng chọn link **filemau.xlsx** tại popup.

![](<../.gitbook/assets/image (288)>)

Hệ thống tải file mẫu về thiết bị.

![](<../.gitbook/assets/image (289)>)
{% endstep %}

{% step %}
## Nhập dữ liệu vào file mẫu

Người dùng nhập dữ liệu lịch nghỉ lễ vào file mẫu theo đúng cấu trúc hệ thống cung cấp.
{% endstep %}
{% endstepper %}

### Xem chi tiết kết quả import sau khi tạo lịch nghỉ lễ

{% stepper %}
{% step %}
## Chọn View Log

Người dùng chọn **View Log** tại màn hình kết quả import sau khi upload file. Hệ thống mở màn hình **Import Detail**.

![](<../.gitbook/assets/image (290)>)
{% endstep %}

{% step %}
## Kiểm tra các dòng dữ liệu

Người dùng kiểm tra các dòng dữ liệu tại màn hình **Import Detail**.

![](<../.gitbook/assets/image (291)>)

Hệ thống hiển thị Name, Start date, End date, Note và Errors nếu có.
{% endstep %}
{% endstepper %}

### Xem chi tiết kết quả import từ Import Report

{% stepper %}
{% step %}
## Mở màn hình Import Report

Người dùng mở màn hình **Import Report** trong chức năng **Holiday Schedules**.
{% endstep %}

{% step %}
## Chọn Action → Detail

Người dùng chọn **Action → Detail** tại file import cần kiểm tra.

![](<../.gitbook/assets/image (292)>)

Hệ thống mở màn hình **Import Detail**.
{% endstep %}

{% step %}
## Kiểm tra chi tiết dữ liệu

Người dùng kiểm tra thông tin chi tiết các dòng dữ liệu trong file import. Nếu dòng dữ liệu lỗi, hệ thống hiển thị nguyên nhân lỗi tại cột **Errors**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

1. Người dùng cần có quyền import lịch nghỉ lễ để sử dụng chức năng này.
2. Mỗi lần import, cần chọn **Program** trước khi upload file; lịch nghỉ lễ trong file sẽ được áp dụng cho **Program đã chọn**.
3. Nếu cần áp dụng cùng một lịch nghỉ lễ cho nhiều Program, có thể chọn nhiều Program khi import.
4. File import chỉ hỗ trợ định dạng **CSV** hoặc **XLSX**.
5. File trạng thái **Successful**: toàn bộ ngày nghỉ lễ trong file được tạo thành công.
6. File trạng thái **Failed**: có ít nhất một ngày nghỉ lễ trong file không được tạo thành công.
7. Cần vào **Import Detail** để kiểm tra lỗi cụ thể tại cột **Errors**.
8. Chức năng này không hỗ trợ tạo/chỉnh sửa/xóa từng ngày nghỉ lễ trực tiếp trên giao diện.

### Quy tắc file import

| Quy tắc         | Mô tả                                                      |
| --------------- | ---------------------------------------------------------- |
| Định dạng file  | Chỉ hỗ trợ **CSV** hoặc **XLSX**.                          |
| Template        | Nên sử dụng file mẫu do hệ thống cung cấp.                 |
| Program         | Bắt buộc chọn trước khi import.                            |
| Phạm vi áp dụng | Lịch nghỉ lễ chỉ áp dụng cho Program được chọn.            |
| Tên sự kiện     | Cần nhập rõ ràng, đúng chính tả để dễ nhận diện trên lịch. |
| Start date      | Ngày bắt đầu sự kiện/ngày nghỉ lễ.                         |
| End date        | Ngày kết thúc sự kiện/ngày nghỉ lễ.                        |
| Note            | Ghi chú bổ sung nếu có.                                    |
| Dữ liệu lỗi     | Được hiển thị tại cột Errors trong Import Detail.          |

### Quy tắc trạng thái import

| Trạng thái    | Quy tắc                                                          |
| ------------- | ---------------------------------------------------------------- |
| Successful    | Toàn bộ dòng dữ liệu trong file hợp lệ và được tạo thành công.   |
| Failed        | Có ít nhất một dòng dữ liệu lỗi hoặc không được tạo thành công.  |
| Import Detail | Dùng để kiểm tra chi tiết dữ liệu trong file và nguyên nhân lỗi. |

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                     | Nguyên nhân                                            | Cách xử lý                                                        |
| ------------------------------------ | ------------------------------------------------------ | ----------------------------------------------------------------- |
| Không tạo được lịch nghỉ lễ          | Chưa chọn **Program** trước khi import                 | Chọn Program (trường bắt buộc) trước khi upload file              |
| Không chọn được file để import       | File sai định dạng (không phải CSV/XLSX)               | Dùng file định dạng CSV hoặc XLSX                                 |
| File import có trạng thái **Failed** | Có ít nhất một dòng dữ liệu lỗi/không hợp lệ           | Mở Import Detail, sửa các dòng lỗi theo cột Errors rồi import lại |
| Dữ liệu lệch/không đúng cấu trúc     | Không dùng file mẫu hệ thống cung cấp                  | Tải file mẫu (filemau.xlsx) và nhập đúng cấu trúc                 |
| Không tìm thấy file import           | Sai điều kiện tìm kiếm/lọc                             | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định        |
| Không sửa/xóa được từng ngày nghỉ lễ | Hệ thống chưa hỗ trợ thao tác trực tiếp trên giao diện | Chuẩn bị lại file đúng và import lại                              |
