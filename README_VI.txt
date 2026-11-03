NUCLEAR WATCH – PWA ANDROID – BẢN 0.1

ĐÂY LÀ GÌ?
- PWA tiếng Việt, cài được từ Chrome Android khi được lưu trữ qua HTTPS.
- Tổng hợp bài báo công khai từ GDELT DOC API theo 3 nhóm truy vấn: nguy cơ hạt nhân, tên lửa đạn đạo, sự kiện hạt nhân/phóng xạ.
- Phân loại theo từ khóa để ưu tiên đọc; KHÔNG phải đánh giá tình báo, xác suất chiến tranh hoặc cảnh báo tên lửa.
- Có cache giao diện cơ bản để mở lại khi mất mạng.

GIỚI HẠN QUAN TRỌNG
1. Bản này chưa có máy chủ, chưa có push notification nền 24/7. Thông báo thử nghiệm chỉ hoạt động khi người dùng cấp quyền; trình duyệt có thể giới hạn thông báo khi ứng dụng đóng.
2. Dữ liệu GDELT là tin báo chí được lập chỉ mục; có thể trễ, trùng, thiếu, sai, hoặc không truy cập được do mạng/CORS/dịch vụ bên thứ ba.
3. Từ khóa trong tiêu đề không chứng minh có phóng tên lửa, đầu đạn hạt nhân hay vụ tấn công.
4. Không tự động tạo cảnh báo đỏ. Luôn xác minh bằng cơ quan chức năng và nhiều nguồn độc lập.
5. Không thay thế cảnh báo khẩn cấp của Việt Nam hoặc hướng dẫn của cơ quan cứu hộ.

CÁCH ĐƯA LÊN MẠNG MIỄN PHÍ
1. Tạo tài khoản GitHub nếu chưa có.
2. Tạo repository PUBLIC tên nuclear-watch (GitHub Pages miễn phí cho repository public).
3. Giải nén toàn bộ thư mục này và tải các file/thư mục bên trong lên repository, giữ nguyên cấu trúc.
4. Vào Settings > Pages.
5. Ở Build and deployment chọn Deploy from a branch; chọn branch main và folder /(root), nhấn Save.
6. Đợi GitHub Pages xuất bản. Mở URL dạng https://TEN-TAI-KHOAN.github.io/nuclear-watch/ bằng Chrome Android.
7. Trong Chrome nhấn menu ⋮ > Install app hoặc Add to Home screen.

LƯU Ý: GitHub Pages public nghĩa là mã nguồn ứng dụng công khai. Không đưa thông tin cá nhân, khóa bí mật hoặc dữ liệu riêng tư vào repository.

KIỂM TRA
- Mở trang và nhấn “Cập nhật tin”.
- Nếu không có dữ liệu, thử lại sau; dịch vụ GDELT hoặc kết nối có thể tạm thời không phản hồi.
- Nhấn “Bật thông báo trên máy” để thử quyền thông báo khi trang đang mở.

NÂNG CẤP ĐỂ CÓ PUSH NỀN
Cần một backend chạy lịch định kỳ, lưu trạng thái bài mới, đánh giá nguồn, và gửi Web Push qua VAPID tới subscription của trình duyệt. Có thể thử gói miễn phí của một nhà cung cấp, nhưng hạn mức và điều kiện thay đổi; không thể cam kết miễn phí hoặc 24/7 vĩnh viễn. Không nên triển khai push tự động báo động đỏ từ từ khóa.

BẢN SỬA GIỚI HẠN TỐC ĐỘ (04/11/2026): giãn mỗi truy vấn GDELT cách nhau 5,5 giây và thử lại tối đa 3 lần (cách nhau 6 giây) khi bị lỗi, để tránh lỗi Failed to fetch khi tải trang hoặc bấm Cập nhật tin.
