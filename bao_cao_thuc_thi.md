BÁO CÁO PHÂN TÍCH & THIẾT KẾ GIẢI PHÁP (BƯỚC 1)
1. Phân tích bài toán
Bối cảnh: Trung tâm/cửa hàng giáo dục cần tự động hóa quy trình đánh giá năng lực hiểu bài của học viên thông qua Kỹ thuật Feynman (học viên tự giải thích lại kiến thức bằng ngôn ngữ đơn giản) kết hợp Rubric chấm điểm tự động.

Thách thức (Bẫy dữ liệu): Học viên có thể nộp bài trống, viết lan man lạc đề, hoặc cố tình chèn các câu lệnh đánh lừa AI (Prompt Injection) để xin điểm cao. Ngoài ra, dữ liệu chuẩn (tài liệu gốc/barem điểm) có thể bị thiếu khiến AI tự suy diễn (hallucination).

2. Thiết kế kiến trúc Input / Output (I/O)
A. Dữ liệu đầu vào (INPUT):

{{SUBJECT_TOPIC}}: Tên chủ đề hoặc môn học đang kiểm tra.

{{SOURCE_MATERIAL}}: Tài liệu chuẩn / Đáp án gốc dùng làm căn cứ đối chiếu.

{{RUBRIC_CRITERIA}}: Thang điểm và tiêu chí đánh giá (Độ chính xác, Tính đơn giản/dễ hiểu, Ví dụ minh họa).

{{STUDENT_EXPLANATION}}: Bài giải thích theo phương pháp Feynman của học viên.

B. Cấu trúc đầu ra (OUTPUT):
Hệ thống xuất kết quả theo định dạng chuẩn hóa (Markdown có cấu trúc rõ ràng hoặc JSON) gồm 4 phần bắt buộc:

Trạng thái kiểm tra dữ liệu (Validation Status): Xác nhận dữ liệu hợp lệ hoặc báo mã lỗi cụ thể.

Bảng chấm điểm theo Rubric: Điểm số chi tiết từng tiêu chí + Tổng điểm.

Phân tích lỗ hổng kiến thức (Feynman Gap Analysis): Chỉ ra phần học viên hiểu sai, hiểu mơ hồ hoặc dùng thuật ngữ quá hàn lâm chưa được đơn giản hóa.

Phản hồi gia sư & Gợi ý cải thiện: Lời khuyên mang tính khích lệ và câu hỏi gợi mở để học viên tự sửa bài.
