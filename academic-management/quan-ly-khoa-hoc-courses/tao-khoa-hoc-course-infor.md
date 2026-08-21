---
description: >-
  Kết quả đạt được: Người dùng có thể tạo được khóa học với các thông tin chung
  của khóa.
---

# Tạo khóa học (Course Infor)

## Record of changes

_A - Add | M - Modify | D - Delete_

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 20, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới thiệu chung

{% hint style="info" %}
**Dành cho:** Admin, SX

**Đường dẫn:** [https://ops.upbase.asia/course-full/undefined](https://ops.upbase.asia/course-full/undefined)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Academic Management > Course & Materials
* **Chức năng chính:** Course 4 Level > Create Course
* **Bước thực hiện:** Course Info
* **Module liên quan:**
  * Program Category
  * Subject Category
  * Course Content
  * Resources
  * Certificates
  * Class
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống LMS Ops.
* Tài khoản người dùng có quyền tạo mới khóa học.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Truy cập màn hình tạo mới khóa học</summary>

{% stepper %}
{% step %}
**Admin truy cập Academic Management → Course & Materials → Course 4 Level**

Hệ thống hiển thị màn hình danh sách khóa học.

<figure><img src="../../.gitbook/assets/image (480)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tại màn hình danh sách khóa học, Admin chọn Create Course.**

Lúc này, hệ thống chuyển đến bước **Course Info.**

<figure><img src="../../.gitbook/assets/image (481)" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (482)" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Nhập thông tin chung của khóa học</summary>

{% stepper %}
{% step %}
**Admin cần nhập Tên khóa học (Course Name)**

Đây là trường bắt buộc dùng để hiển thị tên khóa học trên hệ thống và hiển thị cho học viên tại LMS.

<figure><img src="../../.gitbook/assets/image (483)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập mô tả khóa học (Describe)**

Trường này dùng để mô tả nội dung hoặc mục tiêu chính của khóa học.

<figure><img src="../../.gitbook/assets/image (484)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập mã khóa học (Code)**

Đây là trường bắt buộc. Hệ thống không cho phép lưu nếu mã khóa học trùng với mã đã tồn tại.

<figure><img src="../../.gitbook/assets/image (485)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập hoặc chọn Tag. Admin có thể tạo tag mới bằng cách nhập nội dung tag.**

<figure><img src="../../.gitbook/assets/image (486)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Program (Category) từ danh sách hiển thị**

Đây là trường bắt buộc, nhờ vào trường này, hệ thống mới xác định được chương trình học và từ đó cho phép admin chọn môn học tương ứng.

<figure><img src="../../.gitbook/assets/image (487)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn hoặc nhập Subject tương ứng với Program đã chọn.**

<figure><img src="../../.gitbook/assets/image (488)" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Cấu hình thông tin theo loại khóa học</summary>

{% stepper %}
{% step %}
**Admin chọn Type của khóa học**

Hệ thống hỗ trợ các loại khóa học: **Foundation Course**, **Trial Course**, **Practice Course** và **Normal Course**.

<figure><img src="../../.gitbook/assets/image (489)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập thông tin cấu hình khóa học theo từng type**

{% tabs %}
{% tab title="Foundation Course" %}
<figure><img src="../../.gitbook/assets/image (490)" alt=""><figcaption></figcaption></figure>

**Bước 2.1.** Khi Admin chọn **Foundation Course**, hệ thống hiển thị danh sách checkbox level của khóa học.

Admin cần chọn ít nhất **01 level**.

Ví dụ level có thể bao gồm các mức như IA, IB, IIA, IIB tùy theo cấu hình hệ thống.
{% endtab %}

{% tab title="Normal Course" %}
<figure><img src="../../.gitbook/assets/image (491)" alt=""><figcaption></figcaption></figure>

**Bước 2.2:** Khi Admin chọn **Normal Course**, hệ thống hiển thị danh sách combobox các khóa học **Foundation Course** theo từng level.

Admin có thể:

* Nhập ký tự để tìm kiếm khóa học Foundation đã tạo với level tương ứng.
* Chọn hoặc không chọn khóa học Foundation cho từng level.

Với Normal Course, Admin có thể không chọn khóa học Foundation nào cho cả 4 level.
{% endtab %}

{% tab title="Trial Course/ Practice Course" %}
**Bước 2.3:** Với **Trial Course** hoặc **Practice Course**, Admin chỉ cần chọn loại khóa học tương ứng và tiếp tục nhập các thông tin còn lại của Course Info.
{% endtab %}
{% endtabs %}
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Nhập Pass Point</summary>

<figure><img src="../../.gitbook/assets/image (492)" alt=""><figcaption></figcaption></figure>

Admin nhập **Pass Point**. Đây là trường bắt buộc. Pass Point là mức điểm yêu cầu mà học viên phải đạt để có thể nhận được chứng chỉ của khóa học.

</details>

<details>

<summary>Nhập điểm các thành phần</summary>

<figure><img src="../../.gitbook/assets/image (493)" alt=""><figcaption></figcaption></figure>

Admin nhập hệ số điểm cho từng thành phần:

| Thành phần       | Bắt buộc | Ghi chú                                   |
| ---------------- | -------- | ----------------------------------------- |
| **Tiến độ học**  | Y        | Nhập tỷ trọng điểm cho tiến độ học.       |
| **Graded Quiz**  | Y        | Nhập tỷ trọng điểm cho quiz có tính điểm. |
| **Chapter Test** | Y        | Nhập tỷ trọng điểm cho Chapter Test.      |
| **Topic Test**   | Y        | Nhập tỷ trọng điểm cho Topic Test.        |
| **Mid Test**     | Y        | Nhập tỷ trọng điểm cho Mid Test.          |
| **Final Test**   | Y        | Nhập tỷ trọng điểm cho Final Test.        |

Tổng hệ số điểm của tất cả thành phần phải bằng **100**.

</details>

<details>

<summary>Lưu Course Info</summary>

Admin chọn **Save**. Lúc này, hệ thống lưu thông tin đã nhập và tạo khóa học mới.

Sau khi lưu thành công, Admin có thể tiếp tục chuyển sang bước tiếp theo trong quy trình tạo khóa học.

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Course Info là bước đầu tiên trong quy trình tạo khóa học.
2. Các trường có dấu **(\*)** là trường bắt buộc.
3. **Code** là mã định danh khóa học và không được trùng với mã khóa học đã tồn tại.
4. **Program / Category** và **Subject** cần được chọn đúng để đảm bảo khóa học được phân loại chính xác.
5. **Type** là trường bắt buộc và ảnh hưởng đến các thông tin cần cấu hình tiếp theo.
6. Nếu chọn **Foundation Course**, Admin bắt buộc phải chọn ít nhất một level.
7. Nếu chọn **Normal Course**, hệ thống hiển thị danh sách Foundation Course theo từng level để Admin có thể cấu hình khóa học nền tảng đi kèm.
8. Với **Normal Course**, Admin có thể không chọn Foundation Course cho cả 4 level.
9. **Pass Point** là trường bắt buộc, dùng để xác định điều kiện điểm để học viên được nhận chứng chỉ.
10. Tổng điểm các thành phần bắt buộc phải bằng **100**.
11. Sau khi nhập đầy đủ thông tin, Admin cần chọn **Save** để lưu Course Info và tạo khóa học mới.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nên chọn đúng **Program** trước khi chọn **Subject** để đảm bảo môn học thuộc đúng chương trình
2. Với **Normal Course**, nếu cần thiết lập điều kiện học nền tảng, nên tạo sẵn các Foundation Course trước.
3. Nên kiểm tra kỹ tổng tỷ trọng điểm trước khi bấm **Save**.
4. Nếu khóa học chưa chắc chắn cấu hình điểm, nên thống nhất quy tắc tính điểm nội bộ trước khi tạo Course Info.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                               | Nguyên nhân                                              | Cách xử lý                                          |
| -------------------------------------------------------------- | -------------------------------------------------------- | --------------------------------------------------- |
| Không thấy nút Create Course                                   | Tài khoản chưa có quyền tạo khóa học                     | Liên hệ Admin hệ thống để kiểm tra phân quyền       |
| Không lưu được Course Info                                     | Thiếu trường bắt buộc                                    | Kiểm tra và nhập đầy đủ các trường có dấu **(\*)**  |
| Hệ thống báo mã khóa học đã tồn tại                            | Code bị trùng với khóa học đã có                         | Nhập mã khóa học khác                               |
| Không chọn được Subject                                        | Chưa chọn Program hoặc Program chưa có Subject tương ứng | Chọn Program trước hoặc kiểm tra dữ liệu Subject    |
| Chọn Foundation Course nhưng không lưu được                    | Chưa chọn level cho khóa học Foundation                  | Chọn ít nhất một level                              |
| Chọn Normal Course nhưng không thấy Foundation Course cần chọn | Chưa có Foundation Course tương ứng theo level           | Tạo Foundation Course trước hoặc kiểm tra lại level |
| Không lưu được điểm thành phần                                 | Tổng điểm các thành phần không bằng 100                  | Kiểm tra và điều chỉnh lại tỷ trọng điểm            |
| Thông tin đã nhập bị mất                                       | Người dùng rời màn hình khi chưa lưu                     | Chọn **Save** sau khi hoàn tất nhập thông tin       |
