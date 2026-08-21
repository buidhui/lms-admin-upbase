# Tạo hoạt động học

## I. Giới thiệu chung

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Khóa học đã được tạo thành công ở bước **Course Info**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Truy cập bước Course Content</summary>

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>

</details>

<details>

<summary>Tạo Section</summary>

{% stepper %}
{% step %}
**Tạo Section mới**

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền thông tin Section**

<figure><img src="../../../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

Các trường thông tin:

* Section Name (bắt buộc): tên của section.
* Section Short Name: tên viết tắt của section, dùng trong các trường hợp biều đồ hạn chế hiển thị tên quá dài.
* Describe: mô tả nội dung section.
{% endstep %}

{% step %}
**Chọn Save để lưu Section**

Nhân sự vận hành có thể Chỉnh sửa hoặc Xóa Section đã tạo.

<figure><img src="../../../.gitbook/assets/image (34).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Xóa section sẽ xóa toàn bộ nội dung có trong section đó.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Learning Outcome</summary>

{% stepper %}
{% step %}
**Để tạo mục tiêu học tập cho Seccion, chọn Action → Add Learning Outcome**

<figure><img src="../../../.gitbook/assets/image (30).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền thông tin Learning Outcome**

<figure><img src="../../../.gitbook/assets/image (968)" alt=""><figcaption></figcaption></figure>

Các trường thông tin:

* Name (bắt buộc): tên hiển thị của mục tiêu học tập trong khóa học.
* Mô tả: mô tả chung về mục tiêu học tập của section.
* Add more learning outcome: thêm các tiêu chí để hoàn thành mục tiêu học tập, các tiêu chí này sẽ được gắn với từng hoạt động học trong section đó
{% endstep %}

{% step %}
**Chọn Save để lưu Learning Outcome**

Nhân sự vận hành có thể chỉnh sửa hoặc xóa Learning Outcome đã tạo

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Activity</summary>

{% stepper %}
{% step %}
**Để tạo Activity, chọn Action → New Activity**

<figure><img src="../../../.gitbook/assets/image (33).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền thông tin Activity**

<figure><img src="../../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

Các trường thông tin:

* Activity Name: tên hoạt động học.
* Duration: thời lượng ước lượng cần thiết để hoàn thành hoạt động học.
* Type of Activity: loại icon hiển thị định dạng nội dung học tập trên hệ thống UpLMS
  * Text
  * Video
  * Quiz
* Choose Learning Outcome: chọn một hoặc nhiều tiêu chí mục tiêu học tập đã tạo ở [#tao-learning-outcome](tao-cau-phan-hoc-section-subsection-unit-activity.md#tao-learning-outcome "mention") gắn với hoạt động học.
* Upload File: đính kèm tài liệu gắn với hoạt động học đang tạo.

{% hint style="info" %}
- Phần uppload file, nhân sự tạo khóa học có thể chọn tài liệu từ kho tài liệu UpLMS hoặc upload trực tiếp từ thiết bị.&#x20;
- Kích cỡ file tối đa là 500MB và có thể thêm một hoặc nhiều tài liệu.
{% endhint %}
{% endstep %}

{% step %}
**Chọn Save để lưu Activity.**

Nhân sự vận hành có thể chỉnh sửa hoặc xóa Activity đã tạo

<figure><img src="../../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo nội dung cho Activity</summary>

Nội dung của hoạt động học được thể hiện trong các Tab, có ít nhất 1 Tab trong mỗi hoạt động học.

{% stepper %}
{% step %}
**Tại Activity cần tạo nội dung, chọn Action → Add Tab**

<figure><img src="../../../.gitbook/assets/image (38).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Điền tên Tab và lưu**

<figure><img src="../../../.gitbook/assets/image (39).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tạo nội dung trong Tab**

Tại Tab đã tạo, chọn Add Document.

<figure><img src="../../../.gitbook/assets/image (40).png" alt=""><figcaption></figcaption></figure>

Các loại document:

* Text: bao gồm chữ và hình ảnh (tạo trong Text Editor)
* Video
* Quiz

{% tabs %}
{% tab title="Text" %}
Nhập nội dung.

<figure><img src="../../../.gitbook/assets/image (42).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Video" %}
{% stepper %}
{% step %}
**Admin chọn Video trong danh sách Document.**

<figure><img src="../../../.gitbook/assets/image (983)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn loại upload video**

Admin có 2 lựa chọn:

<figure><img src="../../../.gitbook/assets/image (984)" alt=""><figcaption></figcaption></figure>

