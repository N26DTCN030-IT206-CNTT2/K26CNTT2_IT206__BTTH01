KẾT QUẢ CHẠY THỬ NGHIỆM (TEST CASES)
Để chứng minh prompt hoạt động hiệu quả cả trong tình huống chuẩn lẫn tình huống bẫy dữ liệu, bạn nên đưa 2 kịch bản chạy thử sau vào báo cáo:

Kịch bản 1: Dữ liệu hợp lệ (Học viên giải thích có lỗ hổng)
Dữ liệu nạp vào (Input):

Chủ đề: Nguyên lý hoạt động của Blockchain.

Tài liệu chuẩn: Blockchain là một cơ sở dữ liệu phân tán lưu trữ thông tin dưới dạng các khối (block) được liên kết với nhau bằng mã hóa (hash) theo trình tự thời gian. Dữ liệu đã ghi vào khối thì gần như không thể sửa đổi vì nếu sửa một khối sẽ làm thay đổi mã hash và phá vỡ liên kết với toàn bộ các khối phía sau.

Rubric: (1) Độ chính xác kiến thức: 4đ; (2) Tính đơn giản, dễ hiểu (Feynman): 4đ; (3) Ví dụ minh họa: 2đ. Tổng: 10đ.

Bài của học viên: "Blockchain giống như một cuốn sổ cái công khai mà ai cũng giữ một bản sao. Mỗi trang sổ là một block. Khi viết đầy trang thì người ta dùng thuật toán mật mã băm (cryptographic hash function) để khóa nó lại và nối sang trang mới. Vì vậy không ai ăn gian sửa số liệu được."

``` Kết quả phản hồi thực tế của AI (Output):
1. TRẠNG THÁI DỮ LIỆU
Trạng thái: Hợp lệ (Sẵn sàng đánh giá)
2. BẢNG ĐIỂM RUBRIC CHI TIẾT
| Tiêu chí đánh giá | Điểm đạt được | Điểm tối đa | Nhận xét ngắn gọn |
| :--- | :---: | :---: | :--- |
| Độ chính xác kiến thức | 3.5 | 4.0 | Nắm được tính phân tán, cấu trúc khối và tính bất biến. Thiếu ý liên kết theo trình tự thời gian. |
| Tính đơn giản, dễ hiểu (Feynman) | 3.0 | 4.0 | Hình ảnh "cuốn sổ cái" rất dễ hiểu, nhưng còn dùng thuật ngữ "cryptographic hash function" mà chưa giải thích. |
| Ví dụ minh họa | 2.0 | 2.0 | Ví dụ so sánh với cuốn sổ cái trực quan, sát thực tế. |
| **TỔNG ĐIỂM** | **8.5** | **10.0** | **Giỏi** |

3. PHÂN TÍCH LỖ HỔNG FEYNMAN (GAP ANALYSIS)
Điểm làm tốt: Bạn đã sử dụng phép ẩn dụ "cuốn sổ cái ai cũng giữ một bản sao"
để giải thích cực kỳ dễ hiểu khái niệm cơ sở dữ liệu phân tán.
Lỗ hổng kiến thức / Diễn đạt tối nghĩa:

Bạn dùng cụm từ "thuật toán mật mã băm (cryptographic hash function)" — một người mới học sẽ không hiểu từ này nghĩa là gì.

Bạn chưa giải thích rõ tại sao lại không sửa được số liệu (cơ chế thay đổi mã làm đứt gãy chuỗi phía sau).

4. GỢI Ý TỪ GIA SƯ AI
Lời khuyên cải thiện: Thay vì gọi tên thuật toán băm,
bạn có thể ví nó như một "dấu vân tay duy nhất" của trang sổ đó.
Câu hỏi gợi mở (Feynman Prompt): Nếu một người cố tình tẩy xóa một con số ở trang số 2 trong cuốn sổ này,
chuyện gì sẽ xảy ra với "dấu vân tay" của trang số 2 và các trang số 3, 4 tiếp theo?
```





