# Tạo bài Test/Quiz cho khóa học

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

<summary>Tạo mới bài Test/Quiz</summary>

{% stepper %}
{% step %}
**Sau khi chọn loại bài test, Admin cần nhập các thông tin cho bài test như ảnh sau:**

<figure><img src="../../../.gitbook/assets/image (916).png" alt=""><figcaption></figcaption></figure>

<table><thead><tr><th width="180">Tên trường thông tin</th><th>Mô tả</th></tr></thead><tbody><tr><td>Name</td><td>Nhập tên bài test</td></tr><tr><td>Type of Test</td><td><p>Loại bài kiểm tra:</p><ul><li>Multiple Choice: Dạng bài trắc nghiệm</li><li>Constructed: Dạng bài tự luận</li><li>Mixed (Multiple Choice + Constructed): Dạng bài mix, bao gồm cả trắc nghiệm và tự luận.</li><li>Mặc định chọn Multiple Choice</li></ul></td></tr><tr><td>Test Mode</td><td><p>Admin chọn một trong hai loại bài test dưới đây:</p><ul><li>Tutor: cho phép học viên làm bài không giới hạn thời gian</li><li>Timed: giới hạn thời gian làm bài → Nếu Admin chọn Timed, màn hình hiển thị Duration yêu cầu Admin nhập thời gian cho phép làm bài theo giờ và phút</li><li>Mặc định chọn Tutor</li></ul></td></tr><tr><td>Manual Grading</td><td><p>Chỉ hiển thị với Type of Test = Constructed/Mixed (Multiple Choice + Constructed)</p><ul><li>Yes: bài kiểm tra sẽ được chấm điểm thủ công bởi đội SX.</li><li>No: bài kiểm tra sẽ được hệ thống chấm điểm tự động.</li></ul></td></tr><tr><td>Graded Assignment</td><td><p>Đánh dấu bài kiểm tra được sử dụng để tính điểm cho toàn bộ khóa học, gồm 2 giá trị:</p><ul><li>Yes</li><li>No<br></li></ul></td></tr><tr><td>Grading Preference</td><td><p>Chọn cách hiển thị đáp án và Solution</p><ul><li>After each question: hiển thị sau khi trả lời mỗi câu hỏi</li><li>After all questions: hiển thị sau khi hoàn thành bài test</li><li>Mặc định chọn After all questions</li></ul></td></tr><tr><td>Pass Point</td><td><p>Điểm pass bài test</p><ul><li>Auto 50%: điểm pass point là 50%</li><li>Manual: cho phép Admin nhập số điểm pass point → Nếu Admin chọn ‘Manual’ màn hình hiển thị textbox cho phép Admin nhập số điểm</li><li>Mặc định chọn Auto 50%</li></ul></td></tr><tr><td>Attempt</td><td><p>Cho phép chọn số lần làm bài</p><ul><li>Unlimited: không giới hạn số lần làm bài</li><li>Limited: giới hạn số lần làm bài → Nếu Admin chọn ‘Limited' màn hình hiển thị textbox cho phép Admin nhập số lần học viên được phép nộp bài</li><li>Mặc định chọn Unlimited</li></ul></td></tr><tr><td>Total Score</td><td><ul><li>Tổng điểm của bài Test/Quiz, có thể điền khác thang điểm 100.</li><li>Chỉ nhập giá trị lớn hơn 0.</li><li>Phần thập phân tối đa 2 chữ số.</li></ul></td></tr></tbody></table>

{% hint style="info" %}
Với các loại bài kiểm tra là Quiz/Chapter test/Topic Test/Midterm test/Final test, khi người dùng chọn Manual Grading = ‘Yes’ thì giá trị của Graded Assignment = ‘Yes’.

Với loại bài kiểm tra là Mocktest thì giá trị của Graded Assignment = 'No' trong mọi trường hợp.
{% endhint %}
{% endstep %}

{% step %}
**Admin thực hiện cài đặt câu hỏi cho bài test bằng cách click Configure Questions, gồm 3 bước:**

* Add Question: thêm câu hỏi vào bài Test/Quiz
* Setup Score: cài đặt điểm cho bài test và cho từng câu hỏi trong bài Test
* Reorder: sắp xếp thứ tự hiển thị của câu hỏi trong bài test.

<figure><img src="../../../.gitbook/assets/image (917).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Admin chọn "Add Question" để cài đặt thông tin câu hỏi cho bài Test/Quiz**

Tại bước **Add Question**, màn hình hiển thị danh sách câu hỏi đã được tạo trên hệ thống theo loại bài Test/Quiz mà người dùng đã chọn trước đó (Multiple choice, Constructed hoặc Mixed)

