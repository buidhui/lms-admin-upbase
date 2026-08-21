# Case Study

## Record of changes

\*A - Add M - Modify D - Delete

<table data-first-column-sticky><thead><tr><th>Effective Date</th><th>Update Person</th><th>A,M,D</th><th>Change Description</th><th>Version</th><th data-hidden>Effective Date</th></tr></thead><tbody><tr><td>May 18, 2026</td><td>Lê Xuân Mai</td><td>M</td><td>Chuẩn hóa nội dung lên GitBook</td><td>4.7.0</td><td>May 18, 2026</td></tr></tbody></table>

## I. Giới Thiệu Chung

### 1.1 Mục đích

Tài liệu này hướng dẫn người dùng cách sử dụng chức năng **Case Study** trong hệ thống **LMS Operations**.

Chức năng **Case Study** cho phép người dùng tạo và quản lý các tình huống học tập/đánh giá có cấu trúc từ một hoặc nhiều **Item Set**. Thông qua chức năng này, người dùng có thể xem danh sách Case Study, xem thông tin chi tiết, tạo mới, chỉnh sửa thông tin, thêm/xóa Item Set trong Case Study và thay đổi thứ tự hiển thị của các Item Set.

### 1.2 Đối tượng áp dụng

| Đối tượng | Vai trò                              | Quyền hạn                                                            |
| --------- | ------------------------------------ | -------------------------------------------------------------------- |
| Admin     | Quản trị hệ thống LMS Operations     | Có quyền quản lý toàn bộ Case Study                                  |
| Ops User  | Người dùng vận hành nội dung học tập | Có quyền xem, tạo mới, chỉnh sửa Case Study theo phân quyền được cấp |

### 1.3 Phạm vi & Module liên quan

* **Module chính:** Question Bank
* **Chức năng chính:** Case Study
* **Module liên quan:**
  * Item Set
  * Question List
  * Test / Quiz
  * Course & Materials

### 1.4 Điều kiện tiên quyết

Để sử dụng chức năng **Case Study**, người dùng cần đáp ứng các điều kiện sau:

* Người dùng đã đăng nhập thành công vào hệ thống **LMS Operations**.
* Tài khoản người dùng đã được cấp quyền truy cập module **Question Bank**.
* Tài khoản người dùng có quyền xem danh sách **Case Study**.
* Đối với thao tác tạo mới, tài khoản cần có quyền tạo mới **Case Study**.
* Đối với thao tác chỉnh sửa, tài khoản cần có quyền chỉnh sửa **Case Study**.
* Đối với thao tác thêm Item Set vào Case Study, hệ thống cần có sẵn Item Set để người dùng lựa chọn.
* Đối với thao tác chỉnh sửa thứ tự Item Set, Case Study cần có ít nhất một Item Set trong danh sách.

## II. Tổng Quan Giao Diện

<figure><img src="../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure>

Màn hình **Case Study** cho phép người dùng xem, tìm kiếm và quản lý danh sách các Case Study đã được tạo trên hệ thống. Theo user guide gốc, khi người dùng truy cập **Question Bank > Case Study**, hệ thống hiển thị danh sách Case Study theo **thời gian tạo giảm dần**.

Tại màn hình này, người dùng có thể:

* Xem danh sách Case Study hiện có.
* Tìm kiếm Case Study theo tên, tiêu chí sắp xếp hoặc khoảng thời gian.
* Mở màn hình chi tiết của một Case Study.
* Tạo mới Case Study.
* Chỉnh sửa thông tin Case Study.
* Quản lý danh sách Item Set thuộc Case Study.
* Thay đổi thứ tự hiển thị của Item Set trong Case Study.

#### Các thành phần chính trên màn hình danh sách

| Khu vực / Thành phần     | Mô tả                                                                              |
| ------------------------ | ---------------------------------------------------------------------------------- |
| **Case Study List**      | Danh sách các Case Study đã được tạo trong hệ thống.                               |
| **Vùng bộ lọc tìm kiếm** | Cho phép người dùng tìm kiếm Case Study theo điều kiện lọc.                        |
| **Search**               | Thực hiện tìm kiếm theo điều kiện đã nhập.                                         |
| **Reset**                | Xóa toàn bộ điều kiện tìm kiếm và đưa danh sách về trạng thái mặc định.            |
| **Create**               | Tạo mới một Case Study.                                                            |
| **Case Study Name**      | Tên Case Study. Người dùng có thể nhấp vào tên để xem/chỉnh sửa chi tiết.          |
| **Date**                 | Hiển thị thông tin ngày tạo/cập nhật Case Study nếu hệ thống có cấu hình hiển thị. |
| **Action/Menu thao tác** | Cho phép người dùng thực hiện các thao tác với Case Study theo quyền được cấp.     |

