# Tạo cấu phần học (Section, Subsection, Unit, Activity,...)

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn Admin cách sử dụng chức năng **Course Content** để tạo và cấu hình nội dung bài học cho khóa học trên hệ thống **OPS**.

Chức năng **Course Content** cho phép Admin xây dựng cấu trúc nội dung học tập cho khóa học theo mô hình nhiều cấp. Với khóa học dạng **4 level**, nội dung được tổ chức theo thứ tự:

**Section → Subsection → Unit → Activity**

Trong mỗi Activity, Admin có thể tạo các Tab nội dung và thêm các loại học liệu như **Text**, **Video**, **Quiz** hoặc cấu hình các bài kiểm tra/Case Study tùy theo nhu cầu đào tạo.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                                    | Quyền hạn                                                        |
| --------- | ------------------------------------------ | ---------------------------------------------------------------- |
| Admin     | Người quản trị/vận hành khóa học           | Có quyền tạo, chỉnh sửa và quản lý nội dung khóa học             |
| SX        | Người phụ trách học thuật/nội dung đào tạo | Có quyền thiết kế cấu trúc bài học, mục tiêu học tập và học liệu |

### 1.3 Phạm vi & Module liên quan

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

### 1.4 Điều kiện tiên quyết

* Admin đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản Admin có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công ở bước **Course Info**.

## II. Tổng Quan Giao Diện

![](<.gitbook/assets/image (1032)>)

Màn hình **Course Content** là bước thứ hai trong quy trình tạo khóa học. Tại màn hình này, Admin xây dựng cấu trúc nội dung học tập và tạo các học phần chi tiết cho khóa học.

Quy trình tạo khóa học gồm 4 bước:

| Bước       | Tên bước       | Mô tả                                           |
| ---------- | -------------- | ----------------------------------------------- |
| **Step 1** | Course Info    | Nhập thông tin chung của khóa học               |
| **Step 2** | Course Content | Tạo nội dung bài học                            |
| **Step 3** | Resource       | Thêm tài liệu cho khóa học                      |
| **Step 4** | Certificate    | Chọn chứng chỉ cho học viên hoàn thành khóa học |

### Các thành phần chính trên màn hình Course Content

![](<.gitbook/assets/image (1033)>)

![](<.gitbook/assets/image (1034)>)

| Khu vực / Thành phần             | Mô tả                                                                                                                    |
| -------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| **Thanh process**                | Hiển thị các bước tạo khóa học, trong đó Course Content là bước tạo nội dung bài học.                                    |
| **Cây nội dung khóa học**        | Hiển thị cấu trúc nội dung đã tạo theo dạng phân cấp Section, Subsection, Unit, Activity.                                |
| **New Section**                  | Tạo mới Section trong khóa học.                                                                                          |
| **Copy Course Content**          | Sao chép cấu phần học từ khóa học khác vào khóa học hiện tại.                                                            |
| **Link Section**                 | Liên kết Section từ khóa học khác, chỉ áp dụng với khóa Practice.                                                        |
| **Action/Menu thao tác**         | Hiển thị các thao tác tương ứng với từng cấu phần học như thêm mới, chỉnh sửa, xóa, preview, copy hoặc link.             |
| **Panel tạo/chỉnh sửa bên phải** | Hiển thị form nhập thông tin khi Admin tạo mới hoặc chỉnh sửa Section, Subsection, Unit, Activity hoặc các nội dung con. |
| **Save**                         | Lưu thông tin cấu phần đang tạo hoặc chỉnh sửa.                                                                          |
| **Next/Continue**                | Chuyển sang bước tiếp theo trong quy trình tạo khóa học, nếu hệ thống hỗ trợ.                                            |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Truy cập bước Course Content

{% stepper %}
{% step %}
## Hoàn thành Course Info

Admin hoàn thành bước **Course Info** và chọn **Save** để tạo khóa học.

![](<.gitbook/assets/image (1035)>)
{% endstep %}

{% step %}
## Truy cập Course Content

Sau khi lưu Course Info, hệ thống chuyển sang bước **Course Content**.

![](<.gitbook/assets/image (960)>)

Tại đây, Admin có thể bắt đầu tạo cấu trúc nội dung khóa học.
{% endstep %}
{% endstepper %}

### 3.2 Tạo Section

**Mục tiêu:** Admin tạo cấp nội dung lớn nhất trong khóa học.

{% stepper %}
{% step %}
## Chọn New Section

