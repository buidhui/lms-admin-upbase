# Quản lý lịch nghỉ lễ (Holiday Schedules)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version | Effective Date |
| -------------- | ------------- | ----- | ------------------------------ | ------- | -------------- |
| May 28, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   | May 18, 2026   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, CX Admin

**Đường dẫn:** Department Operations → Customer Experience → Holiday Schedules
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Operation
* **Chức năng chính:** Holiday Schedules
* **Màn hình liên quan:** Import Report
* **Module liên quan:** Class, Calendar, Learning Schedule, Program, Import Log
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản có quyền truy cập menu **Customer Experience → Holiday Schedules**.
* Tài khoản có quyền tạo lịch nghỉ lễ bằng file import.
{% endhint %}

{% hint style="info" %}
Theo thay đổi hiện tại, người dùng cần chọn **Program** trước khi import file. Các ngày nghỉ lễ trong file sẽ được áp dụng cho **Program đã chọn**, thay vì áp dụng chung cho toàn bộ Program.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách file import lịch nghỉ lễ</summary>

{% stepper %}
{% step %}
**Mở màn hình Import Report**

Người dùng chọn **Holiday Schedules** tại menu **Customer Experience**. Hệ thống mở màn hình **Import Report**.

<figure><img src="../.gitbook/assets/image (760).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem danh sách file import**

Người dùng xem danh sách file import tại bảng **Import Report**. Hệ thống hiển thị các thông tin: Program, Import file, Importer, Date và Status của từng file.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tìm kiếm/lọc file import</summary>

{% stepper %}
{% step %}
**Nhập/chọn điều kiện tìm kiếm**

Người dùng nhập hoặc chọn điều kiện tại vùng tìm kiếm của màn hình **Import Report** (Search, Status hoặc Program).

<figure><img src="../.gitbook/assets/image (761).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Search**

Người dùng chọn **Search**. Hệ thống hiển thị danh sách file import thỏa mãn điều kiện tìm kiếm.
{% endstep %}

{% step %}
**Chọn Reset**

Người dùng chọn **Reset** nếu muốn xóa điều kiện. Hệ thống hiển thị lại danh sách file import theo trạng thái mặc định.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo lịch nghỉ lễ bằng file import</summary>

{% stepper %}
{% step %}
**Chọn Create Holiday Schedule**

Người dùng chọn **Create Holiday Schedule** tại màn hình **Import Report**.

<figure><img src="../.gitbook/assets/image (762).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị popup **Create Holiday Schedule**.

<figure><img src="../.gitbook/assets/image (763).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Program**

Người dùng chọn **Program** tại popup. Đây là Program sẽ được áp dụng lịch nghỉ lễ trong file import. (Trường bắt buộc)
{% endstep %}

{% step %}
**Chọn file để import**

Người dùng chọn **Browse** hoặc kéo thả file vào vùng upload. Hệ thống chỉ hỗ trợ file định dạng **CSV** hoặc **XLSX**.
{% endstep %}

{% step %}
**Chọn đúng file lịch nghỉ lễ**

Người dùng chọn đúng file cần import từ thiết bị. Mỗi lần tạo lịch nghỉ lễ, chỉ nên chọn file đúng template hệ thống cung cấp.
{% endstep %}

{% step %}
**Chọn Create**

Người dùng chọn **Create** tại popup. Hệ thống upload file và xử lý dữ liệu lịch nghỉ lễ cho Program đã chọn.
{% endstep %}

{% step %}
**Xem kết quả import**

Hệ thống hiển thị kết quả import: tên file, số lượng dữ liệu, số dòng thành công và số dòng lỗi nếu có.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tải file mẫu lịch nghỉ lễ</summary>

{% stepper %}
{% step %}
**Chọn Create Holiday Schedule**

Người dùng chọn **Create Holiday Schedule** tại màn hình **Import Report**. Hệ thống hiển thị popup **Create Holiday Schedule**.
{% endstep %}

{% step %}
**Chọn link file mẫu**

Người dùng chọn link **filemau.xlsx** tại popup.