## III. Các Bước Thực Hiện Chi Tiết

### 3.1 Xem danh sách và thông tin chi tiết Case Study

**a. Xem danh sách và thông tin chi tiết Case Study**

_**Bước 1**_: Sau khi đăng nhập hệ thống thành công, tại mục Question Bank, người dùng nhấp vào Case Study thì danh sách các Case Study được hiển thị theo thời gian tạo giảm dần.

<figure><img src="../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: User click vào tên Case Study để xem các thông tin chi tiết bao gồm thông tin cơ bản và danh sách Item-set thuộc Case Study.

<figure><img src="../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Tại khu vực danh sách Item-set, người dùng nhấp vào tên để xem chi tiết Item-set đó.

<figure><img src="../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (126).png" alt=""><figcaption></figcaption></figure>

**b. Tìm kiếm Case Study**

Tìm kiếm theo các trường Case Study Name, Sort By, From Date - To Date

* Chọn “Search” để hiển thị các Case Study theo điều kiện tìm kiếm trên màn hình.
* Chọn “Reset” để xóa tất cả các giá trị tìm kiếm và hiển thị danh sách Case Study theo thời gian tạo.

<figure><img src="../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

### **3.2. Tạo mới Case Study** <a href="#id-3.2.-tao-moi-case-study" id="id-3.2.-tao-moi-case-study"></a>

_**Bước 1**_: Đối với trường hợp người dùng tạo mới Case Study thì mở màn hình Case Study và chọn Create.

<figure><img src="../.gitbook/assets/image (128).png" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: User thực hiện nhập các thông tin để tạo Case Study:

* Name: tên Case Study.
* Description: mô tả của Case Study.

Những trường kèm dấu '\*' là những trường thông tin bắt buộc.

<figure><img src="../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Sau khi hoàn thành điền thông tin, User click ‘Save’ để lưu, lúc này khu vực danh sách Item-set xuất hiện.

<figure><img src="../.gitbook/assets/image (130).png" alt=""><figcaption><p><em>Click Save để lưu thông tin</em></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (131).png" alt=""><figcaption><p><em>Danh sách Item-set của Case Study</em></p></figcaption></figure>

_**Bước 4**_: Người dùng click ‘Add Item-set’ để mở màn hình ‘Add Item-set’ và thêm các bộ câu hỏi vào Case Study.

<figure><img src="../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>

_**Bước 5**_: Lựa chọn Item set muốn thêm và click ‘Add’ để lưu thông tin. Sau đó người dùng sẽ được chuyển hướng về màn hình thông tin của Case Study.

<figure><img src="../.gitbook/assets/image (133).png" alt=""><figcaption><p><em>Thêm Item Set vào Case Study</em></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (134).png" alt=""><figcaption><p><em>Item set được thêm thành công vào Case Study</em></p></figcaption></figure>

### **3.3. Chỉnh sửa Case Study** <a href="#id-3.3.-chinh-sua-case-study" id="id-3.3.-chinh-sua-case-study"></a>

_**Bước 1**_: Mở màn hình Case Study và click vào bản ghi muốn chỉnh sửa.

<figure><img src="../.gitbook/assets/image (135).png" alt=""><figcaption><p><em>Click vào tên Case Study</em></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (136).png" alt=""><figcaption><p><em>Màn hình chỉnh sửa hiển thị</em></p></figcaption></figure>

_**Bước 2**_: Thực hiện nhập các thông tin để chỉnh sửa Case Study tại màn hình Case Study Detail:

* Name: tên Item Set.
* Description: Nội dung Item Set

Những trường kèm dấu '\*' là những trường thông tin bắt buộc.

<figure><img src="../.gitbook/assets/image (137).png" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Sau khi hoàn thành thay đổi thông tin, User click ‘Save’ để lưu.

_**Bước 4**_: Thực hiện thay đổi Item Set thuộc Case Study.

Người dùng có thể thực hiện thêm/xóa Item Set khỏi Case Study theo các thao tác như trong ảnh.

<figure><img src="../.gitbook/assets/image (138).png" alt=""><figcaption><p><em>Thêm Item Set vào Case Study</em></p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (139).png" alt=""><figcaption><p><em>Xóa Item Set khỏi Case Study</em></p></figcaption></figure>

### **3.4. Chỉnh sửa thứ tự của Item Set trong Case Study** <a href="#id-3.4.-chinh-sua-thu-tu-cua-item-set-trong-case-study" id="id-3.4.-chinh-sua-thu-tu-cua-item-set-trong-case-study"></a>

_**Bước 1**_: Mở màn hình Case Study và click vào bản ghi muốn chỉnh sửa thứ tự Item set.