<figure><img src="../../../.gitbook/assets/image (918).png" alt=""><figcaption></figcaption></figure>

Người dùng sử dụng bộ lọc để tìm kiếm câu hỏi cần thêm vào bài Test/Quiz.

| Bộ lọc        | Mô tả                                                     |
| ------------- | --------------------------------------------------------- |
| Search        | Tìm kiếm theo tên/nội dung câu hỏi                        |
| Course        | Lọc câu hỏi theo khóa học                                 |
| Part          | Lọc câu hỏi theo học phần                                 |
| Chapter       | Lọc câu hỏi theo chương                                   |
| Unit          | Lọc câu hỏi theo bài học                                  |
| Activity      | Lọc câu hỏi theo hoạt động                                |
| Item Set      | Lọc câu hỏi theo Item Set                                 |
| Question Type | Lọc câu hỏi theo loại câu hỏi, có thể chọn nhiều giá trị. |

{% hint style="info" %}
**Danh sách câu hỏi hiển thị phụ thuộc vào Type of Test.**

* Type of Test = Multiple Choice: Hệ thống hiển thị toàn bộ câu hỏi trắc nghiệm trên hệ thống.
* Type of Test = Constructed Question: Hệ thống hiển thị toàn bộ câu hỏi tự luận trên hệ thống.
* Type of Test = Mixed: Hệ thống hiển thị cả câu hỏi trắc nghiệm và câu hỏi tự luận.

**Cách sắp xếp:**

* Câu hỏi được nhóm theo **Item Set**.
* Item Set được tạo gần đây nhất hiển thị ở đầu danh sách.
* Các câu hỏi trong cùng một Item Set được sắp xếp theo thời gian tạo từ gần đến xa.
* Câu hỏi trắc nghiệm và tự luận có thể hiển thị xen kẽ theo đúng thứ tự tạo trong Item Set.
{% endhint %}
{% endstep %}

{% step %}
**Admin thực hiện tick chọn các câu hỏi cần thêm vào bài test**

Số lượng câu hỏi đã chọn được hiển thị ở góc màn hình như ảnh sau:

<figure><img src="../../../.gitbook/assets/image (919).png" alt=""><figcaption></figcaption></figure>

Thứ tự câu hỏi tại bước **Setup Score** và **Reorder** phụ thuộc vào thứ tự người dùng chọn câu hỏi tại bước **Add Question**.

| Trường hợp                                          | Logic hệ thống                                                          |
| --------------------------------------------------- | ----------------------------------------------------------------------- |
| Người dùng chọn đơn lẻ từng câu                     | Câu nào được chọn trước sẽ đứng trước                                   |
| Người dùng chọn toàn bộ câu hỏi trong trang         | Thứ tự câu hỏi giữ nguyên như thứ tự đang hiển thị tại màn Add Question |
| Người dùng chọn một câu, sau đó bỏ chọn và chọn lại | Câu hỏi đó được đưa xuống cuối danh sách                                |
{% endstep %}

{% step %}
**Admin click button Add & Create để thêm câu hỏi, tạo bài test theo thông tin đã cài đặt trước đó, đồng thời chuyển sang bước Setup Score.**

{% hint style="info" %}
Nếu bài Test/Quiz đã có người làm, người dùng chỉ xem thông tin tại bước Add Question và không thể chỉnh sửa.
{% endhint %}

Setup Score: Thiết lập điểm cho câu hỏi
{% endstep %}

{% step %}
**Tại màn hình Setup Score, người dùng cài đặt thông tin điểm của bài Test/Quiz.**

Màn hình gồm 2 khu vực chính:

1. Khu vực cài đặt điểm cho bài Test/Quiz.
2. Khu vực hiển thị danh sách câu hỏi.

<figure><img src="../../../.gitbook/assets/image (920).png" alt=""><figcaption></figcaption></figure>

Người dùng thực hiện điền thông tin tại Khu vực cài đặt điểm cho toàn bộ bài Test/Quiz.

Các trường thông tin bao gồm:

| Trường thông tin   | Mô tả                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Total Score        | <p>Tổng điểm tối đa của bài Test/Quiz, cho phép người dùng điền số lớn hơn 0 và có thể khác 100.</p><p>Khi thay đổi Total Score, hệ thống sẽ tự động tính lại toàn bộ điểm của từng Question (Mark) nếu Score Distribution = Evenly across all questions hoặc Evenly by Question Type</p>                                                                                                                                                                                       |
| Current Score      | <p>Tổng điểm hiện tại của toàn bộ câu hỏi, hệ thống tự tính:</p><ul><li>Nếu Tổng điểm của toàn bộ câu hỏi trong bài test <strong>lớn hơn</strong> hoặc <strong>nhỏ hơn</strong> Total Score: khi ấn Next để chuyển sang bước 3 báo lỗi ‘Mark of all questions not equal [Total Score]’</li><li>Nếu Tổng điểm của toàn bộ câu hỏi trong bài test <strong>bằng</strong> Total Score: click Next chuyển sang bước tiếp theo thành công</li></ul>                                   |
| Score Distribution | <p>Cách phân phối điểm cho từng câu hỏi, chọn 1 trong 3 giá trị:</p><ul><li>Evenly across all questions: Hệ thống tự động chia đều <strong>Total Score</strong> cho toàn bộ câu hỏi trong bài Test/Quiz.</li><li>Evenly by Question Type (MCQ/Essay): cài đặt điểm cho nhóm câu hỏi trắc nghiệm (MCQ) và câu hỏi tự luận (Essay), sau đó hệ thống sẽ tự chia đều điểm cho các câu hỏi trong từng nhóm.</li><li>Custom: người dùng tự chỉnh sửa điểm của từng câu hỏi.</li></ul> |
| MCQ Score          | <p>Tổng điểm dành cho các câu hỏi trắc nghiệm, chỉ hiển thị nếu Score Distribution = Evenly by Question Type (MCQ/Essay).</p><p>Chỉ điền số lớn hơn 0 và nhỏ hơn Total Score, nếu không thỏa mãn thì khi click Next sang bước tiếp theo báo lỗi bên dưới trường thông tin như sau ‘MCQ Score must be between 0 and [Total Score]’</p>                                                                                                                                           |
| Essay Score        | <p>Tổng điểm dành cho các câu hỏi tự luận, chỉ hiển thị nếu Score Distribution = Evenly by Question Type (MCQ/Essay)</p><p>Chỉ điền số lớn hơn 0 và nhỏ hơn Total Score, nếu không thỏa mãn thì khi click Next sang bước tiếp theo báo lỗi bên dưới trường thông tin như sau ‘Essay Score must be between 0 and [Total Score]’</p>                                                                                                                                              |
{% endstep %}

{% step %}
**Cài đặt điểm cho từng câu hỏi.**

Tại khu vực hiển thị danh sách câu hỏi, các thông tin được hiển thị như sau:

* STT
* Question: nội dung câu hỏi
* Item Set name: tên Item set
* Type: loại câu hỏi
* Level: mức độ của câu hỏi
* Mark: điểm tuyệt đối của câu hỏi. Giá trị của Mark phụ thuộc vào **Score Distribution** đã cài đặt ở trên:
  * Evenly across all questions: Hệ thống chia đều Total Score cho toàn bộ câu hỏi
  * Evenly by Question Type (MCQ/Essay): Hệ thống chia đều MCQ Score/Essay Score cho từng nhóm câu hỏi
  * Custom:
    * Người dùng tự nhập điểm cho từng câu hỏi
    * Người dùng có thể thiết lập điểm hàng loạt cho nhiều câu hỏi bằng cách:
      *   Tick chọn từ 2 câu hỏi trở lên. Lúc này hệ thống hiển thị nút **Setup Score** kèm số lượng câu hỏi đã chọn.

          <figure><img src="../../../.gitbook/assets/image (921).png" alt=""><figcaption></figcaption></figure>
      *   Click vào nút **Setup Score** và điền điểm tại popup, sau đó chọn **Save** để lưu

          <figure><img src="../../../.gitbook/assets/image (922).png" alt=""><figcaption></figcaption></figure>
* Converted Mark:
  * Điểm của câu hỏi sau khi quy đổi về thang 100.
  * Công thức: Converted Mark = Mark / Total Score × 100.

Người dùng có thể sử dụng Filter để lọc ra danh sách câu hỏi mong muốn, cụ thể:

| Trường        | Mô tả                               |
| ------------- | ----------------------------------- |
| Search        | Tìm kiếm theo tên/nội dung câu hỏi  |
| Course        | Lọc theo khóa học                   |
| Part          | Lọc theo học phần                   |
| Chapter       | Lọc theo chương                     |
| Unit          | Lọc theo bài học                    |
| Activity      | Lọc theo hoạt động                  |
| Item Set      | Lọc theo Item Set                   |
| Question Type | Lọc theo loại câu hỏi               |
| Group by      | Nhóm câu hỏi theo giá trị được chọn |
| Sort by       | Sắp xếp danh sách câu hỏi           |
| From date     | Lọc theo thời gian tạo từ ngày      |
| To date       | Lọc theo thời gian tạo đến ngày     |
{% endstep %}