Tại màn hình **Course Content**, Admin chọn **New Section**.

![](<.gitbook/assets/image (961)>)

Hệ thống hiển thị form tạo mới Section ở phía bên phải màn hình.

![](<.gitbook/assets/image (962)>)
{% endstep %}

{% step %}
## Nhập thông tin Section

| Trường thông tin       | Bắt buộc | Mô tả                                                                                                    |
| ---------------------- | -------- | -------------------------------------------------------------------------------------------------------- |
| **Section Name**       | Y        | Tên của Section.                                                                                         |
| **Belong to**          | N        | Nội dung kiến thức của Section.                                                                          |
| **Section Short name** | N        | Tên viết tắt của Section.                                                                                |
| **Foundation content** | N        | Nội dung học quan trọng mà học viên cần hoàn thành trước khi học Section này. Có thể chọn nhiều giá trị. |
| **Describe**           | N        | Mô tả Section.                                                                                           |
{% endstep %}

{% step %}
## Lưu Section

Admin chọn **Save** để lưu Section.

Sau khi tạo thành công, Section được hiển thị trên cây nội dung khóa học.

Lúc này, admin có thể thực hiện các thao tác với Section như sau:

![](<.gitbook/assets/image (963)>)

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

### 3.3 Tạo Subsection

**Mục tiêu:** Admin tạo Subsection thuộc một Section đã có.

{% stepper %}
{% step %}
## Chọn New Subsection

Tại Section cần tạo nội dung con, Admin chọn **Action → New Subsection**.

![](<.gitbook/assets/image (964)>)

Hệ thống hiển thị form tạo mới Subsection ở phía bên phải màn hình.

![](<.gitbook/assets/image (965)>)
{% endstep %}

{% step %}
## Nhập thông tin Subsection

| Trường thông tin          | Bắt buộc | Mô tả                                                                            |
| ------------------------- | -------- | -------------------------------------------------------------------------------- |
| **Subsection Name**       | Y        | Tên của Subsection.                                                              |
| **Subsection Short name** | N        | Tên viết tắt của Subsection.                                                     |
| **Foundation content**    | N        | Nội dung học quan trọng mà học viên cần hoàn thành trước khi học Subsection này. |
| **Description**           | N        | Mô tả của Subsection.                                                            |
{% endstep %}

{% step %}
## Lưu Subsection

Admin chọn **Save** để lưu Subsection.

Lúc này, admin có thể thực hiện các thao tác với Subsection như sau:

![](<.gitbook/assets/image (966)>)

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

### 3.4 Tạo Learning Outcome

**Mục tiêu:** Admin tạo mục tiêu học tập cho Subsection.

{% stepper %}
{% step %}
## Chọn Add Learning Outcome

Tại Subsection cần tạo mục tiêu học tập, Admin chọn **Action → Add Learning Outcome**.

![](<.gitbook/assets/image (967)>)

Hệ thống hiển thị form tạo mới Learning schedule như hình.

![](<.gitbook/assets/image (968)>)
{% endstep %}

{% step %}
## Nhập thông tin Learning Outcome

| Trường thông tin              | Bắt buộc | Mô tả                                              |
| ----------------------------- | -------- | -------------------------------------------------- |
| **Name**                      | Y        | Tên hiển thị trên nội dung bài học.                |
| **Mô tả**                     | Y        | Mô tả Learning Outcome.                            |
| **Add more learning outcome** | N        | Tạo thêm nội dung mục tiêu học tập cho Subsection. |
{% endstep %}

{% step %}
## Lưu Learning Outcome

Admin chọn **Save** để lưu Learning Outcome.

Lúc này, admin có thể thực hiện các thao tác với Learning Outcome như sau:

![](<.gitbook/assets/image (969)>)

| Thao tác   | Mô tả                       |
| ---------- | --------------------------- |
| **Edit**   | Chỉnh sửa Learning Outcome. |
| **Delete** | Xóa Learning Outcome.       |
{% endstep %}
{% endstepper %}

### 3.5 Tạo Unit

**Mục tiêu:** Admin tạo Unit thuộc một Subsection.

{% stepper %}
{% step %}
## Chọn Add Unit

Tại Subsection cần tạo Unit, Admin chọn **Action → Add Unit**.

![](<.gitbook/assets/image (970)>)

Hệ thống hiển thị form tạo mới Unit ở phía bên phải màn hình.

![](<.gitbook/assets/image (971)>)
{% endstep %}