| Lựa chọn            | Mô tả                                                                         |
| ------------------- | ----------------------------------------------------------------------------- |
| **Single Video**    | Upload 1 video.                                                               |
| **Multiple Videos** | Chọn nhiều video, từ 1 đến 3 video, để tăng trải nghiệm học tập cho học viên. |
{% endstep %}

{% step %}
**Admin chọn Upload.**

<figure><img src="../../../.gitbook/assets/image (985)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị 2 cách upload video:

<figure><img src="../../../.gitbook/assets/image (986)" alt=""><figcaption></figcaption></figure>

| Cách upload                 | Mô tả                                                       |
| --------------------------- | ----------------------------------------------------------- |
| **Upload file từ thiết bị** | Admin chọn video từ thiết bị đang sử dụng.                  |
| **Chọn video từ Resource**  | Admin chọn video đã có sẵn trong kho tài liệu của hệ thống. |
|                             |                                                             |
{% endstep %}

{% step %}
**Cấu hình video nếu upload từ thiết bị**

Sau khi video được tải lên thành công, hệ thống chuyển tới giao diện cài đặt video. Admin có thể cấu hình:

<figure><img src="../../../.gitbook/assets/image (987)" alt=""><figcaption></figcaption></figure>

| Tab cấu hình | Mô tả                                                                                                              |
| ------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Timeline** | Thêm các mốc timeline cho video. Nội dung mô tả timeline không được bỏ trống và được sắp xếp theo thời gian video. |
| **Question** | Thêm câu hỏi vào từng mốc thời gian của video. Có thể thêm nhiều câu hỏi và tìm kiếm/lọc trong danh sách câu hỏi.  |
| **Settings** | Cấu hình quiz cho các câu hỏi đã thêm, gồm Quiz Name, Graded Assignment, Pass Point và Attempt.                    |
{% endstep %}

{% step %}
**Admin chọn Finish để lưu video vào màn hình tạo Tab.**
{% endstep %}

{% step %}
**Admin chọn Save Document để lưu Video vào nội dung Tab.**
{% endstep %}
{% endstepper %}
{% endtab %}

{% tab title="Quiz" %}
{% stepper %}
{% step %}
**Admin chọn Quiz trong danh sách Document.**

<figure><img src="../../../.gitbook/assets/image (988)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin thực hiện tạo bài Quiz/Test theo tài liệu hướng dẫn riêng về Tạo bài Test/Quiz.**

<figure><img src="../../../.gitbook/assets/image (989)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sau khi hoàn thành cấu hình Quiz/Test, Admin lưu Document vào Tab.**
{% endstep %}
{% endstepper %}
{% endtab %}
{% endtabs %}
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thêm Case Study vào Course Content</summary>

{% stepper %}
{% step %}
**Tại Subsection cần thêm Case Study, Admin chọn Action → Add Case Study.**

<figure><img src="../../../.gitbook/assets/image (990)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập thông tin chung cho Case Study trong khóa học**

<figure><img src="../../../.gitbook/assets/image (991)" alt=""><figcaption></figcaption></figure>

| Trường thông tin    | Mô tả                                 |
| ------------------- | ------------------------------------- |
| **Case Study Name** | Tên hiển thị cho học phần Case Study. |
| **Mô tả**           | Mô tả cho học phần Case Study.        |
{% endstep %}

{% step %}
**Admin bấm Choose Case Study. Sau đó chọn Case Study đã được tạo trước đó.**

<figure><img src="../../../.gitbook/assets/image (992)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Save để lưu Case Study vào nội dung khóa học.**
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Thêm Storyline vào Course Content</summary>

{% stepper %}
{% step %}
**Tại Unit cần thêm Storyline, Admin chọn Action → Add Story Line.**

<figure><img src="../../../.gitbook/assets/image (993)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập thông tin chung cho Storyline trong khóa học**

<figure><img src="../../../.gitbook/assets/image (994)" alt=""><figcaption></figcaption></figure>

| Trường thông tin   | Mô tả                                |
| ------------------ | ------------------------------------ |
| **Storyline Name** | Tên hiển thị cho học phần Storyline. |
| **Mô tả**          | Mô tả cho học phần Storyline.        |
{% endstep %}

{% step %}
**Admin bấm Choose Storyline. Sau đó chọn Storyline đã được tạo trước đó.**

<figure><img src="../../../.gitbook/assets/image (995)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Save để lưu Storyline vào nội dung khóa học.**
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Sao chép cấu phần học</summary>

