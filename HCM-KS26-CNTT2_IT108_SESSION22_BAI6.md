### 1. Viết Prompt nhờ AI giải thích lỗi (Công thức 3 thành phần)

Để nhờ AI giải thích nguyên nhân lỗi `error: open(".git/FETCH_HEAD"): Permission denied` một cách dễ hiểu nhất, em sử dụng công thức Prompt 3 thành phần (**Vai trò - Bối cảnh & Nhiệm vụ - Yêu cầu đầu ra**):

> **Prompt mẫu:**
> 
> "Bạn là một người anh khóa trên thân thiện chuyên dạy lập trình cho sinh viên năm nhất.
> 
> Tôi đang cần push code gấp lên GitHub cho kịp deadline bài tập thì Terminal báo lỗi: `error: open(".git/FETCH_HEAD"): Permission denied`. Tôi đã thử tắt đi chạy lại nhưng vẫn bị lỗi này.
> 
> Hãy giải thích cho tôi nguyên nhân gây ra lỗi này bằng ngôn ngữ cực kỳ bình dân, dễ hiểu (dùng ví dụ thực tế) và gợi ý cách khắc phục nhanh nhất trên Windows."

---

### 2. Mô phỏng minh họa hướng dẫn Run as Administrator & Quy tắc chụp ảnh

AI hướng dẫn em mở Terminal/Command Prompt dưới quyền **Run as Administrator** (Chạy với quyền Quản trị viên).

```text
+-------------------------------------------------------------------------+
| [Search Windows] > gõ "cmd" hoặc "PowerShell"                           |
|  ├── Click chuột phải > Chọn "Run as Administrator"                     |
|  └── [Chụp ảnh màn hình minh họa]                                        |
+-------------------------------------------------------------------------+
```

#### **Các lưu ý bảo mật & chuyên nghiệp khi chụp ảnh màn hình gửi bài/nhờ hỗ trợ:**

* **Khoanh vùng lỗi chính:** Dùng khung màu đỏ hoặc vàng khoanh rõ dòng thông báo lỗi `error: open(".git/FETCH_HEAD"): Permission denied` để người xem thấy ngay vấn đề.
* **Che/Bảo mật thông tin cá nhân (Blur/Censorship):**
  * Che thông tin đường dẫn thư mục chứa tên thật hoặc mã số sinh viên (ví dụ: `C:\Users\LeGiaBao_MSSV123\...`).
  * Che thông tin Personal Access Token hoặc đường dẫn SSH Key cá nhân (nếu có hiện trên màn hình).
* **Cắt gọn màn hình (Crop):** Chỉ chụp khung cửa sổ Terminal và các bước thao tác, không chụp toàn bộ màn hình máy tính chứa ứng dụng cá nhân (Facebook, Zalo, game...).

---

### 3. Soạn tin nhắn nhờ Giảng viên hỗ trợ (Theo Bug Reporting Framework)

Nếu đã thử chạy quyền Administrator mà vẫn bị lỗi, em sẽ nhắn tin nhờ Thầy/Cô hỗ trợ theo đúng mẫu chuẩn:

```text
Kính gửi Thầy/Cô [Tên Giảng Viên],

Em là Lê Gia Bảo - MSSV: [N26DTCN006], sinh viên lớp [HCM-KS26-CNTT2].

Em đang gặp sự cố khi đẩy bài tập lên GitHub và cần sự hỗ trợ của Thầy/Cô. Em xin gửi thông tin chi tiết báo lỗi như sau ạ:

1. Bối cảnh (Context):
- Em đang thực hiện lệnh `git pull` / `git push` bài tập lớn môn Nhập môn CNTT.
- Hệ điều hành: Windows 11, dùng Git Bash / Terminal.

2. Kết quả kỳ vọng (Expected):
- Git kết nối thành công với GitHub và đẩy code mới lên repository của bài tập.

3. Thực tế xảy ra (Actual):
- Terminal liên tục báo lỗi phân quyền: error: open(".git/FETCH_HEAD"): Permission denied.
- Em đã thử chạy Terminal bằng quyền "Run as Administrator" và khởi động lại máy nhưng vẫn không hết lỗi.

4. Log chi tiết & Ảnh chụp màn hình (Log/Screenshot):
- Mã lỗi: error: open(".git/FETCH_HEAD"): Permission denied / fatal: cannot update HEAD
- Em xin gửi kèm ảnh chụp màn hình thông báo lỗi (đã khoanh vùng lỗi cụ thể) ở phía dưới ạ.

Em cảm ơn Thầy/Cô rất nhiều ạ!
```