{% step %}
**Chọn Next để chuyển qua bước Reorder (sắp xếp thứ tự hiển thị của câu hỏi)**

<figure><img src="../../../.gitbook/assets/image (923).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
Nếu bài Test/Quiz đã có người làm, người dùng chỉ xem thông tin tại bước **Setup Score** và không thể chỉnh sửa.
{% endhint %}
{% endstep %}

{% step %}
**Tại màn hình Reorder, người dùng kiểm tra danh sách câu hỏi trong bài Test/Quiz.**

* Thứ tự mặc định là thứ tự người dùng đã tick câu hỏi tại bước **Add Question**.
* STT phản ánh thứ tự thực tế của câu hỏi trong bài Test/Quiz.

<figure><img src="../../../.gitbook/assets/image (924).png" alt=""><figcaption></figcaption></figure>

Người dùng sắp xếp lại thứ tự câu hỏi bằng một trong các cách sau:

{% tabs %}
{% tab title="Di chuyển 1 câu hỏi" %}
**Cách 1:** Kéo thả câu hỏi: Di chuyển con trỏ chuột đến icon di chuyển và nhấn giữ để thay đổi vị trí câu hỏi

<figure><img src="../../../.gitbook/assets/image (925).png" alt=""><figcaption></figcaption></figure>

**Cách 2:** Chọn **Move to top/Move to bottom**: Di chuyển câu hỏi đến vị trí đầu danh sách/cuối danh sách bằng cách chọn **Action > Move to top/Move to bottom**

<figure><img src="../../../.gitbook/assets/image (926).png" alt=""><figcaption></figcaption></figure>

**Cách 3:** Chọn **Move to position**: Di chuyển câu hỏi đến một vị trí xác định bằng cách chọn **Action > Move to position > Điền vị trí muốn chuyển câu hỏi đến > Save.**

<figure><img src="../../../.gitbook/assets/image (927).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Di chuyển nhiều câu hỏi cùng một lúc" %}
Người dùng có thể di chuyển nhóm câu hỏi khi chọn từ 2 câu hỏi liền kề trở lên.

* Ví dụ hợp lệ: 2, 3, 4, 5
* Ví dụ không hợp lệ: 1, 3, 4, 5

Người dùng có thể lựa chọn di chuyển nhóm câu hỏi này đến 1 trong các vị trí dưới đây với thao tác tương tự như khi di chuyển 1 câu hỏi:

* Đầu danh sách (Move to top)
* Cuối danh sách (Move to bottom)
* Vị trí xác định (Move to position)

<figure><img src="../../../.gitbook/assets/image (928).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
**Sau khi hoàn tất sắp xếp, chọn Finish**

Lúc này người dùng sẽ được điều hướng quay lại màn hình Test/Quiz Detail

<figure><img src="../../../.gitbook/assets/image (930).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Chọn Save để hoàn thành việc tạo bài Test/Quiz**

<figure><img src="../../../.gitbook/assets/image (932).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa bài Test/Quiz đã tạo</summary>

{% stepper %}
{% step %}
**Truy cập vào bài Test/quiz cần chỉnh sửa**

Tại màn hình chi tiết bài Test/Quiz, người dùng có thể chỉnh sửa các thông tin sau, thao tác tương tự mục _**Tạo mới bài Test/Quiz**_:

* Thông tin chung của bài Test/Quiz.
* Danh sách câu hỏi thông qua **Configure Questions**.
* Điểm của từng câu hỏi tại bước **Setup Score**.
* Thứ tự câu hỏi tại bước **Reorder**.

<figure><img src="../../../.gitbook/assets/image (933).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Sau khi hoàn tất việc chỉnh sửa, chọn Save để lưu thay đổi**

<figure><img src="../../../.gitbook/assets/image (934).png" alt=""><figcaption></figcaption></figure>

Khi bài test/quiz đã có học viên làm, người dùng chỉ được chỉnh sửa các thông tin sau:

* Tên bài Test
* Thứ tự hiển thị câu hỏi trong bài test tại bước **Reorder**.
{% endstep %}
{% endstepper %}

</details>