**Các cấp có thể sao chép bao gồm:**

| Cấp sao chép   | Cách thao tác                                       | Cấu phần có thể sao chép                                           |
| -------------- | --------------------------------------------------- | ------------------------------------------------------------------ |
| **Section**    | Chọn **Copy Course Content** tại tab Course Content | Section, Midterm Test, Final Test, Mock Test đối với khóa Practice |
| **Subsection** | Chọn **Action → Copy Subsection**                   | Subsection, Part/Topic Test                                        |
| **Unit**       | Chọn **Action → Copy Unit**                         | Learning Outcome, Unit, Case Study, Chapter/Module Test            |
| **Activity**   | Chọn **Action → Copy Activity**                     | Activity                                                           |

<figure><img src="../../../.gitbook/assets/image (996)" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (997)" alt=""><figcaption></figcaption></figure>

#### Luồng thao tác chung

1. Admin chọn chức năng copy tại cấp tương ứng.
2. Admin chọn khóa học nguồn tại trường **Select Course**.
3. Admin chọn một hoặc nhiều cấu phần muốn sao chép.
4. Admin chọn **Save**.
5. Hệ thống sao chép cấu phần và các cấu phần con sang khóa học hiện tại.

</details>

<details>

<summary>Link cấu phần học</summary>

> Tính năng link chỉ áp dụng với khóa **Practice**. Các loại học phần có thể link gồm **Section, Subsection, Unit và Activity**.

{% stepper %}
{% step %}
**Chọn chức năng Link. Admin chọn một trong các thao tác:**

| Loại link           | Cách thao tác                                         |
| ------------------- | ----------------------------------------------------- |
| **Link Section**    | Chọn button Link Section tại màn hình Course Content. |
| **Link Subsection** | Chọn Action của Section → Link Subsection.            |
| **Link Unit**       | Chọn Action của Subsection → Link Unit.               |
| **Link Activity**   | Chọn Action của Unit → Link Activity.                 |

<figure><img src="../../../.gitbook/assets/image (998)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập tên khóa học chứa nội dung cần link.**

<figure><img src="../../../.gitbook/assets/image (999)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị danh sách gợi ý các khóa học chứa từ khóa đã nhập.
{% endstep %}

{% step %}
**Admin chọn khóa học chứa học phần cần link.**

<figure><img src="../../../.gitbook/assets/image (1000)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin tick chọn một hoặc nhiều học phần muốn link, sau đó chọn Confirm.**

<figure><img src="../../../.gitbook/assets/image (1001)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống quay về màn hình Course Content và hiển thị học phần đã link với ký hiệu tương ứng.**

<figure><img src="../../../.gitbook/assets/image (1002)" alt=""><figcaption></figcaption></figure>

**Bỏ link học phần:** Nếu muốn gỡ học phần đã link, Admin chọn **Unlink** từ Action của học phần muốn gỡ. Sau đó chọn **Yes** tại popup xác nhận để gỡ nội dung đã link.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xem trước nội dung đã tạo</summary>

{% stepper %}
{% step %}
**Admin chọn Preview từ Action của học phần muốn xem.**

<figure><img src="../../../.gitbook/assets/image (1003)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Hệ thống hiển thị nội dung đã tạo.**

<figure><img src="../../../.gitbook/assets/image (1004)" alt=""><figcaption></figcaption></figure>

Với Activity có nhiều Tab, Admin có thể chuyển giữa các Tab để xem nội dung. Tại giao diện Preview Activity, Admin cũng có thể xem video hoặc chuyển giữa các câu hỏi của bài Quiz.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Khóa/Mở khóa nội dung</summary>

> Chức năng này chỉ sử dụng cho khóa học có **Type = Trial Course**

{% stepper %}
{% step %}
**Admin chọn Action tại nội dung muốn khóa.**

<figure><img src="../../../.gitbook/assets/image (1005)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Lock.**

<figure><img src="../../../.gitbook/assets/image (1006)" alt=""><figcaption></figcaption></figure>

Sau khi khóa, nút **Lock** chuyển thành **Unlock**. Admin thực hiện tương tự để mở khóa lại nội dung.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Show Lock/Hide Lock nội dung</summary>

{% stepper %}
{% step %}
**Admin chọn Action tại nội dung cần thao tác.**

<figure><img src="../../../.gitbook/assets/image (1007)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Show Lock Icon.**

<figure><img src="../../../.gitbook/assets/image (1008)" alt=""><figcaption></figcaption></figure>

