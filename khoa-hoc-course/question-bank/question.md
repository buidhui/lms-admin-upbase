# Question

## I. Thông tin chung

{% hint style="info" %}
**Dành cho:** Admin, Ops User

**Đường dẫn:** [https://ops.sapp.edu.vn/question-bank/question](https://ops.sapp.edu.vn/question-bank/question)
{% endhint %}

{% hint style="info" %}
#### Phạm vi & Module liên quan

* **Module chính:** Question Bank
* **Chức năng chính:** Question / Câu hỏi
* **Module liên quan:** Item Set, Case Study, Test / Quiz
{% endhint %}

{% hint style="warning" %}
#### Điều kiện tiên quyết:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản đã được cấp quyền truy cập module **Question Bank** và quyền thao tác với câu hỏi.
{% endhint %}

## II. Hướng dẫn chi tiết

<details>

<summary>Xem danh sách và thông tin chi tiết câu hỏi</summary>

{% stepper %}
{% step %}
**Truy cập Question Bank → Item Set List**

Sau khi đăng nhập thành công, tại mục Question Bank người dùng nhấp vào **Item Set List**. Danh sách các Item Set hiển thị theo thời gian tạo giảm dần.

<figure><img src="../../.gitbook/assets/image (45).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Xem thông tin chi tiết Item Set / câu hỏi**

Click vào tên Item Set để xem thông tin chi tiết, bao gồm thông tin cơ bản và danh sách câu hỏi thuộc Item Set (Question List).

<figure><img src="../../.gitbook/assets/image (47).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Preview câu hỏi**

Để xem trước câu hỏi hiển thị bên giao diện học viên, chọn nút **Action** tương ứng với câu hỏi muốn xem và chọn **Preview**.

<figure><img src="../../.gitbook/assets/image (79).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (80).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Tìm kiếm câu hỏi**

Tìm kiếm theo các trường Item Set Name, Sort By, From Date - To Date.

* Chọn **Search** để hiển thị kết quả theo điều kiện tìm kiếm.
* Chọn **Reset** để xóa tất cả giá trị tìm kiếm và hiển thị danh sách theo thời gian tạo.

<figure><img src="../../.gitbook/assets/image (46).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Tạo mới câu hỏi</summary>

{% stepper %}
{% step %}
**Chọn Add single question và chọn loại câu hỏi**

Người dùng có thể tạo câu hỏi đơn lẻ bằng cách chọn **Add single question** tại màn hình danh sách Item Set.

<figure><img src="../../.gitbook/assets/image (81).png" alt=""><figcaption></figcaption></figure>

Màn hình hiển thị hộp thoại chọn loại câu hỏi gồm 8 loại:

* Đúng/sai
* Một lựa chọn
* Nhiều lựa chọn
* Ghép đáp án
* Chọn từ
* Điền từ
* Kéo thả
* Tự luận

<figure><img src="../../.gitbook/assets/image (82).png" alt=""><figcaption></figcaption></figure>

Đối với câu hỏi cần soạn, Admin có thể chọn loại câu hỏi tự phản chiếu bằng cách chọn **Yes** tại **Self Reflection**. Câu hỏi tự phản chiếu áp dụng được với cả 8 dạng câu hỏi.

<figure><img src="../../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
**Nhập dữ liệu câu hỏi theo loại đã chọn**

{% tabs %}
{% tab title="Đúng/Sai" %}
Tại màn hình Create True/False question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*)
* Danh sách đáp án (\*): gồm 2 lựa chọn, 1 lựa chọn Đúng và 1 lựa chọn Sai.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

Những trường kèm dấu '\*' là những trường thông tin bắt buộc.

<figure><img src="../../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (86).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Một lựa chọn" %}
Tại màn hình Create One Choice question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*)
* Danh sách đáp án (\*): gồm nhiều lựa chọn, trong đó có 1 đáp án Đúng và các đáp án còn lại là Sai.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

Những trường kèm dấu '\*' là những trường thông tin bắt buộc.

