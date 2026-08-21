# yeu cau cua giang vien teacher request

Tính năng **Teacher Request** cho phép đội vận hành quản lý các đề xuất liên quan đến lịch làm việc, lịch dạy và định mức giảng dạy của giảng viên trên hệ thống **OPS/LMS Operations**.

Thông qua tính năng này, người dùng có thể xem danh sách yêu cầu, kiểm tra thông tin chi tiết, tạo mới, chỉnh sửa, duyệt, từ chối hoặc hủy các đề xuất của giảng viên theo phạm vi được phân quyền.

Các yêu cầu của giảng viên được chia thành 2 nhóm chính:

| Nhóm yêu cầu                  | Mô tả                                                                                        |
| ----------------------------- | -------------------------------------------------------------------------------------------- |
| **Personal Schedule Request** | Quản lý các đề xuất cá nhân của giảng viên, bao gồm **Busy Schedule** và **Weekly Norm**.    |
| **Timeoff Request**           | Quản lý các đề xuất liên quan đến buổi dạy, bao gồm **Timeoff** và **Teaching Mode Change**. |

Trong đó:

| Loại yêu cầu             | Mô tả                                                                               |
| ------------------------ | ----------------------------------------------------------------------------------- |
| **Busy Schedule**        | Giảng viên đăng ký lịch bận để hệ thống ghi nhận thời gian không thể nhận lịch dạy. |
| **Weekly Norm**          | Giảng viên đăng ký hoặc điều chỉnh định mức số buổi dạy trong tuần.                 |
| **Timeoff**              | Giảng viên gửi yêu cầu xin nghỉ một hoặc một số buổi dạy đã được phân công.         |
| **Teaching Mode Change** | Giảng viên gửi yêu cầu đổi hình thức dạy đối với buổi học Offline.                  |

Mỗi yêu cầu có thể có các trạng thái như **Pending**, **Approved**, **Rejected** hoặc **Cancelled**. Khi trạng thái yêu cầu thay đổi, hệ thống sẽ cập nhật dữ liệu liên quan như lịch giảng viên, lịch lớp học, lịch phòng học, đồng thời gửi thông báo tới giảng viên qua LMS theo từng trường hợp nghiệp vụ.

Tính năng này giúp đội vận hành kiểm soát tốt hơn lịch dạy của giảng viên, hạn chế trùng lịch, đảm bảo việc thay đổi lịch dạy được ghi nhận có quy trình và đồng bộ với các lịch liên quan trên hệ thống.
