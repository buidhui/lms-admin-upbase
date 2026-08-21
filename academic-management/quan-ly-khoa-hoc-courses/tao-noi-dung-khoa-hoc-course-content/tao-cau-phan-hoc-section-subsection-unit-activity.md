# Tạo cấu phần học (Section, Subsection, Unit, Activity)

## Record of changes

_A - Add | M - Modify | D - Delete_

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 20, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới thiệu chung

{% hint style="info" %}
**Dành cho:** Admin, SX

**Đường dẫn:** [https://ops.upbase.asia/courses?page\_index=1\&page\_size=10](https://ops.upbase.asia/courses?page_index=1\&page_size=10)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Course & Materials
* **Chức năng chính:** Course 4 Level > Course Content
* **Module liên quan:**
  * Course Info
  * Question Bank
  * Case Study
  * Storyline
  * Resources
  * Class
  * LMS học viên
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết

* Admin đã đăng nhập thành công vào hệ thống LMS Ops.
* Tài khoản Admin có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công ở bước **Course Info**.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Truy cập bước Course Content</summary>

{% stepper %}
{% step %}
**Admin hoàn thành bước Course Info và chọn Save để tạo khóa học.**

<figure><img src="../../../.gitbook/assets/image (959)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sau khi lưu Course Info, hệ thống chuyển sang bước Course Content.**

<figure><img src="../../../.gitbook/assets/image (960)" alt=""><figcaption></figcaption></figure>

Tại đây, Admin có thể bắt đầu tạo cấu trúc nội dung khóa học.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Section</summary>

{% stepper %}
{% step %}
**Tại màn hình Course Content, Admin chọn New Section.**

<figure><img src="../../../.gitbook/assets/image (961)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới Section ở phía bên phải màn hình.

<figure><img src="../../../.gitbook/assets/image (962)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin Section, các trường thông tin bao gồm:**

| Trường thông tin       | Bắt buộc | Mô tả                                                                                                    |
| ---------------------- | -------- | -------------------------------------------------------------------------------------------------------- |
| **Section Name**       | Y        | Tên của Section.                                                                                         |
| **Belong to**          | N        | Nội dung kiến thức của Section.                                                                          |
| **Section Short name** | N        | Tên viết tắt của Section.                                                                                |
| **Foundation content** | N        | Nội dung học quan trọng mà học viên cần hoàn thành trước khi học Section này. Có thể chọn nhiều giá trị. |
| **Describe**           | N        | Mô tả Section.                                                                                           |
{% endstep %}

{% step %}
**Admin chọn Save để lưu Section.**

Sau khi tạo thành công, Section được hiển thị trên cây nội dung khóa học.

Lúc này, admin có thể thực hiện các thao tác với Section như sau:

<figure><img src="../../../.gitbook/assets/image (963)" alt=""><figcaption></figcaption></figure>

| Thao tác                | Mô tả                                |
| ----------------------- | ------------------------------------ |
| **Mở rộng/thu nhỏ**     | Mở hoặc ẩn nội dung con của Section. |
| **New Subsection**      | Tạo Subsection trong Section.        |
| **Copy Subsection**     | Copy Subsection từ khóa học khác.    |
| **Add Part/Topic Test** | Tạo bài kiểm tra thuộc Section.      |
| **Edit**                | Chỉnh sửa Section.                   |
| **Preview**             | Xem trước nội dung Section.          |
| **Delete**              | Xóa Section.                         |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Subsection</summary>

{% stepper %}
{% step %}
**Tại Section cần tạo nội dung con, Admin chọn Action → New Subsection.**

<figure><img src="../../../.gitbook/assets/image (964)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới Subsection ở phía bên phải màn hình.

<figure><img src="../../../.gitbook/assets/image (965)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin Subsection, các trường thông tin bao gồm:**

| Trường thông tin          | Bắt buộc | Mô tả                                                                            |
| ------------------------- | -------- | -------------------------------------------------------------------------------- |
| **Subsection Name**       | Y        | Tên của Subsection.                                                              |
| **Subsection Short name** | N        | Tên viết tắt của Subsection.                                                     |
| **Foundation content**    | N        | Nội dung học quan trọng mà học viên cần hoàn thành trước khi học Subsection này. |
| **Description**           | N        | Mô tả của Subsection.                                                            |
{% endstep %}

{% step %}
**Admin chọn Save để lưu Subsection.**

Lúc này, admin có thể thực hiện các thao tác với Subsection như sau:

<figure><img src="../../../.gitbook/assets/image (966)" alt=""><figcaption></figcaption></figure>

| Thao tác                    | Mô tả                                   |
| --------------------------- | --------------------------------------- |
| **Mở rộng/thu nhỏ**         | Mở hoặc ẩn nội dung con của Subsection. |
| **Add Learning Outcome**    | Tạo mục tiêu học tập cho Subsection.    |
| **Add Chapter/Module Test** | Tạo bài kiểm tra thuộc Subsection.      |
| **Add Case Study**          | Thêm Case Study vào Subsection.         |
| **Add Unit**                | Tạo Unit thuộc Subsection.              |
| **Copy Unit**               | Copy Unit từ khóa học khác.             |
| **Edit**                    | Chỉnh sửa Subsection.                   |
| **Delete**                  | Xóa Subsection.                         |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Learning Outcome</summary>

{% stepper %}
{% step %}
**Tại Subsection cần tạo mục tiêu học tập, Admin chọn Action → Add Learning Outcome.**

<figure><img src="../../../.gitbook/assets/image (967)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới Learning schedule như hình.

<figure><img src="../../../.gitbook/assets/image (968)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập thông tin Learning Outcome, các trường thông tin bao gồm:**

| Trường thông tin              | Bắt buộc | Mô tả                                              |
| ----------------------------- | -------- | -------------------------------------------------- |
| **Name**                      | Y        | Tên hiển thị trên nội dung bài học.                |
| **Mô tả**                     | Y        | Mô tả Learning Outcome.                            |
| **Add more learning outcome** | N        | Tạo thêm nội dung mục tiêu học tập cho Subsection. |
{% endstep %}

{% step %}
**Admin chọn Save để lưu Learning Outcome.**

Lúc này, admin có thể thực hiện các thao tác với Learning Outcome như sau:

<figure><img src="../../../.gitbook/assets/image (969)" alt=""><figcaption></figcaption></figure>

| Thao tác   | Mô tả                       |
| ---------- | --------------------------- |
| **Edit**   | Chỉnh sửa Learning Outcome. |
| **Delete** | Xóa Learning Outcome.       |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Unit</summary>

{% stepper %}
{% step %}
**Tại Subsection cần tạo Unit, Admin chọn Action → Add Unit.**

<figure><img src="../../../.gitbook/assets/image (970)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới Unit ở phía bên phải màn hình.

<figure><img src="../../../.gitbook/assets/image (971)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin thực hiện nhập thông tin Unit, các trường thông tin bao gồm:**

| Trường thông tin | Bắt buộc | Mô tả         |
| ---------------- | -------- | ------------- |
| **Unit name**    | Y        | Tên của Unit. |
| **Mô tả**        | N        | Mô tả Unit.   |
{% endstep %}

{% step %}
**Admin chọn Save để lưu Unit.**

Khi này, admin có thể thực hiện các thao tác với Unit bao gồm:

<figure><img src="../../../.gitbook/assets/image (972)" alt=""><figcaption></figcaption></figure>

| Thao tác            | Mô tả                             |
| ------------------- | --------------------------------- |
| **Mở rộng/thu nhỏ** | Mở hoặc ẩn nội dung con của Unit. |
| **New Activity**    | Tạo Activity thuộc Unit.          |
| **Copy Activity**   | Copy Activity từ khóa học khác.   |
| **Add Storyline**   | Tạo storyline cho khóa học        |
| **Edit**            | Chỉnh sửa Unit.                   |
| **Preview**         | Xem trước Unit.                   |
| **Delete**          | Xóa Unit.                         |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Activity</summary>

{% stepper %}
{% step %}
**Tại Unit cần tạo Activity, Admin chọn Action → New Activity.**

<figure><img src="../../../.gitbook/assets/image (973)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới Activity như hình.

<figure><img src="../../../.gitbook/assets/image (974)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Lúc này, admin có thể nhập thông tin Activity bao gồm:**

| Trường thông tin            | Bắt buộc | Mô tả                                                                                               |
| --------------------------- | -------- | --------------------------------------------------------------------------------------------------- |
| **Activity Name**           | Y        | Tên hoạt động học tập.                                                                              |
| **Duration (Hour/Minutes)** | Y        | Thời lượng của Activity.                                                                            |
| **Type of Activity**        | Y        | Loại Activity hiển thị icon trên giao diện học viên LMS, gồm Text, Video, Quiz, Pass Exam Analysis. |
| **Grade Activity**          | Y        | Xác định Activity có tính điểm hay không. Hệ thống mặc định chọn Yes.                               |
| **Choose Learning Outcome** | N        | Chọn một hoặc nhiều Learning Outcome đã tạo.                                                        |
| **Upload File**             | N        | Đính kèm tài liệu vào nội dung Activity.                                                            |

Với phần upload file, Admin có thể chọn tài liệu từ kho tài liệu LMS hoặc upload trực tiếp từ thiết bị cá nhân; kích cỡ file tối đa là 500MB và có thể thêm một hoặc nhiều tài liệu đính kèm.
{% endstep %}

{% step %}
**Admin chọn Save để lưu Activity.**

Lúc này, admin có thể thực hiện các thao tác với Activity sau:

<figure><img src="../../../.gitbook/assets/image (975)" alt=""><figcaption></figcaption></figure>

| Thao tác    | Mô tả                            |
| ----------- | -------------------------------- |
| **Add Tab** | Tạo Tab nội dung trong Activity. |
| **Edit**    | Chỉnh sửa Activity.              |
| **Delete**  | Xóa Activity.                    |
| **Preview** | Xem trước nội dung Activity.     |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Tab nội dung cho Activity</summary>

{% stepper %}
{% step %}
**Tại Activity cần tạo nội dung, Admin chọn Action → Add Tab.**

<figure><img src="../../../.gitbook/assets/image (976)" alt=""><figcaption></figcaption></figure>

Hệ thống hiển thị form tạo mới tab như hình.

<figure><img src="../../../.gitbook/assets/image (977)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập tên tại trường Tab Name.**
{% endstep %}

{% step %}
**Chọn Save. Sau khi tạo Tab thành công, Admin có thể tiếp tục thêm Document vào Tab.**
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo Document trong Tab</summary>

{% stepper %}
{% step %}
**Tại Tab đã tạo, Admin chọn Add Document.**

<figure><img src="../../../.gitbook/assets/image (978)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn loại Document**

Hệ thống hiển thị các loại Document sau:

<figure><img src="../../../.gitbook/assets/image (979)" alt=""><figcaption></figcaption></figure>

| Loại Document | Mô tả                                            |
| ------------- | ------------------------------------------------ |
| **Text**      | Admin nhập nội dung dạng chữ cho bài học.        |
| **Video**     | Admin thêm video bài giảng cho chương trình học. |
| **Quiz**      | Admin tạo bài test cho học viên.                 |
{% endstep %}

{% step %}
**Tạo các loại Document như sau:**

{% tabs %}
{% tab title="Dạng Text" %}
{% stepper %}
{% step %}
**Admin chọn Text trong danh sách Document.**

<figure><img src="../../../.gitbook/assets/image (980)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin nhập nội dung học tập vào khu vực mô tả.**

<figure><img src="../../../.gitbook/assets/image (981)" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn Save Document để lưu nội dung.**

<figure><img src="../../../.gitbook/assets/image (982)" alt=""><figcaption></figcaption></figure>

Sau khi lưu, hệ thống hiển thị Document Text trong Tab. Admin có thể chỉnh sửa, xóa hoặc tiếp tục thêm Document khác.
{% endstep %}
{% endstepper %}
{% endtab %}

{% tab title="Dạng Video" %}
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

{% tab title="Dạng Quiz" %}
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