<figure><img src="../.gitbook/assets/image (764).png" alt=""><figcaption></figcaption></figure>

Hệ thống tải file mẫu về thiết bị.

<figure><img src="../.gitbook/assets/image (765).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập dữ liệu vào file mẫu**

Người dùng nhập dữ liệu lịch nghỉ lễ vào file mẫu theo đúng cấu trúc hệ thống cung cấp.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết kết quả import sau khi tạo lịch nghỉ lễ</summary>

{% stepper %}
{% step %}
**Chọn View Log**

Người dùng chọn **View Log** tại màn hình kết quả import sau khi upload file. Hệ thống mở màn hình **Import Detail**.

<figure><img src="../.gitbook/assets/image (766).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Kiểm tra các dòng dữ liệu**

Người dùng kiểm tra các dòng dữ liệu tại màn hình **Import Detail**.

<figure><img src="../.gitbook/assets/image (767).png" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị Name, Start date, End date, Note và Errors nếu có.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem chi tiết kết quả import từ Import Report</summary>

{% stepper %}
{% step %}
**Mở màn hình Import Report**

Người dùng mở màn hình **Import Report** trong chức năng **Holiday Schedules**.
{% endstep %}

{% step %}
**Chọn Action → Detail**

Người dùng chọn **Action → Detail** tại file import cần kiểm tra.

<figure><img src="../.gitbook/assets/image (768).png" alt=""><figcaption></figcaption></figure>

Hệ thống mở màn hình **Import Detail**.
{% endstep %}

{% step %}
**Kiểm tra chi tiết dữ liệu**

Người dùng kiểm tra thông tin chi tiết các dòng dữ liệu trong file import. Nếu dòng dữ liệu lỗi, hệ thống hiển thị nguyên nhân lỗi tại cột **Errors**.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần có quyền import lịch nghỉ lễ để sử dụng chức năng này.
2. Mỗi lần import, cần chọn **Program** trước khi upload file; lịch nghỉ lễ trong file sẽ được áp dụng cho **Program đã chọn**.
3. Nếu cần áp dụng cùng một lịch nghỉ lễ cho nhiều Program, có thể chọn nhiều Program khi import.
4. File import chỉ hỗ trợ định dạng **CSV** hoặc **XLSX**.
5. File trạng thái **Successful**: toàn bộ ngày nghỉ lễ trong file được tạo thành công.
6. File trạng thái **Failed**: có ít nhất một ngày nghỉ lễ trong file không được tạo thành công.
7. Cần vào **Import Detail** để kiểm tra lỗi cụ thể tại cột **Errors**.
8. Chức năng này không hỗ trợ tạo/chỉnh sửa/xóa từng ngày nghỉ lễ trực tiếp trên giao diện.
{% endhint %}

### Quy tắc file import

<table data-search="false"><thead><tr><th>Quy tắc</th><th>Mô tả</th></tr></thead><tbody><tr><td>Định dạng file</td><td>Chỉ hỗ trợ <strong>CSV</strong> hoặc <strong>XLSX</strong>.</td></tr><tr><td>Template</td><td>Nên sử dụng file mẫu do hệ thống cung cấp.</td></tr><tr><td>Program</td><td>Bắt buộc chọn trước khi import.</td></tr><tr><td>Phạm vi áp dụng</td><td>Lịch nghỉ lễ chỉ áp dụng cho Program được chọn.</td></tr><tr><td>Tên sự kiện</td><td>Cần nhập rõ ràng, đúng chính tả để dễ nhận diện trên lịch.</td></tr><tr><td>Start date</td><td>Ngày bắt đầu sự kiện/ngày nghỉ lễ.</td></tr><tr><td>End date</td><td>Ngày kết thúc sự kiện/ngày nghỉ lễ.</td></tr><tr><td>Note</td><td>Ghi chú bổ sung nếu có.</td></tr><tr><td>Dữ liệu lỗi</td><td>Được hiển thị tại cột Errors trong Import Detail.</td></tr></tbody></table>

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