<figure><img src="../../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (88).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Nhiều lựa chọn" %}
Tại màn hình Create One Choice question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*)
* Danh sách đáp án (\*): gồm nhiều lựa chọn, trong đó có ít nhất 2 đáp án Đúng và các đáp án còn lại là Sai.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (89).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (90).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Ghép đáp án" %}
Tại màn hình Create Matching question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*)
* Danh sách đáp án (\*): gồm 2 phần, các bộ đáp án bị trống ở 1 trong 2 cột hoặc cả 2 cột đều sẽ bị hệ thống bỏ qua:
  * Đáp án
  * Đáp án tương ứng
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Chọn từ" %}
Tại màn hình Create Select Word question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*): Mỗi \[dấu ngoặc vuông] được hiểu là một chỗ trống để học viên chọn đáp án.
* Danh sách đáp án (\*): Tương ứng với từng chỗ trống. Mỗi chỗ trống là một nhóm các đáp án, cần có ít nhất 1 đáp án đúng trong một chỗ trống. Người làm bài chỉ cần chọn 1 đáp án trong các đáp án đúng sẽ được tính là trả lời đúng câu hỏi.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (93).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (94).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Điền từ" %}
Tại màn hình Create Fill Up question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*): Mỗi \[dấu ngoặc vuông] được hiểu là một chỗ trống để học viên nhập đáp án.
* Danh sách đáp án (\*): Các đáp án đúng tương ứng với từng chỗ trống. Mỗi chỗ trống có thể có 1 hoặc nhiều đáp án đúng. Người làm bài chỉ cần chọn 1 đáp án trong các đáp án đúng sẽ được tính là trả lời đúng câu hỏi.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (95).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (96).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Kéo thả" %}
Tại màn hình Create Drag Drop question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi (\*): Mỗi \[dấu ngoặc vuông] được hiểu là một chỗ trống để học viên chọn đáp án.
* Danh sách đáp án (\*): Số lượng đáp án luôn lớn hơn hoặc bằng số lượng ô trống. Các đáp án tương ứng với từng ô trống là đáp án đúng của ô trống đó, còn lại là đáp án gây nhiễu.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (97).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (98).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Tự luận" %}
Tại màn hình Create Constructed question, người dùng nhập dữ liệu:

* Question Level (\*): độ khó của câu hỏi, chọn 1 trong các giá trị cho trước.
* Question Layout (\*): cách thức hiển thị câu hỏi bên phía giao diện học viên, chọn 1 trong các giá trị cho trước.
* Question Category (\*): phân loại câu hỏi, chọn 1 trong các giá trị cho trước.
* Assignment Type (\*): loại bài tập, chọn 1 trong các giá trị cho trước
* Response Option (\*): hình thức trả lời câu hỏi, chọn 1 trong các giá trị cho trước
* Câu hỏi tự do: chọn ô này để đánh dấu đây là câu hỏi tự do.
* Belong to (\*): (không hiển thị với câu hỏi tự do) dùng để xác định câu hỏi thuộc cấu phần học nào, bao gồm: Course, Section, Subsection, Unit, Activity. Người dùng cần điền lần lượt theo thứ tự từ trái sang phải.
* Nội dung câu hỏi
* Requirements (\*): câu hỏi nhỏ của câu tự luận.
* Exhibit/Time Value Tables: tài liệu cho câu hỏi (chỉ áp dụng cho các câu hỏi cũ, với các câu hỏi mới thì không còn thông tin này)
* Answer Template: Được sử dụng để thiết lập sẵn mẫu trả lời dưới dạng Word/Excel cho từng câu hỏi hoặc từng Requirement. Khi template được tạo, học viên có thể làm bài trực tiếp trên mẫu này thay vì phải soạn thảo từ đầu.
* Solution (\*): lời giải cho chi tiết cho câu hỏi.
* Gợi ý
* Tag

<figure><img src="../../.gitbook/assets/image (99).png" alt=""><figcaption></figcaption></figure>

Nếu câu tự luận có câu hỏi nhỏ thì điền nội dung câu hỏi trường ‘Requirement’, bỏ trống trường ‘Nội dung câu hỏi’

<figure><img src="../../.gitbook/assets/image (100).png" alt=""><figcaption></figcaption></figure>

Trong trường hợp User muốn thêm file **Answer Template** cho câu hỏi không có nhiều requirement, user click vào biểu tượng drop down để hiển thị vùng _add answer template_.