{% step %}
## Nhập thông tin Unit

| Trường thông tin | Bắt buộc | Mô tả         |
| ---------------- | -------- | ------------- |
| **Unit name**    | Y        | Tên của Unit. |
| **Mô tả**        | N        | Mô tả Unit.   |
{% endstep %}

{% step %}
## Lưu Unit

Admin chọn **Save** để lưu Unit.

Khi này, admin có thể thực hiện các thao tác với Unit bao gồm:

![](<.gitbook/assets/image (972)>)

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

### 3.6 Tạo Activity

**Mục tiêu:** Admin tạo hoạt động học tập thuộc Unit.

{% stepper %}
{% step %}
## Chọn New Activity

Tại Unit cần tạo Activity, Admin chọn **Action → New Activity**.

![](<.gitbook/assets/image (973)>)

Hệ thống hiển thị form tạo mới Activity như hình.

![](<.gitbook/assets/image (974)>)
{% endstep %}

{% step %}
## Nhập thông tin Activity

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
## Lưu Activity

Admin chọn **Save** để lưu Activity.

Lúc này, admin có thể thực hiện các thao tác với Activity sau:

![](<.gitbook/assets/image (975)>)

| Thao tác    | Mô tả                            |
| ----------- | -------------------------------- |
| **Add Tab** | Tạo Tab nội dung trong Activity. |
| **Edit**    | Chỉnh sửa Activity.              |
| **Delete**  | Xóa Activity.                    |
| **Preview** | Xem trước nội dung Activity.     |
{% endstep %}
{% endstepper %}

### 3.7 Tạo Tab nội dung cho Activity

**Mục tiêu:** Admin tạo khu vực chứa nội dung học tập trong Activity.

{% stepper %}
{% step %}
## Chọn Add Tab

Tại Activity cần tạo nội dung, Admin chọn **Action → Add Tab**.

![](<.gitbook/assets/image (976)>)

Hệ thống hiển thị form tạo mới tab như hình.

![](<.gitbook/assets/image (977)>)
{% endstep %}

{% step %}
## Nhập tên Tab

Admin nhập tên tại trường **Tab Name**.
{% endstep %}

{% step %}
## Lưu Tab

Chọn **Save**. Sau khi tạo Tab thành công, Admin có thể tiếp tục thêm Document vào Tab.
{% endstep %}
{% endstepper %}

### 3.8 Tạo Document trong Tab

**Mục tiêu:** Admin thêm nội dung học tập chi tiết vào Tab.

{% stepper %}
{% step %}
## Chọn Add Document

Tại Tab đã tạo, Admin chọn **Add Document**.

![](<.gitbook/assets/image (978)>)
{% endstep %}

{% step %}
## Chọn loại Document

Hệ thống hiển thị các loại Document sau:

![](<.gitbook/assets/image (979)>)

| Loại Document | Mô tả                                            |
| ------------- | ------------------------------------------------ |
| **Text**      | Admin nhập nội dung dạng chữ cho bài học.        |
| **Video**     | Admin thêm video bài giảng cho chương trình học. |
| **Quiz**      | Admin tạo bài test cho học viên.                 |
{% endstep %}
{% endstepper %}

#### 3.8.1 Tạo Document dạng Text

{% stepper %}
{% step %}
## Chọn Text

Admin chọn **Text** trong danh sách Document.

![](<.gitbook/assets/image (980)>)
{% endstep %}

{% step %}
## Nhập nội dung học tập

Admin nhập nội dung học tập vào khu vực mô tả.

![](<.gitbook/assets/image (981)>)
{% endstep %}

{% step %}
## Lưu Document

Admin chọn **Save Document** để lưu nội dung.

![](<.gitbook/assets/image (982)>)

Sau khi lưu, hệ thống hiển thị Document Text trong Tab. Admin có thể chỉnh sửa, xóa hoặc tiếp tục thêm Document khác.
{% endstep %}
{% endstepper %}

#### 3.8.2 Tạo Document dạng Video

{% stepper %}
{% step %}
## Chọn Video

Admin chọn **Video** trong danh sách Document.

![](<.gitbook/assets/image (983)>)
{% endstep %}

{% step %}
## Chọn loại upload video

Admin có 2 lựa chọn:

![](<.gitbook/assets/image (984)>)

