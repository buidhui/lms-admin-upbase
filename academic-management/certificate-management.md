# Certificate Management

## Record of changes

_A - Add | M - Modify | D - Delete_

| Effective Date | Update Person | A,M,D | Change Description                                    | Version |
| -------------- | ------------- | ----- | ----------------------------------------------------- | ------- |
| May 18, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook                        | 4.7.0   |
| Jun 18, 2026   | Nhà BA        | M     | Chuẩn hóa component theo template User guide mới nhất | 4.8.0   |

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, SX

**Đường dẫn:** Course & Materials → Certificates
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Course & Materials
* **Chức năng chính:** Certificate Management
* **Module liên quan:** Course, Resources, Learning Progress / Certificate Logic, LMS học viên
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Người dùng đã đăng nhập thành công vào hệ thống vận hành **LMS Ops**.
* Tài khoản đã được cấp quyền truy cập chức năng **Certificates**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách / chi tiết chứng chỉ</summary>

{% stepper %}
{% step %}
**Truy cập màn hình Certificates**

Sau khi đăng nhập thành công, tại thanh Menu click vào **Certificates**. Các trường thông tin hiển thị bao gồm:

* Số thứ tự
* Tên Chứng chỉ
* Loại Chứng chỉ (theo từng loại Khóa học)
* Trạng thái: **Published** (có thể thêm vào làm Certificate của Khóa học) / **Block** (không xuất hiện trong danh sách chứng chỉ có thể thêm vào Khóa học)
* Ngày tạo và ngày cập nhật Chứng chỉ

<figure><img src="../.gitbook/assets/image (1401).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem hình ảnh chi tiết Chứng chỉ**

Click vào tên Chứng chỉ (Template Name) để xem hình ảnh chi tiết của Chứng chỉ.

<figure><img src="../.gitbook/assets/image (1402).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1403).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm Chứng chỉ**

<figure><img src="../.gitbook/assets/image (165).png" alt=""><figcaption></figcaption></figure>

Tìm kiếm theo các trường Tên Chứng chỉ, Program, Sort by, From Date - To Date.

* Chọn **Search** để hiển thị các Chứng chỉ theo điều kiện tìm kiếm.
* Chọn **Reset** để xóa tất cả giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới chứng chỉ</summary>

{% stepper %}
{% step %}
**Chọn Create Template**

Tại màn hình danh sách Chứng chỉ, chọn **Create Template** để chuyển đến màn hình tạo mới Chứng chỉ.

<figure><img src="../.gitbook/assets/image (166).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (167).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin cần thiết**

* **Tên Chứng chỉ**
* **Program:** chọn 1 giá trị trong các giá trị có sẵn.

<figure><img src="../.gitbook/assets/image (168).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Upload File ảnh chứng chỉ**

Click **Upload File** để mở màn hình chọn ảnh làm Chứng chỉ — có thể chọn ảnh từ thiết bị hoặc chọn ảnh có sẵn trên hệ thống.

<figure><img src="../.gitbook/assets/image (169).png" alt=""><figcaption></figcaption></figure>

* **Tải ảnh từ thiết bị:** Tại thẻ Upload File, chọn **Browse** để chọn ảnh. Định dạng cho phép: _.jpg, .jpeg, .png, .gif, .webp_. Chỉ được chọn một ảnh để tải lên.

<figure><img src="../.gitbook/assets/image (170).png" alt=""><figcaption></figcaption></figure>

* **Chọn ảnh có sẵn trên hệ thống:** Chuyển qua màn hình **Resources** và chọn hình ảnh cho Chứng chỉ.

<figure><img src="../.gitbook/assets/image (171).png" alt=""><figcaption></figcaption></figure>

Có thể tìm kiếm hình ảnh theo các điều kiện:

* Tên hình ảnh
* Vị trí tài liệu theo Khóa học (chọn lần lượt): Course → Part → Chapter → Unit → Activity
* Loại tài liệu: Image
* From Date - To Date: khoảng thời gian tải hình ảnh lên hệ thống

Click **Search** để tìm kiếm theo điều kiện đã nhập; click **Reset** để xóa điều kiện và hiển thị danh sách hình ảnh ban đầu.
{% endstep %}

{% step %}
**Click Upload để lưu ảnh**

<figure><img src="../.gitbook/assets/image (172).png" alt=""><figcaption><p>Tải file template chứng chỉ lên hệ thống</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (173).png" alt=""><figcaption><p>Chọn ảnh chứng chỉ từ hệ thống</p></figcaption></figure>
{% endstep %}

{% step %}
**Thêm khu vực hiển thị tên học viên**

Click **Add Student Name** để thêm khu vực hiển thị tên học viên.

