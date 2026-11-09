# Bài 2: Xử lý lỗi thư viện mã nguồn bằng Github Issues

## Cách lọc và ưu tiên đọc bình luận trên Github Issues:
- **Ưu tiên bình luận có nhiều lượt thả tim và thumbs up:** Mấy bình luận này nhận được nhiều tim hay nút Like là do những người gặp lỗi trước đó đã làm theo thành công nên người ta bấm cảm ơn. 
- **Được người quản lí Repo ghim hoặc có nhãn Owner/Maintainer:** Mấy người chủ dự án thường sẽ ghim câu trả lời chuẩn nhất lên trên cùng để mọi người bấm vào là thấy.
- **Bình luận ngắn gọn, chỉ rõ vị trí sửa code:** Thường các bình luận xịn sẽ ghi luôn là sửa ở dòng nào, thay đổi file cấu hình ra sao hoặc đổi phiên bản thư viện về bản nào là hết lỗi. 
--- 
## Khái niệm Workaround và lí do không nên ngồi đợi cập nhật:
- **Workaround là gì?**
>Workaround hiểu nôm na là một "mẹo chữa cháy" hoặc cách lách lỗi tạm thời. Nó giúp chương trình của mình chạy tiếp được ngay lúc đó chứ chưa phải là sửa tận gốc trong thư viện của nhà sản xuất.
- **Tại sao không nên ngồi đợi bản cập nhật chính thức?**
>- **Dễ trễ deadline bài tập/dự án:** Để nhóm phát triển ra được một bản vá chính thức (patch/update) thì họ phải kiểm tra kỹ nhiều thứ nên mất thời gian. Em không thể dừng làm bài để ngồi chờ họ được.
 >- **Không biết chính xác khi nào họ mới sửa xong:** Dự án mã nguồn mở làm vì cộng đồng nên có lỗi sửa trong vài tiếng, nhưng cũng có lỗi cả tháng chưa ai đụng tới.
>- **Đảm bảo công việc không bị gián đoạn:** Dùng Workaround giúp em và nhóm tiếp tục viết tiếp các chức năng khác. Sau này khi nhà sản xuất ra bản cập nhật mới thì chỉ cần chạy lệnh update thư viện rồi xoá đoạn code chữa cháy đi là xong.