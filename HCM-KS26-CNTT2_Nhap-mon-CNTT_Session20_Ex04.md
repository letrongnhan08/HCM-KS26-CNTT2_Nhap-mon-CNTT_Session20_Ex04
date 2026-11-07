**Bài 4 : Đánh giá công cụ hỗ trợ xử lý lỗi lập trình** 

| Tiêu chí               | Google Search (StackOverflow)                                                                                                              | AI Assistant                                                                                                            |
| :--------------------- | :----------------------------------------------------------------------------------------------------------------------------------------- | :---------------------------------------------------------------------------------------------------------------------- |
| Độ chính xác           | Dựa trên thử nghiệm thực tế, được cộng đồng kiểm chứng (upvote/tick xanh)                                                                  | Hiểu nhanh cấu trúc mã lỗi, nhưng hay đưa ra giải pháp tổng hợp chắp vá, nhưng dễ sai lệch với kiến trúc dự án phức tạp |
| Tính cập nhật          | Tức thời, phản ánh ngay các lỗi từ bản cập nhật mới nhất                                                                                   | Bị giới hạn cập nhật kiến thức do thời gian dữ liệu huấn luyện                                                          |
| Khả năng giải thích    | Phụ thuộc vào người trả lời, thường cung cấp mã lệnh để dùng ngay. Người dùng phải tự đọc nhiều bài viết, chắt lọc thông tin và thử nghiệm | Rất chi tiết, giải thích rõ cơ chế từng lệnh và dễ dàng hỏi đáp thêm                                                    |
| Rủi ro (Hallucination) | Thấp. Chỉ có rủi ro áp dụng nhầm bài viết cũ,không có tích xanh hoặc không có upvote                                                       | Có nguy cơ bịa đặt tham số dòng lệnh hoặc file cấu hình không tồn tại                                                   |

**Trường hợp bắt buộc phải dùng Google Search để đảm bảo an toàn:**

\-Khi gặp các lỗi bảo mật, lỗ hổng: Phải dùng Google để tra cứu các báo cáo bảo mật chính thống,có mã độc không, không nên tin AI 100% vì nó có thể đưa ra giải quyết chung chung hoặc bị Hallucination nói làm tiến trình đó cho hệ thống hợp lệ rồi khẳng định là an toàn và hiệu quả,sẽ khiến mình làm sai và gây nguy hiểm  bảo mật.

\-Thực thi lệnh hệ thống quyền cao (Root/Admin): Cần dùng Google đối chiếu tài liệu chính thức trước khi chạy các lệnh ép buộc dừng tiến trình, tránh việc AI cấp sai tham số làm sập hệ thống hoặc mất dữ liệu.  