| Lựa chọn            | Mô tả                                                                         |
| ------------------- | ----------------------------------------------------------------------------- |
| **Single Video**    | Upload 1 video.                                                               |
| **Multiple Videos** | Chọn nhiều video, từ 1 đến 3 video, để tăng trải nghiệm học tập cho học viên. |
{% endstep %}

{% step %}
## Chọn Upload

Admin chọn **Upload**.

![](<.gitbook/assets/image (985)>)

Hệ thống hiển thị 2 cách upload video:

![](<.gitbook/assets/image (986)>)

| Cách upload                 | Mô tả                                                       |
| --------------------------- | ----------------------------------------------------------- |
| **Upload file từ thiết bị** | Admin chọn video từ thiết bị đang sử dụng.                  |
| **Chọn video từ Resource**  | Admin chọn video đã có sẵn trong kho tài liệu của hệ thống. |
{% endstep %}

{% step %}
## Cấu hình video nếu upload từ thiết bị

Sau khi video được tải lên thành công, hệ thống chuyển tới giao diện cài đặt video. Admin có thể cấu hình:

![](<.gitbook/assets/image (987)>)

| Tab cấu hình | Mô tả                                                                                                              |
| ------------ | ------------------------------------------------------------------------------------------------------------------ |
| **Timeline** | Thêm các mốc timeline cho video. Nội dung mô tả timeline không được bỏ trống và được sắp xếp theo thời gian video. |
| **Question** | Thêm câu hỏi vào từng mốc thời gian của video. Có thể thêm nhiều câu hỏi và tìm kiếm/lọc trong danh sách câu hỏi.  |
| **Settings** | Cấu hình quiz cho các câu hỏi đã thêm, gồm Quiz Name, Graded Assignment, Pass Point và Attempt.                    |
{% endstep %}

{% step %}
## Lưu video

Admin chọn **Finish** để lưu video vào màn hình tạo Tab.
{% endstep %}

{% step %}
## Lưu Document

Admin chọn **Save Document** để lưu Video vào nội dung Tab.
{% endstep %}
{% endstepper %}

#### 3.8.3 Tạo Document dạng Quiz

{% stepper %}
{% step %}
## Chọn Quiz

Admin chọn **Quiz** trong danh sách Document.

![](<.gitbook/assets/image (988)>)
{% endstep %}

{% step %}
## Tạo Quiz/Test

Admin thực hiện tạo bài Quiz/Test theo tài liệu hướng dẫn riêng về **Tạo bài Test/Quiz**.

![](<.gitbook/assets/image (989)>)
{% endstep %}

{% step %}
## Lưu Document

Sau khi hoàn thành cấu hình Quiz/Test, Admin lưu Document vào Tab.
{% endstep %}
{% endstepper %}

### 3.9 Thêm Case Study vào Course Content

**Mục tiêu:** Admin thêm Case Study đã tạo vào nội dung khóa học.

{% stepper %}
{% step %}
## Chọn Add Case Study

Tại Subsection cần thêm Case Study, Admin chọn **Action → Add Case Study**.

![](<.gitbook/assets/image (990)>)
{% endstep %}

{% step %}
## Nhập thông tin chung

Admin nhập thông tin chung cho Case Study trong khóa học.

![](<.gitbook/assets/image (991)>)

| Trường thông tin    | Mô tả                                 |
| ------------------- | ------------------------------------- |
| **Case Study Name** | Tên hiển thị cho học phần Case Study. |
| **Mô tả**           | Mô tả cho học phần Case Study.        |
{% endstep %}

{% step %}
## Chọn Case Study

Admin bấm **Choose Case Study**. Sau đó chọn Case Study đã được tạo trước đó.

![](<.gitbook/assets/image (992)>)
{% endstep %}

{% step %}
## Lưu Case Study

Admin chọn **Save** để lưu Case Study vào nội dung khóa học.
{% endstep %}
{% endstepper %}

### 3.10 Thêm Storyline vào Course Content

**Mục tiêu:** Admin thêm Storyline đã tạo vào nội dung khóa học.

{% stepper %}
{% step %}
## Chọn Add Story Line

Tại Unit cần thêm Storyline, Admin chọn **Action → Add Story Line**.

![](<.gitbook/assets/image (993)>)
{% endstep %}

{% step %}
## Nhập thông tin chung

Admin nhập thông tin chung cho **Storyline** trong khóa học.

![](<.gitbook/assets/image (994)>)

| Trường thông tin   | Mô tả                                |
| ------------------ | ------------------------------------ |
| **Storyline Name** | Tên hiển thị cho học phần Storyline. |
| **Mô tả**          | Mô tả cho học phần Storyline.        |
{% endstep %}

