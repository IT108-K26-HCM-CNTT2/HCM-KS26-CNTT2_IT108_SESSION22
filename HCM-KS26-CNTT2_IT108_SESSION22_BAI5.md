### 1. Mẫu Bug Report Template (Dành cho nhóm)

Để tránh việc mọi người nhắn tin trôi bài hoặc hỏi chung chung kiểu *"Chị ơi máy em bị lỗi rồi"*, mỗi khi gặp sự cố về môi trường (Docker, đụng Port...), thành viên bắt buộc phải điền theo mẫu 4 phần này trước khi gửi vào nhóm chat:

```text
[BÁO LỖI / NÊU CÂU HỎI]

1. Context (Bối cảnh):
- Đang làm phần nào / chạy lệnh gì?
- Hệ điều hành & môi trường: (Ví dụ: Windows 11, Docker v24, Node.js v18)

2. Expected (Kỳ vọng):
- Đúng ra hệ thống phải chạy như thế nào? (Ví dụ: Web chạy ở localhost:3000)

3. Actual (Thực tế xảy ra):
- Thực tế đang bị sao? (Ví dụ: Báo lỗi đụng cổng 3000, không nhấp vào web được)

4. Log / Screenshot (Mã lỗi chi tiết):
- Dán đoạn log lỗi Terminal hoặc gửi ảnh chụp màn hình chỗ bị lỗi ở đây:
...
```

---

### 2. Quy trình 3 bước tra cứu bắt buộc (Tự xử lý 80% lỗi trước khi hỏi)

Trước khi gửi tin nhắn nhờ nhóm hỗ trợ, các thành viên phải tự mình đi qua 3 bước này:

```text
Bước 1: Googling (Tìm kiếm bằng cú pháp nâng cao)
   │
   ▼
Bước 2: Community Search (Tra cứu GitHub Issues / StackOverflow)
   │
   ▼
Bước 3: AI Translation & Explain (Nhờ AI giải thích & hướng dẫn)
```

#### **Bước 1: Googling (Tìm kiếm với toán tử nâng cao)**
* **Cách làm:** Coppy nguyên văn dòng thông báo lỗi ngắn gọn nhất quăng lên Google.
* **Mẹo:** Dùng dấu ngoặc kép và loại trừ các trang rác.
* *Ví dụ:* `"port 3000 is already in use" filetype:md -tailieu`

#### **Bước 2: Community Search (Tìm trên GitHub Issues / StackOverflow)**
* **Cách làm:** Nếu tìm Google chung chung không ra, khoanh vùng tìm kiếm trực tiếp trên các diễn đàn kỹ thuật uy tín.
* *Ví dụ:* `"Docker port conflict" site:stackoverflow.com` hoặc `"Port already allocated" site:github.com`
* **Lưu ý:** Ưu tiên đọc các bài viết có gắn nhãn "Windows 11" hoặc có nhiều tim/thumbs up.

#### **Bước 3: AI Translation & Explain (Dùng AI dịch & giải thích log lỗi)**
* **Cách làm:** Nếu đoạn log lỗi dài quá đọc không hiểu, copy toàn bộ dòng Log đó quăng cho ChatGPT / Gemini và nhờ dịch ra tiếng Việt.
* **Prompt mẫu:** *"Dịch đoạn log lỗi này sang tiếng Việt, giải thích nguyên nhân tại sao bị và gợi ý 2 cách sửa bằng câu lệnh cho hệ điều hành Windows 11 giúp tôi."*

> 💡 **Quy định chung:** Nếu đã đi hết 3 bước trên (tốn khoảng 10-15 phút) mà vẫn chưa sửa được thì mới lấy thông tin đã gom được điền vào **Bug Report Template** ở phần 1 rồi post lên nhóm để nhờ anh/chị hỗ trợ!