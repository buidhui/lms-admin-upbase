# chuc nang cai dat va van hanh lop hoc zoom

## Cài Đặt Và Vận Hành Lớp Học Zoom

### Record of Changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description | Version |
| -------------- | ------------- | ----- | ------------------ | ------- |
| Nov 11, 2025   | Đinh Công Hải | A     | Create new         | 4.1.0   |

### Definitions and Acronyms

| # | Term              | Definition                                                              |
| - | ----------------- | ----------------------------------------------------------------------- |
| 1 | Ops               | Operations – Vận hành                                                   |
| 2 | LMS               | Learning Management System – Hệ thống quản lý học tập                   |
| 3 | Live Online       | Hình thức học trực tuyến qua Zoom                                       |
| 4 | Hybrid            | Hình thức học kết hợp trực tiếp và trực tuyến qua Zoom                  |
| 5 | Link Meeting      | Đường dẫn tham gia cuộc họp/lớp học Zoom                                |
| 6 | Construction Mode | Cấu hình hình thức tổ chức lớp học trên LMS (Live Online, Hybrid, v.v.) |

## I. Giới Thiệu Chung

### 1.1 Mục Đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Cài Đặt Và Vận Hành Lớp Học Zoom** trong hệ thống LMS Operations, bao gồm các bước cài đặt Zoom để tích hợp với LMS và quản lý link Zoom cho từng lớp học.

### 1.2 Đối Tượng Áp Dụng

| Đối tượng | Vai trò                           | Quyền hạn                                                |
| --------- | --------------------------------- | -------------------------------------------------------- |
| Ops       | Quản lý vận hành lớp học trên LMS | Cài đặt Zoom, thêm/sửa link Zoom cho lớp học và buổi học |

### 1.3 Phạm Vi & Module Liên Quan

* **Module chính:** Quản lý lớp học (Class Management) trên LMS Operations
* **Module liên quan:** Calendar (Lịch học), Lesson Management (Quản lý buổi học)
* **Hệ thống tích hợp:** Zoom (tích hợp qua link meeting cá nhân hóa)

### 1.4 Điều Kiện Tiên Quyết

* Đã có tài khoản Zoom và tài khoản LMS Operations với quyền vận hành lớp học.
* Lớp học phải có **Construction Mode** là **Live Online** hoặc **Hybrid** thì mới cần cài đặt link Zoom.

## II. Tổng Quan Giao Diện

Hai giao diện chính liên quan đến chức năng này:

* **Trang cài đặt cuộc họp Zoom (Zoom Web):** Nơi người dùng tạo và cấu hình cuộc họp Zoom, lấy link meeting để điền vào LMS.
* **Màn hình Class Detail trên LMS:** Bao gồm các tab **Setting** và **Calendar** cho phép thêm/sửa link Zoom ở cấp lớp học và cấp buổi học.

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Cài Đặt Zoom Để Tích Hợp Trên LMS

**Mục tiêu:** Tạo cuộc họp Zoom với cấu hình đúng chuẩn và lấy link meeting để điền vào hệ thống LMS.

{% stepper %}
{% step %}
### Tạo cuộc họp mới