{% step %}
## Chọn Storyline

Admin bấm **Choose Storyline**. Sau đó chọn Storyline đã được tạo trước đó.

![](<.gitbook/assets/image (995)>)
{% endstep %}

{% step %}
## Lưu Storyline

Admin chọn **Save** để lưu Storyline vào nội dung khóa học.
{% endstep %}
{% endstepper %}

### 3.11 Sao chép cấu phần học

**Mục tiêu:** Admin tạo nhanh nội dung khóa học bằng cách sao chép cấu phần từ khóa học đã tồn tại.

**Các cấp có thể sao chép bao gồm:**

| Cấp sao chép   | Cách thao tác                                       | Cấu phần có thể sao chép                                           |
| -------------- | --------------------------------------------------- | ------------------------------------------------------------------ |
| **Section**    | Chọn **Copy Course Content** tại tab Course Content | Section, Midterm Test, Final Test, Mock Test đối với khóa Practice |
| **Subsection** | Chọn **Action → Copy Subsection**                   | Subsection, Part/Topic Test                                        |
| **Unit**       | Chọn **Action → Copy Unit**                         | Learning Outcome, Unit, Case Study, Chapter/Module Test            |
| **Activity**   | Chọn **Action → Copy Activity**                     | Activity                                                           |

![](<.gitbook/assets/image (996)>)

![](<.gitbook/assets/image (997)>)

#### Luồng thao tác chung

{% stepper %}
{% step %}
## Chọn chức năng copy

Admin chọn chức năng copy tại cấp tương ứng.
{% endstep %}

{% step %}
## Chọn khóa học nguồn

Admin chọn khóa học nguồn tại trường **Select Course**.
{% endstep %}

{% step %}
## Chọn cấu phần

Admin chọn một hoặc nhiều cấu phần muốn sao chép.
{% endstep %}

{% step %}
## Lưu

Admin chọn **Save**.
{% endstep %}

{% step %}
## Hoàn tất sao chép

Hệ thống sao chép cấu phần và các cấu phần con sang khóa học hiện tại.
{% endstep %}
{% endstepper %}

### 3.12 Link cấu phần học

**Mục tiêu:** Admin liên kết cấu phần học từ khóa học khác vào khóa học hiện tại.

{% hint style="info" %}
Tính năng link chỉ áp dụng với khóa **Practice**. Các loại học phần có thể link gồm **Section, Subsection, Unit và Activity**.
{% endhint %}

{% stepper %}
{% step %}
## Chọn chức năng Link

Admin chọn một trong các thao tác:

| Loại link           | Cách thao tác                                         |
| ------------------- | ----------------------------------------------------- |
| **Link Section**    | Chọn button Link Section tại màn hình Course Content. |
| **Link Subsection** | Chọn Action của Section → Link Subsection.            |
| **Link Unit**       | Chọn Action của Subsection → Link Unit.               |
| **Link Activity**   | Chọn Action của Unit → Link Activity.                 |

![](<.gitbook/assets/image (998)>)
{% endstep %}

{% step %}
## Nhập tên khóa học

Admin nhập tên khóa học chứa nội dung cần link.

![](<.gitbook/assets/image (999)>)

Hệ thống hiển thị danh sách gợi ý các khóa học chứa từ khóa đã nhập.
{% endstep %}

{% step %}
## Chọn khóa học

Admin chọn khóa học chứa học phần cần link.

![](<.gitbook/assets/image (1000)>)
{% endstep %}

{% step %}
## Chọn học phần cần link

Admin tick chọn một hoặc nhiều học phần muốn link, sau đó chọn **Confirm**.

![](<.gitbook/assets/image (1001)>)
{% endstep %}

{% step %}
## Hoàn tất liên kết

Hệ thống quay về màn hình Course Content và hiển thị học phần đã link với ký hiệu tương ứng.

![](<.gitbook/assets/image (1002)>)
{% endstep %}
{% endstepper %}

**Bỏ link học phần:** Nếu muốn gỡ học phần đã link, Admin chọn **Unlink** từ Action của học phần muốn gỡ. Sau đó chọn **Yes** tại popup xác nhận để gỡ nội dung đã link.

### 3.13 Xem trước nội dung đã tạo

**Mục tiêu:** Admin kiểm tra cách nội dung hiển thị trước khi đưa vào sử dụng.