<figure><img src="../.gitbook/assets/image (140).png" alt=""><figcaption></figcaption></figure>

_**Bước 2**_: Tại khu vực danh sách Item Set, chọn **Reorder** để chuyển đến màn hình sắp xếp thứ tự.

<figure><img src="../.gitbook/assets/image (141).png" alt=""><figcaption></figcaption></figure>

_**Bước 3**_: Thực hiện điền thứ tự mới cho các Item set trong danh sách:

* Chỉ được điền thứ tự là số nguyên dương.
* Thứ tự lớn nhất cần nhỏ hơn hoặc bằng tổng số Item set thuộc Case Study.
* Không được điền thứ tự trùng nhau.

Sau khi điền xong thì click Save để lưu thông tin, lúc này các Item set sẽ hiển thị theo thứ tự vừa thay đổi

<figure><img src="../.gitbook/assets/image (142).png" alt=""><figcaption></figcaption></figure>

## IV. Lưu Ý & Quy Tắc Nghiệp Vụ

### ⚠️ Lưu ý quan trọng

* Người dùng cần có quyền tương ứng để xem, tạo mới hoặc chỉnh sửa Case Study.
* Danh sách Case Study mặc định được hiển thị theo thời gian tạo giảm dần, người dùng có thể sử dung filter "Sort By" để sắp xếp lại thứ tự case study.
* Các trường có dấu **(\*)** là trường bắt buộc, người dùng cần nhập đầy đủ trước khi lưu.
* Case Study có thể bao gồm một hoặc nhiều Item Set.
* Sau khi tạo mới Case Study và bấm **Save**, hệ thống mới hiển thị khu vực danh sách Item Set để người dùng thêm Item Set vào Case Study.
* Khi thêm Item Set, người dùng cần chọn Item Set có sẵn trong hệ thống.
* Người dùng có thể thêm hoặc xóa Item Set khỏi Case Study tại màn hình chi tiết Case Study.
* Khi chỉnh sửa thứ tự Item Set, thứ tự nhập vào phải là số nguyên dương.
* Không được nhập thứ tự Item Set trùng nhau.
* Thứ tự lớn nhất phải nhỏ hơn hoặc bằng tổng số Item Set đang thuộc Case Study.
* Sau khi bấm **Save** tại màn hình Reorder, danh sách Item Set sẽ được hiển thị theo thứ tự mới.

### 💡 Mẹo sử dụng

* Nên đặt tên Case Study rõ ràng.
* Nên nhập mô tả ngắn gọn nhưng đủ ý để người dùng khác hiểu bối cảnh của Case Study.
* Nên chuẩn bị sẵn các Item Set trước khi tạo hoặc cấu hình Case Study.
* Nên kiểm tra lại danh sách Item Set sau khi thêm để đảm bảo đúng nội dung cần sử dụng.
* Nên sắp xếp Item Set theo đúng trình tự học tập hoặc trình tự câu hỏi mong muốn trước khi đưa Case Study vào sử dụng.
* Khi Case Study có nhiều Item Set, nên dùng chức năng **Reorder** để kiểm soát thứ tự thay vì xóa và thêm lại Item Set.
* Nên sử dụng bộ lọc **Case Study Name** hoặc khoảng thời gian để tìm nhanh Case Study khi dữ liệu nhiều.

## V. Câu Hỏi Thường Gặp

**Q: Case Study dùng để làm gì?**\
A: Case Study dùng để tạo một tình huống học tập/đánh giá gồm một hoặc nhiều Item Set. Người dùng có thể tổ chức các bộ câu hỏi theo cùng một bối cảnh hoặc kịch bản học tập.

**Q: Tôi có thể tạo Case Study khi chưa có Item Set không?**\
A: Có thể tạo thông tin cơ bản của Case Study trước. Tuy nhiên, để hoàn thiện nội dung Case Study, người dùng cần thêm các Item Set vào Case Study sau khi lưu.

**Q: Sau khi tạo Case Study, vì sao chưa thấy danh sách Item Set?**\
A: Sau khi người dùng nhập thông tin và chọn **Save**, khu vực danh sách Item Set mới xuất hiện để người dùng thêm Item Set vào Case Study.

**Q: Tôi có thể thay đổi thứ tự Item Set trong Case Study không?**\
A: Có. Người dùng chọn **Reorder** tại khu vực danh sách Item Set, nhập thứ tự mới và bấm **Save** để lưu.

**Q: Khi reorder Item Set, tôi cần lưu ý gì?**\
A: Thứ tự phải là số nguyên dương, không được trùng nhau và không được lớn hơn tổng số Item Set trong Case Study.