<figure><img src="../../.gitbook/assets/image (101).png" alt=""><figcaption><p>User click vào icon drop down để thực hiện thêm Answer Template</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (103).png" alt=""><figcaption><p>Vùng add Answer Template cho câu hỏi không có requiement</p></figcaption></figure>

* Trường thông tin _Answer Template Type_ được hiển thị dựa trên lựa chọn _Response Option_. Cụ thể, nếu người dùng chọn _Response Option_ là Word, hệ thống sẽ cho phép thêm _Answer Template_ dưới dạng Word; ngược lại, nếu chọn Excel, hệ thống sẽ cho phép thêm _Answer Template_ dưới dạng Excel.
* _**Cách 1:**_ Người dùng chọn chức năng Upload File để tải lên file template Word/Excel tương ứng với Answer Template Type.
  * Sau khi upload thành công, hệ thống hiển thị file tại vùng Preview để người dùng xem trước và có thể chỉnh sửa trực tiếp.
  * Trường hợp muốn xóa file Word/Excel vừa tải lên, người dùng click vào icon thùng rác bên cạnh tên file trên giao diện.

<figure><img src="../../.gitbook/assets/image (105).png" alt=""><figcaption><p>Tải file Word/Excel từ máy tính</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (107).png" alt=""><figcaption><p>Chọn file Word/Excel từ Resource</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (108).png" alt=""><figcaption><p>Giao diện Preview hiển thị template đã được tải lên</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (109).png" alt=""><figcaption><p>Xóa file template vừa tải</p></figcaption></figure>

* _**Cách 2:**_ User thao tác trực tiếp trên giao diện tại vùng “Preview”.

<figure><img src="../../.gitbook/assets/image (110).png" alt=""><figcaption><p>Tạo Answer Template trực tiếp trên giao diện Preview</p></figcaption></figure>

Trong trường hợp câu hỏi có nhiều Requirement, nếu người dùng muốn thêm file Answer Template, tại popup **Add More Requirements** họ click vào biểu tượng Dropdown để mở vùng thêm **Answer Template**.\
Sau khi vùng này hiển thị, người dùng tiến hành thiết lập template trả lời tương tự như quy trình đối với câu hỏi không có Requirement.

<figure><img src="../../.gitbook/assets/image (111).png" alt=""><figcaption><p>User click vào icon drop down để thực hiện thêm Answer Template</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (112).png" alt=""><figcaption><p>Vùng add Answer Template cho từng Requirement</p></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
**Lưu câu hỏi**

Sau khi hoàn thành nhập dữ liệu, người dùng chọn:

* **Save:** lưu câu hỏi.
* **Save & New:** lưu câu hỏi và tiếp tục tạo câu hỏi mới.
* **Preview:** xem trước câu hỏi vừa tạo.
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Chỉnh sửa câu hỏi</summary>

{% stepper %}
{% step %}
**Mở màn hình chỉnh sửa câu hỏi**

Đối với single question: tại màn hình danh sách câu hỏi, nhấp vào tên câu hỏi để chuyển đến màn hình chỉnh sửa.

<figure><img src="../../.gitbook/assets/image (113).png" alt=""><figcaption><p><em>Click vào nội dung câu hỏi</em></p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (113).png" alt=""><figcaption><p><em>Click vào nội dung câu hỏi</em></p></figcaption></figure>

Đối với question trong Item Set: tại màn hình Item Set Detail > Question List, nhấp vào tên câu hỏi để chuyển đến màn hình chỉnh sửa.

<figure><img src="../../.gitbook/assets/image (115).png" alt=""><figcaption><p><em>Click vào nội dung câu hỏi tại màn Item Set Detail</em></p></figcaption></figure>
{% endstep %}

{% step %}
**Chỉnh sửa thông tin và lưu**

Thực hiện chỉnh sửa các trường thông tin của câu hỏi, sau đó click **Save** để lưu.

<figure><img src="../../.gitbook/assets/image (116).png" alt=""><figcaption></figcaption></figure>

Việc chỉnh sửa phụ thuộc vào trạng thái câu hỏi:

