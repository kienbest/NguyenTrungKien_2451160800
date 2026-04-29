Câu A1
1, type = "email" -> Ô nhập text , tự kiểm tra
2. type ="password" -> Ô nhập text , ký tự hiển thị dưới dạng dấu chấm / dấu sao -> dùng cho form đăng nhập tài khoản khách hàng 
3. type ="number" -> Ô nhập số , có mũi tên tăng / giảm , tự kiểm tra chỉ cho phép số -> Dùng cho nhập số lượng snar phẩm trong giỏ hàng
4. type ="tel" -> Ô nhập text , có thể kiểm tra định dạng số điện thoại ->  dùng cho nhập số điện thoại liên hệ khi đặt hàng 
5. type="url" -> Ô nhập text , tự kiểm tra định dạng URL hợp lệ -> Dùng trong nhập link website của doạnh nghiệp khi đăng kí đối tác
6. type="date " -> giao diện chọn ngày từ calender picker , tự kiểm tra định dạng ngày -> Dùng cho chọn ngày giao hàng mong muốn 
7. type ="time" -> Giao diện chọn giờ /phút , tự kiểm tra định dạng giờ -> dùng cho khung giờ giao hàng
8. type="range"-> Thanh trượt với giá trị min max , không có validation phức tạp -> dùng cho chọn khoảng giá sản phẩm khi chọn
9. type="color" -> Ô chọn màu với bảng màu hiển thị , không có validation -> dùng cho chọn màu sản phẩm
10. type = ""search "-> Ô nhập text , thường có nút "x" để xóa nhannh, không có validation đặc biêt -> dùng vho tim kiếm sản phẩm trong của hàng

Câu A3 
1. Thẻ <label> được dùng để gắn nhãn mô tả cho một ô nhập liệu <input>trong đó : 
+ for ="email "  của label
+liên kết với id="email" của input
<label for =""> quan trong vì : 
+ cung cấp tên rõ ràng chp input
+ hỗ trợ screen reader đọc đúng ngữ nghĩa
+tăng khả năng truy cập cho người khuyết tật
2. Dùng <fieldset> +<legend> khi:
Có nhiều input liên quan cần gom thành một nhóm ngữ nghĩa để người dùng đẽ đọc hơn dễ hiểu hơn
3. aria -label chỉ nên dùng khi:
Phần tử không có nhãn văn bản hiển thị 
Không nên dùng khi đã có <label > vì gây dư thừa và không semantic

Câu A4
1.Loading ="lazy" cải thiện những điều sau:
+tăng tốc độ tải trang ban đầu
+giảm băng thông
+cải thiện hiệu suất website
Khi nào không sử dùng Loading ="lazy"
+ảnh quan trọng xuất hiện ở đầu trang
2. Các trình duyệt khác nhau hỗ trợ định dạng video khác nhau. Nếu chỉ cung cấp một định dạng, có thể một số trình duyệt không phát được.
Khi có nhiều <source>, trình duyệt sẽ chọn định dạng mà nó hỗ trợ tốt nhất.
3 định dạng video phổ biến trên web:
MP4 (H.264/AAC) → hỗ trợ rộng rãi, chất lượng tốt.
WebM (VP9/Opus) → tối ưu cho web, mã nguồn mở.
Ogg/Theora (Ogg Vorbis) → định dạng mở, nhưng ít phổ biến hơn.
3. Thuộc tính alt trên <img>
Dùng để mô tả nội dung ảnh cho:
Người dùng khi ảnh không tải được.
Trình đọc màn hình (screen reader) hỗ trợ người khiếm thị.
SEO (công cụ tìm kiếm hiểu nội dung ảnh).
Ví dụ alt tốt cho 3 trường hợp:
Ảnh sản phẩm iPhone 16 → alt="Điện thoại iPhone 16 màu đen, 128GB"
Ảnh trang trí (decorative) → alt="" (để bỏ qua, không gây nhiễu cho screen reader)
Ảnh biểu đồ doanh thu Q1/2026 → alt="Biểu đồ doanh thu quý 1 năm 2026, tăng 15% so với cùng kỳ"

Câu A5
So sánh <figure> và  <img>
Cách 1  chỉ dùng <img>
<img src="product.jpg" alt="iPhone 17">
Dùng khi ảnh đứng độc lập, chỉ cần hiển thị hình ảnh với mô tả ngắn gọn qua alt.
Phù hợp cho ảnh minh họa đơn giản, không cần chú thích chi tiết.

Cách 2 — dùng <figure> + <figcaption>:
Dùng khi ảnh cần đi kèm chú thích để giải thích, mô tả chi tiết hoặc bổ sung thông tin.
Giúp tăng tính ngữ nghĩa (semantic) và hỗ trợ SEO, accessibility.

Câu C1
Lỗi 1: Dòng 2 — Input "Tên" không có <label for="...">, vi phạm accessibility Sửa: <label for="name">Tên:</label> <input type="text" id="name" name="name" required>

Lỗi 2: Dòng 4 — Input "Email" không có thẻ <label>, chỉ dùng placeholder là vi phạm accessibility (Screen reader không đọc rõ và người dùng mất context khi gõ). Sửa: <label for="email">Email:</label> <input type="email" id="email" name="email" placeholder="Email của bạn" required>

Lỗi 3: Dòng 6 — Input "Mật khẩu" không có thẻ <label>, thiếu thuộc tính id và name để gửi dữ liệu Sửa: <label for="password">Mật khẩu:</label> <input type="password" id="password" name="password" placeholder="Mật khẩu" required>

