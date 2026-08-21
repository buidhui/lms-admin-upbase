# Chấm điểm bằng AI

#### Tổng quan chức năng chấm điểm tự luận bằng AI

Chấm điểm tự luận bằng AI là tính năng cho phép hệ thống sử dụng AI (Gemini) **tự động chấm điểm các câu hỏi tự luận** ngay sau khi học viên nộp bài. AI dựa trên **Rubric File** (cơ chế chấm điểm), **Context Files** (bối cảnh khóa học) và nội dung bài làm để đưa ra điểm số và nhận xét, giúp Mentor tiết kiệm thời gian và tăng tính nhất quán khi chấm bài. Tính năng áp dụng cho các khóa học có **Program Category = "ACCA"**.

Quy trình vận hành gồm 3 luồng tuần tự: **SX cài đặt** dữ liệu đầu vào cho AI (Grading Files, Context File, bài Test/Quiz); **AI tự động chấm** khi học viên nộp bài và **Mentor review** lại kết quả; khi cần, Mentor có thể **yêu cầu AI chấm lại** hoặc theo dõi các câu bị lỗi. Kết quả chỉ được gửi cho học viên sau khi Mentor phụ trách bấm **"Finish"** hoàn tất chấm bài.

Tài liệu chi tiết được tách theo từng vai trò/luồng nghiệp vụ:

* **Cài đặt chấm điểm bằng AI (SX)** — Upload Grading Files cho câu hỏi tự luận, Context File cho khóa học và cấu hình bài Test/Quiz để AI chấm tự động.
* **AI tự động chấm & Mentor review (Mentor)** — Diễn biến sau khi học viên nộp bài, xem và chỉnh sửa kết quả AI, hoàn tất chấm bài.
* **Chấm lại bằng AI & theo dõi lỗi (Mentor)** — Yêu cầu AI Regrade từng câu, AI Grade All toàn bài và theo dõi AI Grading Failures.
* **Học viên xem kết quả chấm (Học viên)** — Xem điểm, nhận xét và các Grading Files sau khi Mentor hoàn tất.
