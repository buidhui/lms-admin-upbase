# Tạo bài Test/Quiz cho khóa học

## Record of changes

_A - Add M - Modify D - Delete_

| Effective Date | Update Person | A,M,D | Change Description             | Version |
| -------------- | ------------- | ----- | ------------------------------ | ------- |
| May 20, 2026   | Lê Xuân Mai   | M     | Chuẩn hóa nội dung lên GitBook | 4.7.0   |

## I. Giới Thiệu Chung

**Dành cho:** Admin, SX

**Đường dẫn:** [https://ops.sapp.edu.vn/courses?page\_index=1\&page\_size=10](https://ops.sapp.edu.vn/courses?page_index=1\&page_size=10)

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

#### Điều kiện tiên quyết

* Admin đã đăng nhập thành công vào hệ thống OPS.
* Tài khoản Admin có quyền tạo hoặc chỉnh sửa khóa học.
* Khóa học đã được tạo thành công ở bước **Course Info**.

## II. Hướng dẫn chi tiết

### Tạo mới bài Test/Quiz

{% stepper %}
{% step %}
## Nhập thông tin bài test

**Sau khi chọn loại bài test, Admin cần nhập các thông tin cho bài test như ảnh sau:**

![](<.gitbook/assets/image (1011)>)

| Tên trường thông tin | Mô tả                                                                                                                                                                                                                                                                                                        |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Name                 | Nhập tên bài test                                                                                                                                                                                                                                                                                            |
| Type of Test         | <p>Loại bài kiểm tra:<br><br>- Multiple Choice: Dạng bài trắc nghiệm<br>- Constructed: Dạng bài tự luận<br>- Mixed (Multiple Choice + Constructed): Dạng bài mix, bao gồm cả trắc nghiệm và tự luận.<br>- Mặc định chọn Multiple Choice</p>                                                                  |
| Test Mode            | <p>Admin chọn một trong hai loại bài test dưới đây:<br><br>- Tutor: cho phép học viên làm bài không giới hạn thời gian<br>- Timed: giới hạn thời gian làm bài → Nếu Admin chọn Timed, màn hình hiển thị Duration yêu cầu Admin nhập thời gian cho phép làm bài theo giờ và phút<br>- Mặc định chọn Tutor</p> |
| Manual Grading       | <p>Chỉ hiển thị với Type of Test = Constructed/Mixed (Multiple Choice + Constructed)<br><br>- Yes: bài kiểm tra sẽ được chấm điểm thủ công bởi đội SX.<br>- No: bài kiểm tra sẽ được hệ thống chấm điểm tự động.</p>                                                                                         |
| Graded Assignment    | <p>Đánh dấu bài kiểm tra được sử dụng để tính điểm cho toàn bộ khóa học, gồm 2 giá trị:<br><br>- Yes<br>- No</p>                                                                                                                                                                                             |
| Grading Preference   | <p>Chọn cách hiển thị đáp án và Solution<br><br>- After each question: hiển thị sau khi trả lời mỗi câu hỏi<br>- After all questions: hiển thị sau khi hoàn thành bài test<br>- Mặc định chọn After all questions</p>                                                                                        |
| Pass Point           | <p>Điểm pass bài test<br><br>- Auto 50%: điểm pass point là 50%<br>- Manual: cho phép Admin nhập số điểm pass point → Nếu Admin chọn ‘Manual’ màn hình hiển thị textbox cho phép Admin nhập số điểm<br>- Mặc định chọn Auto 50%</p>                                                                          |
| Attempt              | <p>Cho phép chọn số lần làm bài<br><br>- Unlimited: không giới hạn số lần làm bài<br>- Limited: giới hạn số lần làm bài → Nếu Admin chọn ‘Limited' màn hình hiển thị textbox cho phép Admin nhập số lần học viên được phép nộp bài<br>- Mặc định chọn Unlimited</p>                                          |
| Total Score          | <p>- Tổng điểm của bài Test/Quiz, có thể điền khác thang điểm 100.<br>- Chỉ nhập giá trị lớn hơn 0.<br>- Phần thập phân tối đa 2 chữ số.</p>                                                                                                                                                                 |

Với các loại bài kiểm tra là Quiz/Chapter test/Topic Test/Midterm test/Final test, khi người dùng chọn Manual Grading = ‘Yes’ thì giá trị của Graded Assigment = ‘Yes’.

Với loại bài kiểm tra là Mocktest thì giá trị của Graded Assignment = 'No' trong mọi trường hợp.
{% endstep %}

{% step %}
## Cài đặt câu hỏi

**Admin thực hiện cài đặt câu hỏi cho bài test bằng cách click Configure Questions, gồm 3 bước:**

* Add Question: thêm câu hỏi vào bài Test/Quiz
* Setup Score: cài đặt điểm cho bài test và cho từng câu hỏi trong bài Test
* Reorder: sắp xếp thứ tự hiển thị của câu hỏi trong bài test.

![](<.gitbook/assets/image (1012)>)
{% endstep %}

{% step %}
## Thêm câu hỏi

**Admin chọn "Add Question" để cài đặt thông tin câu hỏi cho bài Test/Quiz**

Tại bước **Add Question**, màn hình hiển thị danh sách câu hỏi đã được tạo trên hệ thống theo loại bài Test/Quiz mà người dùng đã chọn trước đó (Multiple choice, Constructed hoặc Mixed)

![](<.gitbook/assets/image (1013)>)

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

**Danh sách câu hỏi hiển thị phụ thuộc vào Type of Test.**

* Type of Test = Multiple Choice: Hệ thống hiển thị toàn bộ câu hỏi trắc nghiệm trên hệ thống.
* Type of Test = Constructed Question: Hệ thống hiển thị toàn bộ câu hỏi tự luận trên hệ thống.
* Type of Test = Mixed: Hệ thống hiển thị cả câu hỏi trắc nghiệm và câu hỏi tự luận.

**Cách sắp xếp:**

* Câu hỏi được nhóm theo **Item Set**.
* Item Set được tạo gần đây nhất hiển thị ở đầu danh sách.
* Các câu hỏi trong cùng một Item Set được sắp xếp theo thời gian tạo từ gần đến xa.
* Câu hỏi trắc nghiệm và tự luận có thể hiển thị xen kẽ theo đúng thứ tự tạo trong Item Set.
{% endstep %}

{% step %}
## Chọn câu hỏi

**Admin thực hiện tick chọn các câu hỏi cần thêm vào bài test**

Số lượng câu hỏi đã chọn được hiển thị ở góc màn hình như ảnh sau:

![](<.gitbook/assets/image (1014)>)

Thứ tự câu hỏi tại bước **Setup Score** và **Reorder** phụ thuộc vào thứ tự người dùng chọn câu hỏi tại bước **Add Question**.

| Trường hợp                                          | Logic hệ thống                                                          |
| --------------------------------------------------- | ----------------------------------------------------------------------- |
| Người dùng chọn đơn lẻ từng câu                     | Câu nào được chọn trước sẽ đứng trước                                   |
| Người dùng chọn toàn bộ câu hỏi trong trang         | Thứ tự câu hỏi giữ nguyên như thứ tự đang hiển thị tại màn Add Question |
| Người dùng chọn một câu, sau đó bỏ chọn và chọn lại | Câu hỏi đó được đưa xuống cuối danh sách                                |
{% endstep %}

{% step %}
## Thêm câu hỏi và tạo bài test

**Admin click button Add & Create để thêm câu hỏi, tạo bài test theo thông tin đã cài đặt trước đó, đồng thời chuyển sang bước Setup Score.**

Nếu bài Test/Quiz đã có người làm, người dùng chỉ xem thông tin tại bước Add Question và không thể chỉnh sửa.
{% endstep %}

{% step %}
## Thiết lập điểm cho bài Test/Quiz

### Setup Score: Thiết lập điểm cho câu hỏi

**Tại màn hình Setup Score, người dùng cài đặt thông tin điểm của bài Test/Quiz.**

Màn hình gồm 2 khu vực chính:

1. Khu vực cài đặt điểm cho bài Test/Quiz.
2. Khu vực hiển thị danh sách câu hỏi.

![](<.gitbook/assets/image (1015)>)

Người dùng thực hiện điền thông tin tại Khu vực cài đặt điểm cho toàn bộ bài Test/Quiz.

Các trường thông tin bao gồm:

| Trường thông tin   | Mô tả                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Total Score        | <p>Tổng điểm tối đa của bài Test/Quiz, cho phép người dùng điền số lớn hơn 0 và có thể khác 100.<br><br>Khi thay đổi Total Score, hệ thống sẽ tự động tính lại toàn bộ điểm của từng Question (Mark) nếu Score Distribution = Evenly across all questions hoặc Evenly by Question Type</p>                                                                                                                                                                        |
| Current Score      | <p>Tổng điểm hiện tại của toàn bộ câu hỏi, hệ thống tự tính:<br><br>- Nếu Tổng điểm của toàn bộ câu hỏi trong bài test <strong>lớn hơn</strong> hoặc <strong>nhỏ hơn</strong> Total Score: khi ấn Next để chuyển sang bước 3 báo lỗi ‘Mark of all questions not equal [Total Score]’<br>- Nếu Tổng điểm của toàn bộ câu hỏi trong bài test <strong>bằng</strong> Total Score: click Next chuyển sang bước tiếp theo thành công</p>                                |
| Score Distribution | <p>Cách phân phối điểm cho từng câu hỏi, chọn 1 trong 3 giá trị:<br><br>- Evenly across all questions: Hệ thống tự động chia đều <strong>Total Score</strong> cho toàn bộ câu hỏi trong bài Test/Quiz.<br>- Evenly by Question Type (MCQ/Essay): cài đặt điểm cho nhóm câu hỏi trắc nghiệp (MCQ) và câu hỏi tự luận (Essay), sau đó hệ thống sẽ tự chia đều điểm cho các câu hỏi trong từng nhóm.<br>- Custom: người dùng tự chỉnh sửa điểm của từng câu hỏi.</p> |
| MCQ Score          | <p>Tổng điểm dành cho các câu hỏi trắc nghiệm, chỉ hiển thị nếu Score Distribution = Evenly by Question Type (MCQ/Essay).<br><br>Chỉ điền số lớn hơn 0 và nhỏ hơn Total Score, nếu không thỏa mãn thì khi click Next sang bước tiếp theo báo lỗi bên dưới trường thông tin như sau ‘MCQ Score must be between 0 and [Total Score]’</p>                                                                                                                            |
| Essay Score        | <p>Tổng điểm dành cho các câu hỏi tự luận, chỉ hiển thị nếu Score Distribution = Evenly by Question Type (MCQ/Essay)<br><br>Chỉ điền số lớn hơn 0 và nhỏ hơn Total Score, nếu không thỏa mãn thì khi click Next sang bước tiếp theo báo lỗi bên dưới trường thông tin như sau ‘Essay Score must be between 0 and [Total Score]’</p>                                                                                                                               |
{% endstep %}

{% step %}
## Cài đặt điểm cho từng câu hỏi

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

          ![](<.gitbook/assets/image (1016)>)
      *   Click vào nút **Setup Score** và điền điểm tại popup, sau đó chọn **Save** để lưu

          ![](<.gitbook/assets/image (1017)>)
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
## Chuyển sang bước Reorder

**Chọn Next để chuyển qua bước Reorder (sắp xếp thứ tự hiển thị của câu hỏi)**

![](<.gitbook/assets/image (1018)>)

Nếu bài Test/Quiz đã có người làm, người dùng chỉ xem thông tin tại bước **Setup Score** và không thể chỉnh sửa.
{% endstep %}

{% step %}
## Sắp xếp thứ tự câu hỏi

**Tại màn hình Reorder, người dùng kiểm tra danh sách câu hỏi trong bài Test/Quiz.**

* Thứ tự mặc định là thứ tự người dùng đã tick câu hỏi tại bước **Add Question**.
* STT phản ánh thứ tự thực tế của câu hỏi trong bài Test/Quiz.

![](<.gitbook/assets/image (1019)>)

Người dùng sắp xếp lại thứ tự câu hỏi bằng một trong các cách sau:

#### Di chuyển 1 câu hỏi

**Cách 1:** Kéo thả câu hỏi: Di chuyển con trỏ chuột đến icon di chuyển và nhấn giữ để thay đổi vị trí câu hỏi

![](<.gitbook/assets/image (1020)>)

**Cách 2:** Chọn **Move to top/Move to bottom**: Di chuyển câu hỏi đến vị trí đầu danh sách/cuối danh sách bằng cách chọn **Action > Move to top/Move to bottom**

![](<.gitbook/assets/image (1021)>)

**Cách 3:** Chọn **Move to position**: Di chuyển câu hỏi đến một vị trí xác định bằng cách chọn **Action > Move to position > Điền vị trí muốn chuyển câu hỏi đến > Save.**

![](<.gitbook/assets/image (1022)>)

#### Di chuyển nhiều câu hỏi cùng một lúc

Người dùng có thể di chuyển nhóm câu hỏi khi chọn từ 2 câu hỏi liền kề trở lên.

* Ví dụ hợp lệ: 2, 3, 4, 5
* Ví dụ không hợp lệ: 1, 3, 4, 5

Người dùng có thể lựa chọn di chuyển nhóm câu hỏi này đến 1 trong các vị trí dưới đây với thao tác tương tự như khi di chuyển 1 câu hỏi:

* Đầu danh sách (Move to top)
* Cuối danh sách (Move to bottom)
* Vị trí xác định (Move to position)

![](<.gitbook/assets/image (1023)>)
{% endstep %}

{% step %}
## Hoàn tất sắp xếp

**Sau khi hoàn tất sắp xếp, chọn Finish**

Lúc này người dùng sẽ được điều hướng quay lại màn hình Test/Quiz Detail

![](<.gitbook/assets/image (1024)>)
{% endstep %}

{% step %}
## Lưu bài Test/Quiz

**Chọn Save để hoàn thành việc tạo bài Test/Quiz**

![](<.gitbook/assets/image (1025)>)
{% endstep %}
{% endstepper %}

### Chỉnh sửa bài Test/Quiz đã tạo

{% stepper %}
{% step %}
## Truy cập bài Test/Quiz cần chỉnh sửa

**Truy cập vào bài Test/quiz cần chỉnh sửa**

Tại màn hình chi tiết bài Test/Quiz, người dùng có thể chỉnh sửa các thông tin sau, thao tác tương tự mục _**Tạo mới bài Test/Quiz**_:

* Thông tin chung của bài Test/Quiz.
* Danh sách câu hỏi thông qua **Configure Questions**.
* Điểm của từng câu hỏi tại bước **Setup Score**.
* Thứ tự câu hỏi tại bước **Reorder**.

![](<.gitbook/assets/image (1026)>)
{% endstep %}

{% step %}
## Lưu thay đổi

**Sau khi hoàn tất viecj chỉnh sửa, chọn Save để lưu thay đổi**

![](<.gitbook/assets/image (1027)>)

Khi bài test/quiz đã có học viên làm, người dùng chỉ được chỉnh sửa các thông tin sau:

* Tên bài Test
* Thứ tự hiển thị câu hỏi trong bài test tại bước **Reorder**.
{% endstep %}
{% endstepper %}

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

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

### Mẹo sử dụng

1. Nếu bài test có cả trắc nghiệm và tự luận, nên chọn **Type of Test = Mixed**.
2. Nên dùng bộ lọc **Item Set** để tìm nhanh nhóm câu hỏi theo cùng ngữ cảnh/chủ đề.
3. Nếu từng câu hỏi có trọng số khác nhau, nên dùng **Custom**.
4. Trước khi bấm **Next** tại Setup Score, nên kiểm tra **Current Score** đã bằng **Total Score** chưa.
5. Nên kiểm tra lại thứ tự câu hỏi tại bước **Reorder** trước khi bấm **Finish**.
6. Với bài Test/Quiz đã có học viên làm, nên hạn chế chỉnh sửa để tránh ảnh hưởng dữ liệu học tập.

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

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