Tại trang [web Zoom](https://app.zoom.us/meeting#/upcoming), chọn **Cuộc họp (Meeting)** trong menu, sau đó chọn **Lên lịch một cuộc họp (Schedule)**.

<figure><img src="https://sapp-academy.gitbook.io/files/qIQyQc4xJox7ESInwIsF" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Nhập thông tin cuộc họp

Điền đầy đủ thông tin cuộc họp theo yêu cầu.

<figure><img src="https://sapp-academy.gitbook.io/files/lUmrhK0wifFTkB4XI7Do" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Trường **Đăng ký (Register)** bắt buộc phải được chọn để hệ thống LMS có thể tạo link Zoom cá nhân hóa riêng cho từng học viên.
{% endhint %}
{% endstep %}

{% step %}
### Lưu thông tin cuộc họp

Chọn **Lưu (Save)** để lưu cấu hình cuộc họp.

<figure><img src="https://sapp-academy.gitbook.io/files/d2ITTWMxUF94LZ0t4Fid" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Tắt gửi email xác nhận đăng ký

{% hint style="warning" %}
Đây là bước bắt buộc và không được bỏ qua.

Do Zoom đã cài đặt **Bắt buộc đăng ký**, khi hệ thống LMS tạo lịch Zoom cho từng học viên, Zoom sẽ tự động gửi email xác nhận đăng ký chứa thông tin cuộc họp — điều này gây **mất bảo mật thông tin**.
{% endhint %}

Sau khi lưu, chuyển sang tab **Cài đặt email (Email Settings)**.

<figure><img src="https://sapp-academy.gitbook.io/files/ULM7CVwDqEzZaLmFwHZU" alt=""><figcaption></figcaption></figure>

Màn hình hiển thị giao diện _**Cài đặt email**_ như sau:

<figure><img src="https://sapp-academy.gitbook.io/files/lnd4ESfR6jDvEib41M1o" alt=""><figcaption></figcaption></figure>

Tại mục **Email xác nhận đăng ký**, chọn **Chỉnh sửa**, bỏ tích chọn gửi email, sau đó lưu lại.

<figure><img src="https://sapp-academy.gitbook.io/files/SFzE5JGzIyIJfzwm4Bc9" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị giao diện xác nhận đã tắt thành công chức năng gửi email xác nhận đăng ký.

<figure><img src="https://sapp-academy.gitbook.io/files/QFG5SC4hkZefktmRYJO2" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Truy cập danh sách cuộc họp

Tại menu ngang, chọn **Cuộc họp (Meeting)** trong **Ứng dụng web (Web app)** để chuyển đến màn hình danh sách các cuộc họp.

<figure><img src="https://sapp-academy.gitbook.io/files/YrkMB7A0hsQ1HX1RbCYe" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách các cuộc họp đã tạo.

<figure><img src="https://sapp-academy.gitbook.io/files/LmlEGYFOOAlXZS32yjLM" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lấy link Zoom

Chọn **Hiển thị lời mời tham gia cuộc họp (Show Invitation)** để lấy link Zoom.

<figure><img src="https://sapp-academy.gitbook.io/files/3EIzKsrI6aUxGi4A0G0D" alt=""><figcaption></figcaption></figure>

Copy link Zoom để sử dụng tại hệ thống LMS Operations ở bước tiếp theo.

<figure><img src="https://sapp-academy.gitbook.io/files/jRU1jvgWwc7vxH8YKjLY" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị thông báo thành công khi cuộc họp đã được cài đặt đúng chuẩn và link Zoom đã sẵn sàng sử dụng.
{% endstep %}
{% endstepper %}

### 3.2 Thêm / Sửa Link Zoom Cho Lớp Học

{% hint style="info" %}
Lớp học có **Construction Mode** là **Live Online** hoặc **Hybrid** cần được cấu hình link Zoom. Người dùng có thể thêm/sửa link Zoom theo các cách sau.
{% endhint %}

#### 3.2.1 Thêm / Sửa Link Zoom Tại Màn Hình Edit Class (Tab Setting)

**Mục tiêu:** Cập nhật link Zoom cho toàn bộ lịch học của lớp chưa diễn ra.

{% stepper %}
{% step %}
### Chọn tab Setting

Tại **Class Detail**, chọn tab **Setting**.

<figure><img src="https://sapp-academy.gitbook.io/files/JlKCG3A2R4CQUvBIPGhe" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Cập nhật Link Meeting

Chọn mục **Classroom** và điền **Link Meeting** vào trường tương ứng.

<figure><img src="https://sapp-academy.gitbook.io/files/tezscad5Rg9l5GqGxQlR" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lưu thông tin

Chọn **Save** để lưu thông tin.

<figure><img src="https://sapp-academy.gitbook.io/files/Zh41WWS6Ym7rvVvxuJ4y" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị thông báo lưu thành công. Link meeting được cập nhật cho **toàn bộ lịch học chưa diễn ra** của lớp. Hệ thống tự động tạo các link Zoom riêng biệt, cá nhân hóa cho từng học viên.

<figure><img src="https://sapp-academy.gitbook.io/files/0xE5LPK7VaRNz9FcfojZ" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

#### 3.2.2 Thêm / Sửa Link Zoom Tại Generate Schedule (Tab Calendar)

**Mục tiêu:** Cập nhật link Zoom đồng thời khi tạo lịch học hàng loạt cho lớp.

{% stepper %}
{% step %}
### Chọn Generate Schedule

Tại tab **Calendar** trong **Class Detail**, chọn **Generate Schedule**.

<figure><img src="https://sapp-academy.gitbook.io/files/mTaOONVTV1ZNPQNgScV5" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Nhập Link Meeting

Chọn mục **Classroom** và điền **Link Meeting**.

<figure><img src="https://sapp-academy.gitbook.io/files/FF8VZa12kO4ZVmjb1rV1" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Tạo lịch học

Chọn **Generate** để lưu và tạo lịch học.

<figure><img src="https://sapp-academy.gitbook.io/files/O0xyASsnxh2PyLczRJ3w" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị thông báo thành công. Link meeting được cập nhật cho **toàn bộ lịch học chưa diễn ra** được tạo từ lần Generate này.

<figure><img src="https://sapp-academy.gitbook.io/files/bz2HA5elS5vZySa8ROf6" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

#### 3.2.3 Thêm Link Zoom Khi Tạo Buổi Học Đơn Lẻ Mới

**Mục tiêu:** Cấu hình link Zoom ngay khi tạo một buổi học mới ngoài lịch tự động.

{% stepper %}
{% step %}
### Thêm buổi học mới

Tại tab **Calendar** trong **Class Detail**, chọn **Add Lesson** để thêm buổi học mới.

<figure><img src="https://sapp-academy.gitbook.io/files/hCW6RZg4ex7Uj3Vb7w64" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Nhập Link Meeting

Tại màn hình **Create Lesson**, nhập thông tin **Link Meeting** vào trường tương ứng.

<figure><img src="https://sapp-academy.gitbook.io/files/DPOyw99cWD22ivHJ5fY3" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lưu buổi học

Chọn **Save** để lưu thông tin buổi học. Hệ thống hiển thị thông báo tạo buổi học thành công với link Zoom đã được gán.
{% endstep %}
{% endstepper %}

#### 3.2.4 Sửa Link Zoom Của Buổi Học Đơn Lẻ

**Mục tiêu:** Cập nhật link Zoom cho một buổi học cụ thể đã có trong lịch.

{% stepper %}
{% step %}
### Mở màn hình Edit Lesson

Tại màn hình **View Detail** của buổi học cần sửa, chọn **Edit**.

<figure><img src="https://sapp-academy.gitbook.io/files/uPRXlk5gF4q7Nk2IfL4d" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Cập nhật Link Meeting

Tại màn hình **Edit Lesson**, cập nhật **Link Meeting** và điền **Reason for Change** (lý do thay đổi).

<figure><img src="https://sapp-academy.gitbook.io/files/Xi3CuFFJ8A2e6XREhwm9" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Lưu thay đổi

Chọn **Save** để lưu. Hệ thống hiển thị thông báo cập nhật buổi học thành công.
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### Lưu ý quan trọng

{% hint style="warning" %}
* Trường **Đăng ký (Register)** trên Zoom **bắt buộc phải được bật** khi tạo cuộc họp. Nếu không bật, hệ thống LMS sẽ không thể tạo link Zoom cá nhân hóa cho từng học viên.
* Bước **tắt gửi email xác nhận đăng ký** (Bước 4) là **bắt buộc**. Nếu bỏ qua, Zoom sẽ tự động gửi email chứa thông tin cuộc họp tới học viên, gây mất bảo mật.
* Chức năng thêm/sửa link Zoom **chỉ áp dụng** cho lớp học có **Construction Mode** là **Live Online** hoặc **Hybrid**.
{% endhint %}

### Phạm vi cập nhật link theo từng thao tác

| Thao tác                          | Phạm vi cập nhật link Zoom                               |
| --------------------------------- | -------------------------------------------------------- |
| Sửa tại Tab Setting (Edit Class)  | Toàn bộ lịch học của lớp **chưa diễn ra**                |
| Generate Schedule (Tab Calendar)  | Toàn bộ lịch học **chưa diễn ra** tạo từ lần Generate đó |
| Add Lesson (buổi học đơn lẻ mới)  | Chỉ buổi học vừa được tạo                                |
| Edit Lesson (sửa buổi học đơn lẻ) | Chỉ buổi học được chỉnh sửa                              |

### Mẹo sử dụng

* Khi sửa link Zoom của một buổi học đơn lẻ, trường **Reason for Change** là bắt buộc — hãy điền lý do rõ ràng để phục vụ kiểm tra lịch sử thay đổi sau này.
* Nên cài đặt link Zoom từ sớm (tại Tab Setting) trước khi generate lịch học để đảm bảo toàn bộ lịch tự động được gán link đúng ngay từ đầu.

## V. Các Lỗi Thường Gặp Và Cách Xử Lý

| Lỗi / Tình huống                                                     | Nguyên nhân                                                             | Cách xử lý                                                                                        |
| -------------------------------------------------------------------- | ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| Hệ thống LMS không tạo được link Zoom cá nhân hóa cho học viên       | Trường **Register** trên Zoom chưa được bật khi tạo cuộc họp            | Kiểm tra lại cấu hình cuộc họp Zoom, bật tùy chọn **Bắt buộc đăng ký (Register)** và lưu lại      |
| Học viên nhận email xác nhận đăng ký từ Zoom chứa thông tin cuộc họp | Bước tắt gửi email xác nhận đăng ký (Bước 4) bị bỏ qua                  | Vào tab **Cài đặt email** của cuộc họp Zoom, tắt chức năng gửi email xác nhận đăng ký             |
| Link Zoom không hiển thị trong lịch học sau khi Save                 | Lịch học đã diễn ra trước thời điểm cập nhật link                       | Hệ thống chỉ cập nhật link cho các lịch học **chưa diễn ra**; các buổi đã qua không bị ảnh hưởng  |
| Không tìm thấy trường Link Meeting tại màn hình Edit Class           | Lớp học có Construction Mode không phải **Live Online** hoặc **Hybrid** | Kiểm tra lại Construction Mode của lớp học; chỉ các lớp Live Online hoặc Hybrid mới cần link Zoom |
| Không lưu được khi Edit Lesson                                       | Trường **Reason for Change** bị để trống                                | Điền lý do thay đổi vào trường **Reason for Change** trước khi chọn Save                          |

## VI. Câu Hỏi Thường Gặp

<details>

<summary>Q: Tại sao phải bật tùy chọn Register khi tạo cuộc họp Zoom?</summary>

A: Trường Register là điều kiện bắt buộc để hệ thống LMS tạo được link Zoom cá nhân hóa riêng cho từng học viên. Nếu không bật, LMS sẽ không thể phân phối link riêng biệt cho mỗi người.

</details>

<details>

<summary>Q: Nếu bỏ qua Bước 4 (tắt email xác nhận), điều gì xảy ra?</summary>

A: Zoom sẽ tự động gửi email chứa thông tin cuộc họp đến tất cả học viên khi hệ thống LMS tạo link đăng ký, gây mất bảo mật thông tin buổi học.

</details>

<details>

<summary>Q: Khi sửa link Zoom tại Tab Setting, các buổi học đã diễn ra có bị thay đổi không?</summary>

A: Không. Hệ thống chỉ cập nhật link cho các lịch học **chưa diễn ra**.

</details>

<details>

<summary>Q: Có thể thêm link Zoom cho lớp học có Construction Mode là Offline không?</summary>

A: Không. Chức năng thêm/sửa link Zoom chỉ áp dụng cho lớp có Construction Mode là **Live Online** hoặc **Hybrid**.

</details>

<details>

<summary>Q: Sự khác nhau giữa thêm link tại Tab Setting và Tab Calendar (Generate Schedule) là gì?</summary>

A: Cả hai đều cập nhật link cho toàn bộ lịch học chưa diễn ra. Tuy nhiên, Tab Setting áp dụng cho toàn bộ lịch học hiện có của lớp, còn Generate Schedule tạo mới lịch học và gán link đồng thời trong cùng một thao tác.

</details>

_Mọi thắc mắc vui lòng liên hệ bộ phận hỗ trợ nội bộ hoặc team Ops._
