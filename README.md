---
cover: >-
  https://images.unsplash.com/photo-1785228861910-afa6c4197203?crop=entropy&cs=srgb&fm=jpg&ixid=M3wxOTcwMjR8MHwxfHJhbmRvbXx8fHx8fHx8fDE3ODcyODc0NDZ8&ixlib=rb-4.1.0&q=85
coverY: 0
layout:
  width: default
  cover:
    visible: true
    size: hero
    mask: none
  title:
    visible: true
  description:
    visible: false
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: true
  actions:
    visible: true
---

# Welcome to LMS Ops - UpBase

#### LMS Ops là gì?

LMS Ops là hệ thống quản lý vận hành toàn bộ hoạt động đào tạo — từ lúc học viên đăng ký học cho đến khi hoàn thành khóa học và nhận chứng chỉ. Hệ thống này là công cụ làm việc hàng ngày của các bộ phận Admin, CX, SX và lễ tân, để các bộ phận cùng làm việc trên một nguồn dữ liệu duy nhất.

***

#### Tài liệu này dành cho ai?

| Đối tượng                  | Vai trò trong LMS Ops                                                                                         |
| -------------------------- | ------------------------------------------------------------------------------------------------------------- |
| **Business / Management**  | Theo dõi tổng quan vận hành qua Dashboard, nắm luồng xử lý giữa các bộ phận                                   |
| **CX – Vận hành lớp học**  | Tạo và vận hành lớp học, xếp lịch, quản lý giảng viên,...                                                     |
| **SX – Sản xuất nội dung** | Xây dựng khóa học, ngân hàng câu hỏi, bài kiểm tra, chứng chỉ, chấm điểm, hỗ trợ học viên trả lời comment,... |

***

#### Luồng vận hành tổng quan

LMS Ops được thiết kế xuyên suốt theo **hành trình học tập của học viên**, chia làm 3 giai đoạn chính:

**1. Trước khi học viên bắt đầu học**

Toàn bộ công tác chuẩn bị: xây dựng nội dung khóa học, thiết lập tài khoản người dùng, tạo lớp học, phân công giảng viên, xếp lịch và phòng học, đồng thời xử lý đăng ký học — từ đồng bộ dữ liệu HubSpot, thu học phí, đến kiểm tra đầu vào và mở lớp chính thức.

**2. Trong quá trình học viên học**

Vận hành lớp học hàng ngày: theo dõi tiến độ học trên LMS, quản lý lịch nghỉ lễ, hỗ trợ học viên qua support ticket, giám sát tiến độ giảng viên và thực hiện chấm điểm.

**3. Sau khi học viên học xong**

Thông báo kết quả học tập, cấp chứng chỉ hoàn thành và tổng hợp số liệu lên Dashboard để theo dõi hiệu quả vận hành. Kết quả giai đoạn này cũng là đầu vào cho việc tái đăng ký hoặc mở lớp tiếp theo.

<figure><img src=".gitbook/assets/image (1)" alt=""><figcaption><p>Luồng tổng quan quản lý hành trình học tập của học viên trên LMS Ops</p></figcaption></figure>

#### Một số điểm cần lưu ý khi sử dụng tài liệu này

**Tài liệu được tổ chức theo module**, mỗi module tương ứng với một nhóm chức năng trong hệ thống LMS Ops. Người dùng có thể đọc toàn bộ hoặc tra cứu module liên quan đến công việc của mình.

**Màu sắc trong sơ đồ luồng** phân biệt bộ phận phụ trách từng khối tác vụ — vàng là TVTS, xanh lá là CX, xanh dương là SX, tím là hệ thống tự động. Khi phối hợp liên bộ phận, cần chú ý điểm giao tiếp giữa các màu trong luồng.

**Dữ liệu giữa các module có liên kết chặt chẽ** — ví dụ thông tin học viên từ bước Enrollment sẽ tự động ảnh hưởng đến lớp học, lịch học và bảng điểm. Vì vậy việc nhập liệu đúng ở đầu luồng rất quan trọng để tránh sai lệch ở các bước sau.