Sau khi thực hiện, nút **Show Lock** chuyển thành **Hide Lock**. Admin thực hiện tương tự để ẩn trạng thái khóa.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Change CTA to Preview / Change CTA to Begin</summary>

{% stepper %}
{% step %}
**Admin chọn Action tại nội dung muốn thay đổi CTA.**

<figure><img src="../../../.gitbook/assets/image (1009)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Change CTA to Preview.**

<figure><img src="../../../.gitbook/assets/image (1010)" alt=""><figcaption></figcaption></figure>

Sau khi thực hiện, nút này chuyển thành **Change CTA to Begin**. Admin thực hiện tương tự nếu muốn đổi lại CTA về Begin.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Với khóa học 4 level, cấu trúc nội dung cần được tạo theo thứ tự: **Section → Subsection → Unit → Activity**.
2. Admin cần tạo Section trước khi tạo Subsection.
3. Admin cần tạo Subsection trước khi tạo Unit.
4. Admin cần tạo Unit trước khi tạo Activity.
5. Learning Outcome được tạo ở cấp Subsection.
6. Activity có thể được gắn với một hoặc nhiều Learning Outcome.
7. Các trường có dấu **(\*)** là trường bắt buộc.
8. Tính năng link cấu phần học chỉ áp dụng với khóa Practice.
9. Không được link chồng các cấu phần học để tránh vòng lặp dữ liệu giữa các khóa học.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nên tạo Learning Outcome trước khi tạo Activity nếu Activity cần gắn mục tiêu học tập.
2. Với khóa học có nội dung tương tự khóa đã có, nên dùng chức năng **Copy Course Content** để tiết kiệm thời gian.
3. Với khóa Practice, nên dùng tính năng **Link** khi muốn tái sử dụng nội dung từ khóa học khác mà không cần sao chép thủ công.
4. Nên dùng **Preview** sau khi tạo Section, Unit hoặc Activity để kiểm tra cách hiển thị trước khi Publish khóa học.
5. Trước khi xóa cấu phần học, cần kiểm tra cấu phần đó có chứa nội dung con, Quiz/Test hoặc Case Study hay không.
6. Với phần upload file, Admin có thể chọn tài liệu từ kho tài liệu UpLMS hoặc upload trực tiếp từ thiết bị cá nhân; kích cỡ file tối đa là 500MB và có thể thêm một hoặc nhiều tài liệu đính kèm.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                | Nguyên nhân                                                          | Cách xử lý                                                                 |
| ----------------------------------------------- | -------------------------------------------------------------------- | -------------------------------------------------------------------------- |
| Không tạo được Section/Subsection/Unit/Activity | Thiếu trường bắt buộc                                                | Kiểm tra và nhập đầy đủ các trường có dấu **(\*)**                         |
| Không thấy nút tạo cấu phần con                 | Chưa tạo cấu phần cha hoặc tài khoản chưa có quyền                   | Kiểm tra cấu trúc cha và quyền tài khoản                                   |
| Không chọn được Learning Outcome cho Activity   | Chưa tạo Learning Outcome trong Subsection                           | Tạo Learning Outcome trước, sau đó quay lại Activity                       |
| Không lưu được Activity                         | Thiếu Duration, Type of Activity hoặc Grade Activity                 | Kiểm tra các trường bắt buộc của Activity                                  |
| Không upload được tài liệu Resource             | File vượt quá dung lượng hoặc định dạng không phù hợp                | Kiểm tra lại file, dung lượng tối đa 500MB                                 |
| Không thêm được Video                           | Chưa upload/chọn video hoặc thao tác chưa hoàn tất                   | Chọn video hợp lệ, bấm Finish và Save Document                             |
| Không link được học phần                        | Khóa học không phải Practice hoặc chọn sai cấu phần                  | Kiểm tra Type của khóa học và cấu phần cần link                            |
| Không thể sao chép bài kiểm tra                 | Khóa học đã có học viên hoàn thành 100% và bài kiểm tra có tính điểm | Chỉ sao chép bài kiểm tra không tính điểm hoặc kiểm tra lại rule nghiệp vụ |
| Preview không hiển thị đúng                     | Nội dung chưa được lưu hoặc chưa có Document                         | Lưu lại cấu phần/Document và thử Preview lại                               |
| Thay đổi chưa được lưu                          | Admin chưa chọn Save/Save Document/Finish                            | Kiểm tra đúng nút lưu tại từng màn hình                                    |
