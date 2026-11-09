# Bài 3: Sử dụng AI an toàn khi xử lí lỗi phần mềm 
## Báo cáo phân tích theo mô hình IPO:

>Khi gặp lỗi "Path not found" lúc cài Python và nhận được một lệnh lạ từ AI, em áp dụng mô hình IPO để kiểm chứng thông tin như sau:

-  **Input (Đầu vào):**

Đề xuất từ AI: Một đoạn lệnh gạch đầu dòng bảo copy dán vào Terminal/Command Prompt để sửa lỗi PATH.

Nguy cơ nghi vấn: Lệnh trông lạ, tác động sâu vào biến môi trường hệ thống và có thể bị hiện tượng AI "bốc phét" (AI Hallucination) hoặc nhầm lẫn giữa hệ điều hành Windows với macOS/Linux.

-  **Process (Quy trình kiểm chứng):**

   - Em không vội chạy lệnh ngay mà thực hiện kiểm chứng qua 2 bước:

      - Tra cứu trên StackOverflow bằng toán tử tìm kiếm nâng cao:

      - Cú pháp tìm kiếm: **"[Tên_câu_lệnh_lạ]" site:stackoverflow.com**

Mục đích: Xem cộng đồng lập trình viên có ai từng dùng lệnh này để sửa lỗi "Path not found" của Python chưa, có ai cảnh báo nguy hiểm hay thả vote âm không.

Đối chiếu với trang tài liệu chính thức (Official Docs):

Cú pháp tìm kiếm: **"environment variables" site:docs.python.org**

Mục đích: Kiểm tra cách thêm Python vào PATH chuẩn xác theo khuyến cáo từ trang chủ Python xem có trùng khớp với logic câu lệnh của AI hay không.

-  **Output (Kết quả đánh giá):**

Trường hợp An toàn: Nếu lệnh được xác nhận trên StackOverflow có nhiều lượt upvote và khớp với tài liệu docs.python.org, em mới copy vào Terminal để chạy.

Trường hợp Không an toàn / Ảo giác: Nếu tìm trên StackOverflow không ra kết quả, hoặc lệnh này dành cho Linux nhưng máy em chạy Windows, em sẽ hủy bỏ lệnh đó và không chạy trên máy.
---

## Thiết kế Prompt "Hỏi ngược lại" AI trước khi thực thi:

- Để bắt AI tự giải thích và làm rõ độ an toàn của câu lệnh, em dùng câu prompt sau:

  - "Trước khi tôi chạy lệnh này, bạn hãy giải thích rõ:

  - Từng từ khóa/tham số trong lệnh trên có tác dụng gì cụ thể?

   - Lệnh này dành cho hệ điều hành nào (Windows, macOS hay Linux)?

   - Lệnh này có chỉnh sửa, xóa hay ghi đè lên file hệ thống quan trọng nào không?

   - Nếu không chắc chắn 100%, hãy đưa cho tôi cách sửa lỗi 'Path not found' bằng giao diện đồ họa (GUI) an toàn hơn."