# GaitLab – hướng dẫn cho Claude khi sửa trang

Chủ trang: bác sĩ Nguyễn Thành Nhu (giảng viên Phục hồi chức năng). Trang học liệu phân tích định tính dáng đi.
Bác sĩ Nhu quyết MỌI nội dung y khoa. Claude chỉ sửa đúng điều bác sĩ yêu cầu, không tự thêm, bớt hay đổi nghĩa chuyên môn.

## Vai trò
Claude giúp bác sĩ Nhu bảo trì, quản lý, nâng cấp và phát triển trang GaitLab. Mọi nội dung y khoa vẫn do bác sĩ quyết.

## Trang gồm gì
- Chỉ có MỘT tệp `index.html` (khoảng 900 KB), tự chứa đủ: giao diện, bài học, câu hỏi, lời giải. Không cần cài gì để chạy: mở bằng trình duyệt là thấy.
- Nội dung bài học nằm trong phần dữ liệu JavaScript của tệp (28 bài chia 3 học phần: Nền tảng, Quan sát, Lập luận lâm sàng; thêm Thực hành, Tài liệu, Tiến độ). Muốn sửa một câu: tìm đúng câu đó bằng chức năng tìm chuỗi, sửa tại chỗ.
- Video và một số ảnh nằm ở máy chủ khác, trang chỉ trỏ tới. Đừng đổi địa chỉ các video.
- Trang đăng công khai bằng GitHub Pages: mỗi lần lưu thay đổi vào nhánh chính, sau vài phút trang thật cập nhật.

## Cách sửa an toàn (làm đúng thứ tự)
1. Hỏi lại cho chắc chữ cũ và chữ mới. Tìm chuỗi cũ: nếu khớp nhiều chỗ thì liệt kê và hỏi bác sĩ chỗ nào đổi, đừng đổi hàng loạt.
2. Chỉ thay đúng chỗ được yêu cầu. KHÔNG dựng lại hay viết lại cả tệp.
3. Không đổi các mã định danh bài (đường dẫn dạng `#/hoc/...`), vì sẽ làm hỏng liên kết.
4. Sửa xong: mở trang bằng trình duyệt, kiểm chữ mới hiện đúng, chữ cũ biến mất, mở thử vài bài liên quan, trang không báo lỗi.
5. Lưu thay đổi kèm lời nhắn ngắn nói đã sửa gì. Có lịch sử nên sai thì quay lại được bản trước.
6. Báo bác sĩ: đã đổi mấy chỗ, ở bài nào; chỗ nào không tìm thấy hoặc chưa chắc.

## Quy ước chữ bác sĩ đã chốt (giữ nhất quán)
- Dùng "video" (không dùng "phim"); "khung hình" (không chỉ "khung"); "người trưởng thành", "người bệnh" (không "người đi bộ", "người đi").
- Dùng "sàn" (chạm sàn, rời sàn, mặt sàn), không "đất".
- Dùng "thoát sàn" và "khoảng hở thoát sàn" cho foot clearance.
- Dùng "chân đối bên"; "xương bánh chè" (không rút gọn "bánh chè").
- "Dụng cụ hỗ trợ" (không "dụng cụ trợ giúp").
- Tên giai đoạn: "Đáp ứng tải". Nhiệm vụ chức năng: "Tiếp nhận trọng lượng". Cụm động từ: "khi tiếp nhận tải".
- Giữ tiêu đề mục 4.3.7 như hiện tại ("Dáng đi bước cao và bàn chân rủ").
- "nhận tải" / "nhận trọng lượng" đứng một mình (không có "tiếp" ngay trước): dùng "chịu tải" và "chịu sức nặng" (bác sĩ chốt 22/11/2026). Không viết "nhận tải" hay "nhận trọng lượng" đứng một mình nữa. Giữ nguyên "tiếp nhận tải", "Tiếp nhận trọng lượng" / "tiếp nhận trọng lượng" và tên giai đoạn "Đáp ứng tải".

## Đưa lên mạng
- Sửa trực tiếp trên nhánh `main`, hoặc mở PR rồi gộp (merge) vào `main`.
- GitHub Pages tự cập nhật sau khoảng 1-3 phút.
- Kiểm tra trang thật tại https://noah-ntn.github.io/gaitlab

## Việc Claude KHÔNG tự làm
- Không sửa nội dung y khoa, đáp án, số liệu khi bác sĩ chưa nói rõ.
- Không xoá video, ảnh, bài học.
- Không đổi địa chỉ máy chủ video.
- Không đưa mật khẩu, khoá bí mật vào tệp.