<figure><img src="../.gitbook/assets/image (1404).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa đặc điểm ô chứa tên học viên**

* Click chuột phải 2 lần để di chuyển hoặc chỉnh lại kích cỡ của ô văn bản.
* Thay đổi kích chữ, font chữ, căn trái/phải/giữa… tại khu vực chỉnh sửa văn bản.
{% endstep %}

{% step %}
**Lưu Chứng chỉ**

Chọn **Save** để lưu Chứng chỉ.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa chứng chỉ</summary>

{% stepper %}
{% step %}
**Chỉnh sửa Trạng thái chứng chỉ**

Tại màn hình danh sách chứng chỉ, có thể đổi trạng thái từ **Published** sang **Block** và ngược lại.

<figure><img src="../.gitbook/assets/image (1405).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Mở màn hình chỉnh sửa Chứng chỉ**

Click vào Tên Chứng chỉ (Template Name) muốn chỉnh sửa để chuyển đến màn hình chỉnh sửa.

<figure><img src="../.gitbook/assets/image (1406).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin Chứng chỉ**

* Đổi tên
* Đổi program tương ứng với chương trình học
* Đổi ảnh Chứng chỉ
* Chỉnh sửa kích cỡ, định dạng ô chứa tên học viên và tên học viên

Nếu chứng chỉ đã được thêm vào Khóa học thì sẽ không được thay đổi thông tin về loại Chứng chỉ.
{% endstep %}

{% step %}
**Lưu thay đổi**

Chọn **Save** để lưu.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa chứng chỉ.
2. Trạng thái **Published** cho phép chứng chỉ được thêm vào làm Certificate của Course.
3. Trạng thái **Block** khiến chứng chỉ không xuất hiện trong danh sách chứng chỉ có thể thêm vào Course.
4. Hệ thống chỉ cho phép chọn **một ảnh** để làm ảnh chứng chỉ.
5. Định dạng ảnh được hỗ trợ: **.jpg, .jpeg, .png, .gif, .webp**.
6. Cần thêm khu vực **Student Name** để hệ thống hiển thị tên học viên trên chứng chỉ; có thể chỉnh vị trí, kích cỡ, font chữ và căn chỉnh của vùng tên học viên.
7. Nếu chứng chỉ đã được thêm vào Course thì không được thay đổi **Program** / Loại Chứng chỉ.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nên đặt tên chứng chỉ rõ ràng theo chương trình học, program hoặc mục đích sử dụng để dễ tìm kiếm.
2. Nếu dùng ảnh từ Resources, nên dùng bộ lọc **Course → Part → Chapter → Unit → Activity** để tìm đúng tài nguyên.
3. Nên kiểm tra kỹ trạng thái chứng chỉ trước khi gắn vào Course.
4. Nên để chứng chỉ ở trạng thái **Block** nếu mẫu chưa hoàn thiện hoặc chưa muốn sử dụng.
5. Trước khi lưu, nên kiểm tra lại vị trí hiển thị tên học viên trên ảnh để tránh lệch bố cục.
6. Với các chứng chỉ đã đưa vào Course, nên hạn chế chỉnh sửa để tránh ảnh hưởng đến cấu hình khóa học đang sử dụng.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                         | Nguyên nhân                                            | Cách xử lý                                                                  |
| -------------------------------------------------------- | ------------------------------------------------------ | --------------------------------------------------------------------------- |
| Không thể lưu chứng chỉ                                  | Chưa nhập đủ thông tin bắt buộc (Tên, Program, ảnh...) | Kiểm tra và nhập đầy đủ thông tin rồi bấm Save                              |
| Không upload được ảnh                                    | File ảnh sai định dạng hoặc chọn nhiều hơn 1 ảnh       | Chỉ chọn 1 ảnh thuộc định dạng .jpg, .jpeg, .png, .gif, .webp               |
| Không tìm thấy chứng chỉ                                 | Sai điều kiện lọc tìm kiếm                             | Kiểm tra lại điều kiện, bấm Reset để về danh sách mặc định                  |
| Chứng chỉ không hiển thị trong danh sách chọn cho Course | Chứng chỉ đang ở trạng thái **Block**                  | Chuyển trạng thái chứng chỉ sang **Published**                              |
| Không đổi được Loại Chứng chỉ / Program                  | Chứng chỉ đã được thêm vào Course                      | Không thể thay đổi để bảo toàn cấu hình khóa học; tạo chứng chỉ mới nếu cần |
| Tên học viên hiển thị lệch trên chứng chỉ                | Vị trí/kích cỡ ô Student Name chưa được căn chỉnh đúng | Chỉnh lại vị trí, kích cỡ, căn lề vùng Student Name trước khi Save          |