Admin có thể xem trước các nội dung:

* Section
* Unit
* Activity

{% stepper %}
{% step %}
## Chọn Preview

Admin chọn **Preview** từ Action của học phần muốn xem.

![](<.gitbook/assets/image (1003)>)
{% endstep %}

{% step %}
## Xem nội dung

Hệ thống hiển thị nội dung đã tạo.

![](<.gitbook/assets/image (1004)>)

Với Activity có nhiều Tab, Admin có thể chuyển giữa các Tab để xem nội dung. Tại giao diện Preview Activity, Admin cũng có thể xem video hoặc chuyển giữa các câu hỏi của bài Quiz.
{% endstep %}
{% endstepper %}

### 3.14 Khóa/Mở khóa nội dung

**Mục tiêu:** Admin kiểm soát trạng thái khóa của từng cấu phần học.

{% hint style="info" %}
Chức năng này chỉ sử dụng cho khóa học có **Type = Trial Course**
{% endhint %}

{% stepper %}
{% step %}
## Chọn Action

Admin chọn Action tại nội dung muốn khóa.

![](<.gitbook/assets/image (1005)>)
{% endstep %}

{% step %}
## Khóa nội dung

Admin chọn **Lock**.

![](<.gitbook/assets/image (1006)>)

Sau khi khóa, nút **Lock** chuyển thành **Unlock**. Admin thực hiện tương tự để mở khóa lại nội dung.
{% endstep %}
{% endstepper %}

### 3.15 Show Lock/Hide Lock nội dung

**Mục tiêu:** Admin kiểm soát việc hiển thị trạng thái khóa của nội dung trên giao diện học viên.

{% stepper %}
{% step %}
## Chọn Action

Admin chọn Action tại nội dung cần thao tác.

![](<.gitbook/assets/image (1007)>)
{% endstep %}

{% step %}
## Hiển thị biểu tượng khóa

Admin chọn **Show Lock Icon**.

![](<.gitbook/assets/image (1008)>)

Sau khi thực hiện, nút **Show Lock** chuyển thành **Hide Lock**. Admin thực hiện tương tự để ẩn trạng thái khóa.
{% endstep %}
{% endstepper %}

### 3.16 Change CTA to Preview / Change CTA to Begin

**Mục tiêu:** Admin thay đổi CTA hiển thị trên nội dung học tập.

{% stepper %}
{% step %}
## Chọn Action

Admin chọn Action tại nội dung muốn thay đổi CTA.

![](<.gitbook/assets/image (1009)>)
{% endstep %}

{% step %}
## Thay đổi CTA

Admin chọn **Change CTA to Preview**.

![](<.gitbook/assets/image (1010)>)

Sau khi thực hiện, nút này chuyển thành **Change CTA to Begin**. Admin thực hiện tương tự nếu muốn đổi lại CTA về Begin.
{% endstep %}
{% endstepper %}

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

{% hint style="warning" %}
* Với khóa học 4 level, cấu trúc nội dung cần được tạo theo thứ tự: **Section → Subsection → Unit → Activity**.
* Admin cần tạo Section trước khi tạo Subsection.
* Admin cần tạo Subsection trước khi tạo Unit.
* Admin cần tạo Unit trước khi tạo Activity.
* Learning Outcome được tạo ở cấp Subsection.
* Activity có thể được gắn với một hoặc nhiều Learning Outcome.
* Các trường có dấu **(\*)** là trường bắt buộc.
* Tính năng link cấu phần học chỉ áp dụng với khóa Practice.
* Không được link chồng các cấu phần học để tránh vòng lặp dữ liệu giữa các khóa học.
{% endhint %}

### 💡 Mẹo sử dụng

{% hint style="info" %}
* Nên tạo Learning Outcome trước khi tạo Activity nếu Activity cần gắn mục tiêu học tập.
* Với khóa học có nội dung tương tự khóa đã có, nên dùng chức năng **Copy Course Content** để tiết kiệm thời gian.
* Với khóa Practice, nên dùng tính năng **Link** khi muốn tái sử dụng nội dung từ khóa học khác mà không cần sao chép thủ công.
* Nên dùng **Preview** sau khi tạo Section, Unit hoặc Activity để kiểm tra cách hiển thị trước khi Publish khóa học.
* Trước khi xóa cấu phần học, cần kiểm tra cấu phần đó có chứa nội dung con, Quiz/Test hoặc Case Study hay không.
{% endhint %}