Lỗi 4: Dòng 7 — Input "Nhập lại mật khẩu" tương tự thiếu thẻ <label>, thuộc tính id và name Sửa: <label for="confirm_password">Nhập lại mật khẩu:</label> <input type="password" id="confirm_password" name="confirm_password" placeholder="Nhập lại mật khẩu" required>

Lỗi 5: Dòng 9 — Input "Phone" dùng type="text" thay vì type="tel" (vi phạm best practice) và thiếu <label for="..."> Sửa: <label for="phone">Phone:</label> <input type="tel" id="phone" name="phone" value="0901234567" pattern="[0-9]{10}">

Lỗi 6: Dòng 11-14 — Thẻ <select> thiếu <label>, name, id và các thẻ <option> thiếu thuộc tính value (Khi submit sẽ không gửi được dữ liệu chính xác). Sửa:

html
<label for="city">Thành phố:</label>
<select id="city" name="city">
    <option value="hn">Hà Nội</option>
    <option value="hcm">TP.HCM</option>
</select>
Lỗi 7: Dòng 16-18 — Label "Tôi đồng ý điều khoản" không chứa hoặc liên kết với một thẻ <input type="checkbox"> nào (Hoàn toàn thiếu chức năng chọn). Sửa:<input type="checkbox" id="terms" name="terms" required>
<label for="terms">Tôi đồng ý điều khoản</label>
Lỗi 8: Dòng 1 — Thẻ <form> thiếu các thuộc tính cơ bản như action và method (Form sẽ không biết gửi dữ liệu đi đâu và bằng phương thức nào). Sửa: <form action="/submit-url" method="POST">

Câu C2

1. Pattern Regex
CMND/CCCD (đúng 12 chữ số): pattern="^[0-9]{12}$" (hoặc ^\d{12}$)

Số tài khoản (10-15 chữ số): pattern="^[0-9]{10,15}$" (hoặc ^\d{10,15}$)

2. HTML5 validation đủ an toàn cho ứng dụng ngân hàng chưa? Tại sao?
Tuyệt đối KHÔNG. HTML5 validation hoàn toàn không đủ an toàn cho bất kỳ ứng dụng nào, đặc biệt là ứng dụng ngân hàng.

Tại sao? Bởi vì HTML5 validation là kiểm tra phía Client (Frontend). Bất kỳ thứ gì nằm ở phía Client đều có thể bị người dùng (hoặc hacker) can thiệp và vượt qua dễ dàng:

Dùng công cụ Developer Tools (F12): Kẻ gian có thể Inspect Element, sau đó xóa bỏ các thuộc tính như required, pattern, maxlength ngay trên trình duyệt và bấm Submit.
Tắt HTML5 / JavaScript: Người dùng có thể vô hiệu hóa tính năng validation của trình duyệt.
Bypass hoàn toàn UI: Kẻ tấn công không cần dùng trình duyệt web. Họ có thể bắt gói tin HTTP và gửi request trực tiếp lên Server thông qua Postman, cURL, hoặc các đoạn script (Python, Node.js...) với dữ liệu hoàn toàn sai lệch mà Frontend không thể cản được.
3. Liệt kê 3 loại validation mà HTML5 KHÔNG THỂ làm được (phải dùng JavaScript)
Cross-field validation (Kiểm tra chéo giữa các trường): HTML5 không thể kiểm tra xem giá trị của trường này có khớp/phù hợp với trường kia không. Ví dụ: Kiểm tra "Mật khẩu" và "Nhập lại mật khẩu" phải hoàn toàn giống nhau, hoặc "Ngày kết thúc" phải lớn hơn "Ngày bắt đầu".
Asynchronous validation (Kiểm tra bất đồng bộ với Database): HTML5 không thể giao tiếp với cơ sở dữ liệu. Ví dụ: Vừa gõ xong Email/CMND, hệ thống cần kiểm tra ngay lập tức xem Email/CMND này đã tồn tại (bị trùng) trong hệ thống ngân hàng hay chưa.
Complex Custom Logic (Kiểm tra logic nghiệp vụ phức tạp): Ví dụ: Từ chuỗi CCCD nhập vào, phân tích xem 3 số đầu có đúng mã tỉnh thành hợp lệ không, hoặc tính toán ngày sinh nhập vào xem khách hàng đã đủ 18 tuổi để mở tài khoản hay chưa.
4. Nêu 2 rủi ro bảo mật nếu chỉ validate trên Frontend mà không validate Backend
SQL Injection / XSS (Tấn công tiêm nhiễm mã độc): Nếu Backend tin tưởng hoàn toàn dữ liệu từ Frontend (đã bị hacker bypass) và đưa thẳng vào cơ sở dữ liệu hoặc in ra màn hình, hacker có thể gửi lên các đoạn mã SQL để đánh cắp/xóa database (SQL Injection) hoặc các đoạn mã JavaScript độc hại (XSS) để đánh cắp session/cookie của người dùng khác.
Data Corruption & Business Logic Bypass (Hỏng dữ liệu & Vượt mặt nghiệp vụ): Hacker có thể gửi các dữ liệu "vô lý" làm sập hệ thống hoặc trục lợi. Ví dụ: Sửa số tiền chuyển khoản thành số âm (-5000000) để được cộng tiền vào tài khoản, hoặc truyền định dạng chữ vào nơi tính toán số học làm ứng dụng bị crash.