* Câu hỏi **chưa có học viên làm**: được chỉnh sửa toàn bộ thông tin.
* Câu hỏi **đã có học viên làm**: từng loại câu hỏi có những trường được phép chỉnh sửa khác nhau (Y: được chỉnh sửa, N: không).

|                      | **Đúng/Sai** | **Một lựa chọn** | **Nhiều lựa chọn** | **Ghép đáp án** | **Chọn từ** | **Điền Từ** | **Drag Drop** | **Tự luận** |
| -------------------- | ------------ | ---------------- | ------------------ | --------------- | ----------- | ----------- | ------------- | ----------- |
| **Question Level**   | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Self Reflection**  | N            | N                | N                  | N               | N           | N           | N             | N           |
| **Question Layout**  | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Question Type**    | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Câu hỏi tự do**    | N            | N                | N                  | N               | N           | N           | N             | N           |
| **Belong To**        | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Nội Dung Câu Hỏi** | Y            | Y                | Y                  | Y               | N           | N           | N             | Y           |
| **Danh Sách Đáp Án** | N            | N                | N                  | N               | N           | N           | N             | N           |
| **Explanation**      | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Gợi ý**            | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
| **Tag**              | Y            | Y                | Y                  | Y               | Y           | Y           | Y             | Y           |
{% endstep %}
{% endstepper %}

</details>

<details>

<summary>Xóa câu hỏi</summary>

{% stepper %}
{% step %}
**Điều kiện xóa câu hỏi**

* Người dùng đăng nhập thành công vào hệ thống.
* Tài khoản có quyền xóa câu hỏi.
* Câu hỏi chưa được thêm vào bài Test/Quiz.
{% endstep %}

{% step %}
**Chọn Action → Delete**

Tại màn hình danh sách câu hỏi muốn xóa, nhấp nút **Action** và chọn **Delete**.

<figure><img src="../../.gitbook/assets/image (118).png" alt=""><figcaption><p>Xóa câu hỏi tại question list</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/image (119).png" alt=""><figcaption><p>Xóa câu hỏi tại Item Set Detail</p></figcaption></figure>
{% endstep %}

{% step %}
**Xác nhận xóa**

Click **Yes** khi hộp thoại xuất hiện để đồng ý xóa câu hỏi.

<figure><img src="../../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>

{% hint style="warning" %}
Không thể xóa những câu hỏi đã được thêm vào Test/Quiz/Case Study.
{% endhint %}
{% endstep %}
{% endstepper %}

</details>

## III. Lưu Ý & Quy Tắc Nghiệp Vụ

{% hint style="warning" %}
### Lưu ý quan trọng

1. Người dùng cần được cấp quyền tương ứng để tạo mới, chỉnh sửa, xóa hoặc xem chi tiết câu hỏi.
2. Câu hỏi có thể được tạo theo 2 cách: **Add single question** (câu hỏi đơn lẻ) hoặc **Create Question** tại màn hình chi tiết Item Set.
3. Hệ thống hỗ trợ 8 loại câu hỏi: Đúng/Sai, Một lựa chọn, Nhiều lựa chọn, Ghép đáp án, Chọn từ, Điền từ, Kéo thả, Tự luận.
4. Các trường có dấu **(\*)** là trường bắt buộc, cần nhập đầy đủ trước khi lưu.
5. Trường **Belong to** xác định câu hỏi thuộc cấu phần học (Course, Section, Subsection, Unit, Activity); không hiển thị với câu hỏi tự do.
6. **Self Reflection** áp dụng cho cả 8 dạng câu hỏi; với câu hỏi đã có học viên làm, trường này không được chỉnh sửa.
7. Với câu hỏi **Chọn từ, Điền từ, Kéo thả**, mỗi nội dung trong **\[dấu ngoặc vuông]** là một chỗ trống.
8. Với câu hỏi **Ghép đáp án**, các bộ đáp án bị trống ở một hoặc cả hai cột sẽ bị hệ thống bỏ qua.
9. Với câu hỏi **Tự luận** có nhiều câu hỏi nhỏ, nhập nội dung tại **Requirement** và bỏ trống **Nội dung câu hỏi**.
10. **Answer Template** cho phép thiết lập mẫu trả lời Word/Excel; loại file hiển thị theo **Response Option**. Có thể upload file hoặc tạo trực tiếp tại vùng **Preview**.
11. Khi tạo câu hỏi có thể chọn **Save**, **Save & New** hoặc **Preview**.
12. Chỉnh sửa câu hỏi phụ thuộc trạng thái: chưa có học viên làm → sửa toàn bộ; đã có học viên làm → chỉ sửa một số trường theo loại câu hỏi.
13. Không thể xóa câu hỏi đã được thêm vào **Test / Quiz / Case Study**. Sau khi xác nhận xóa, dữ liệu có thể không khôi phục được trên giao diện người dùng.
{% endhint %}