## III. Lưu ý & Quy tắc nghiệp vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Test/Quiz trong tài liệu này chỉ áp dụng trong phạm vi **Course**.
2. Admin cần có quyền tạo/chỉnh sửa khóa học để tạo hoặc chỉnh sửa Test/Quiz.
3. **Type of Test** quyết định danh sách câu hỏi được hiển thị tại bước Add Question.
4. Với **Multiple Choice**, hệ thống chỉ hiển thị câu hỏi trắc nghiệm.
5. Với **Constructed**, hệ thống chỉ hiển thị câu hỏi tự luận.
6. Với **Mixed**, hệ thống hiển thị cả câu hỏi trắc nghiệm và tự luận.
7. Với **Constructed/Mixed**, trường **Manual Grading** được hiển thị.
8. Với **Mocktest**, **Graded Assignment = No** trong mọi trường hợp.
9. Với **Quiz/Chapter Test/Topic Test/Midterm Test/Final Test**, nếu **Manual Grading = Yes** thì **Graded Assignment = Yes**.
10. **Total Score** có thể khác 100 nhưng phải lớn hơn 0 và phần thập phân tối đa 2 chữ số.
11. **Current Score** phải bằng **Total Score** thì Admin mới có thể chuyển sang bước Reorder.
12. **Converted Mark** được hệ thống quy đổi theo công thức: **Mark / Total Score × 100**.
13. Thứ tự câu hỏi tại Setup Score và Reorder phụ thuộc vào thứ tự Admin chọn câu hỏi tại Add Question.
14. Chỉ có thể di chuyển nhiều câu hỏi cùng lúc khi các câu hỏi được chọn nằm liền kề nhau.
15. Nếu bài Test/Quiz đã có học viên làm, Admin chỉ được chỉnh sửa tên bài Test và thứ tự câu hỏi.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nếu bài test có cả trắc nghiệm và tự luận, nên chọn **Type of Test = Mixed**.
2. Nên dùng bộ lọc **Item Set** để tìm nhanh nhóm câu hỏi theo cùng ngữ cảnh/chủ đề.
3. Nếu từng câu hỏi có trọng số khác nhau, nên dùng **Custom**.
4. Trước khi bấm **Next** tại Setup Score, nên kiểm tra **Current Score** đã bằng **Total Score** chưa.
5. Nên kiểm tra lại thứ tự câu hỏi tại bước **Reorder** trước khi bấm **Finish**.
6. Với bài Test/Quiz đã có học viên làm, nên hạn chế chỉnh sửa để tránh ảnh hưởng dữ liệu học tập.
{% endhint %}

## IV. Các lỗi thường gặp & Hướng dẫn xử lý

| Lỗi / Tình huống                                       | Nguyên nhân                                                              | Cách xử lý                                                               |
| ------------------------------------------------------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------ |
| Không tạo được Test/Quiz                               | Tài khoản chưa có quyền hoặc chưa truy cập đúng Course Content           | Kiểm tra quyền tài khoản và vị trí tạo bài test                          |
| Không thấy câu hỏi cần chọn                            | Type of Test không phù hợp với loại câu hỏi                              | Kiểm tra lại Type of Test hoặc tạo câu hỏi đúng loại trong Question Bank |
| Không tìm thấy câu hỏi                                 | Bộ lọc đang quá hẹp hoặc dữ liệu Question Bank chưa có                   | Chọn Reset hoặc kiểm tra dữ liệu Question Bank                           |
| Không chuyển được sang Reorder                         | Current Score khác Total Score                                           | Điều chỉnh Mark hoặc Total Score để hai giá trị bằng nhau                |
| Lỗi “Mark of all questions not equal \[Total Score]”   | Tổng điểm câu hỏi không bằng Total Score                                 | Kiểm tra lại Mark của từng câu hỏi hoặc Score Distribution               |
| Lỗi “MCQ Score must be between 0 and \[Total Score]”   | MCQ Score không hợp lệ                                                   | Nhập MCQ Score lớn hơn 0 và nhỏ hơn Total Score                          |
| Lỗi “Essay Score must be between 0 and \[Total Score]” | Essay Score không hợp lệ                                                 | Nhập Essay Score lớn hơn 0 và nhỏ hơn Total Score                        |
| Không thiết lập được điểm hàng loạt                    | Chưa chọn từ 2 câu hỏi trở lên hoặc Score Distribution không phải Custom | Chọn từ 2 câu hỏi trở lên và kiểm tra Score Distribution                 |
| Không di chuyển được nhiều câu hỏi                     | Các câu hỏi được chọn không liền kề                                      | Chọn các câu hỏi liền kề nhau                                            |
| Không chỉnh sửa được danh sách câu hỏi                 | Bài Test/Quiz đã có học viên làm                                         | Chỉ xem thông tin hoặc chỉ chỉnh sửa các trường được phép                |
| Thay đổi chưa được lưu                                 | Admin chưa bấm Save ở màn Test/Quiz Detail                               | Bấm **Save** sau khi hoàn tất thao tác                                   |