{% hint style="info" %}
### Mẹo sử dụng

1. Nên dùng bộ lọc tại **Question List** (Question Type, Course, Section, Subsection, Unit, Activity, Item Set, Tag, From/To date) để tìm nhanh câu hỏi.
2. Nên đặt **Question Category**, **Question Level** và **Tag** rõ ràng để thuận tiện tìm kiếm, phân loại, tái sử dụng.
3. Trước khi lưu, nên dùng **Preview** để kiểm tra cách câu hỏi hiển thị ở giao diện học viên.
4. Với câu hỏi nhiều đáp án, nên kiểm tra kỹ đáp án đúng/sai trước khi lưu, vì khi đã dùng trong Test/Quiz một số thông tin sẽ bị giới hạn chỉnh sửa.
5. Nên chọn **Belong to** theo đúng thứ tự Course → Section → Subsection → Unit → Activity.
6. Với câu hỏi **Chọn từ/Điền từ/Kéo thả**, nên kiểm tra số lượng dấu **\[ ]** trước khi nhập đáp án.
7. Với câu hỏi **Kéo thả**, nên chuẩn bị số đáp án ≥ số ô trống (phần dư làm đáp án gây nhiễu).
8. Với câu hỏi **Tự luận** cần trả lời theo mẫu, nên thiết lập **Answer Template**.
9. Nên dùng **Save & New** khi cần tạo nhiều câu hỏi liên tiếp.
10. Trước khi xóa, nên kiểm tra câu hỏi đã được dùng trong Test/Quiz/Case Study hay chưa.
{% endhint %}

## IV. Các Lỗi Thường Gặp & Cách Xử Lý

| Lỗi / Tình huống                          | Nguyên nhân                                                  | Cách xử lý                                                                   |
| ----------------------------------------- | ------------------------------------------------------------ | ---------------------------------------------------------------------------- |
| Không lưu được câu hỏi                    | Chưa nhập đủ các trường bắt buộc (\*)                        | Kiểm tra và nhập đầy đủ các trường có dấu (\*) rồi bấm Save                  |
| Không tìm thấy câu hỏi                    | Sai điều kiện lọc tìm kiếm                                   | Kiểm tra lại bộ lọc, bấm Reset để về danh sách mặc định                      |
| Không thấy trường Belong to               | Câu hỏi đang được đánh dấu là **Câu hỏi tự do**              | Bỏ chọn "Câu hỏi tự do" nếu cần gắn câu hỏi vào cấu phần học                 |
| Một số trường không chỉnh sửa được        | Câu hỏi đã có học viên làm, bị giới hạn theo loại câu hỏi    | Đối chiếu ma trận chỉnh sửa; tạo câu hỏi mới nếu cần thay đổi trường bị khóa |
| Đáp án câu Ghép đáp án bị thiếu           | Bộ đáp án trống ở một hoặc cả hai cột nên bị hệ thống bỏ qua | Nhập đầy đủ cả hai cột cho mỗi cặp đáp án                                    |
| Số đáp án câu Kéo thả không hợp lệ        | Số đáp án nhỏ hơn số ô trống                                 | Bổ sung đáp án để số đáp án ≥ số ô trống                                     |
| Answer Template Type không đúng định dạng | Chưa chọn đúng **Response Option** (Word/Excel)              | Chọn Response Option phù hợp trước khi thêm Answer Template                  |
| Không xóa được câu hỏi                    | Câu hỏi đã được thêm vào Test/Quiz/Case Study                | Gỡ câu hỏi khỏi Test/Quiz/Case Study trước khi xóa                           |
