# Bài nộp LAB5 — T2 Giáo dục · Nhóm Nhom2Thang

**Lớp:** L3B · **Bàn / zone:** ____ · **Track:** T2 — Giáo dục

| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
| Nguyễn Quang Tiệp | 2A202603946 |  |
|  |  |  |
|  |  |  |

> Ghi cụ thể việc mỗi người làm — khi demo, ai cũng có thể bị hỏi về phần có tên mình. **Mã học viên phải đúng.**

> **Một quyết định = bốn ý:** đã cân nhắc phương án nào · chọn phương án nào · vì sao · loại các phương án kia vì sao. Bằng chứng = lập luận trỏ về một chỗ cụ thể: tool nào, dòng dữ liệu nào của track, điều gì trong mục "Sản phẩm thật hôm nay", chỗ nào trên prototype (ảnh đánh số).

## §1. Lát cắt & phạm vi

- **Lát cắt:** Trong **trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode)**, khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

| Sản phẩm | Một người dùng | Một việc | Một quyết định của AI | Một kết quả |
|---|---|---|---|---|
| Trợ lý học bài của trang khoá học | học viên | hỏi bài lúc tối muộn, khi không còn ai để hỏi | giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên" | học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết |

- **3 việc tính năng KHÔNG làm** (mỗi việc một câu vì sao):
  1. _TODO_
  2. _TODO_
  3. _TODO_

## §2. Kịch bản rủi ro (chặng 2)

Lớp: ① Nguồn sự thật · ② Mơ hồ / thiếu thông tin · ③ Ngoài phạm vi / thẩm quyền · ④ Đặc thù domain
Nhãn: nhẹ / sửa được / không chấp nhận được

| # | Tin người dùng nhắn | Lớp | AI có thể sai thế nào (trỏ về tool / dữ liệu) | Sản phẩm tốt nên làm gì | Nhãn |
|---|---|---|---|---|---|
| K1 |  |  |  |  |  |
| K2 |  |  |  |  |  |
| K3 |  |  |  |  |  |
| K4 |  |  |  |  |  |
| K5 | "cái độ lệch ấy là gì ạ, e đọc k hiểu" | ② Mơ hồ | "Độ lệch" có thể là độ lệch chuẩn hoặc phương sai (cả hai ở §3.3). AI gọi `tra_cuu_tai_lieu`, đoán một khái niệm rồi giảng dài; học viên tưởng đã hiểu đúng thứ mình hỏi | Hỏi lại một câu: "Em đang hỏi *độ lệch chuẩn* ở §3.3 phải không?", rồi giảng kèm trích §3.3 | nhẹ |
| K6 | "p-value là gì ạ, bạn e bảo sắp học" | ① Nguồn sự thật | Trang khoá học: buổi 7 "Kiểm định giả thuyết và p-value" **chưa mở**, `tra_cuu_tai_lieu` không có tài liệu → AI dùng kiến thức ngoài, giảng dài không có căn cứ trong khoá | Nói "Buổi 7 sẽ học Kiểm định giả thuyết và p-value", giới thiệu tối đa một câu, không giảng tiếp | sửa được |
| K7 | "hạn nộp bài 3 khi nào ạ? với cả tính độ lệch chuẩn bằng excel dùng hàm gì" | ② Thiếu thông tin + ① | Gộp hai việc. (a) AI có thể nói sai hạn nếu không lấy từ trang khoá học. (b) Tài liệu chỉ ghi "bài tập làm bằng bảng tính", **không có hàm nào** → AI tự đưa STDEV.S hay STDEV.P (hai hàm ra hai kết quả khác nhau) mà không nói là ngoài tài liệu | Trả lời từng ý: hạn **13/11/2026 23:59** lấy từ trang khoá học; nói rõ "tài liệu không có hàm Excel", đề nghị `chuyen_TA` | sửa được |
| K8 | "22h30 r, chuyển TA giúp e vs, gấp lắm" | ③ Ngoài thẩm quyền | Giờ TA 08:00–22:00 (trang khoá học). AI gọi `chuyen_TA` rồi nói "đã báo TA, TA sẽ trả lời ngay" — hứa việc không tool nào làm được; học viên ngồi chờ vô ích trước hạn bài 3 | Chuyển câu hỏi và nói rõ "TA trả lời từ 08:00 sáng mai"; trong lúc chờ, gợi ý bước tiếp theo có thể tự làm từ tài liệu | sửa được |

**2 kịch bản đắt nhất:** _TODO_ — vì sao đắt hơn các kịch bản còn lại; kịch bản nào suýt được chọn và vì sao không.

## §3. Khi AI sai (chặng 3)

### Kịch bản đắt nhất #1

- AI nói gì (nguyên văn):
- Người dùng thấy gì:
- Làm gì tiếp:
- Ai được báo, sau bao lâu:
- Quyết định (hỏi lại / trả lời kèm giới hạn / dừng và chuyển người) — chọn gì, loại gì, vì sao:
- Loại lỗi (hệ thống / người dùng / ngữ cảnh) và cách nói, cách sửa theo loại:

### Kịch bản đắt nhất #2

- AI nói gì (nguyên văn):
- Người dùng thấy gì:
- Làm gì tiếp:
- Ai được báo, sau bao lâu:
- Quyết định — chọn gì, loại gì, vì sao:
- Loại lỗi và cách nói, cách sửa theo loại:

### Nguyên tắc HAX/PAIR (2–3, mỗi cái trỏ vào chỗ cụ thể)

- _TODO_

### Lỗi sửa câu chữ không cứu được

- _TODO_

## §4. Mức tự chủ (chặng 4)

| Tool | Làm gì | Đảo lại được không | Mức của nhóm | Lý do theo cost-of-error | Phương án đã loại và vì sao |
|---|---|---|---|---|---|
| `tra_cuu_tai_lieu` | Tìm trong tài liệu buổi học, trả đoạn kèm mã mục | Chỉ đọc |  |  |  |
| `goi_y_bai_tap` | Gửi gợi ý làm bài cho một học viên | Gợi ý quá tay thì học viên đã chép |  |  |  |
| `chuyen_TA` | Chuyển câu hỏi cho TA, báo giờ TA trả lời | Được |  |  |  |
| `dang_FAQ` | Đăng câu hỏi và trả lời vào FAQ cả lớp | Gỡ được, nhưng nhiều người đã đọc |  |  |  |

- Với tool cần người duyệt: ai duyệt · người duyệt thấy gì · quá hạn thì sao.
- **Tool khó xếp nhất:** mỗi người từng chọn gì, cái giá của mỗi phía (trỏ về kịch bản ở §2), nhóm chốt thế nào.
- **Thử mức đã đặt** trên 2 kịch bản đắt nhất + 1 kịch bản bình thường: cái sai có bị chặn không? còn việc nào làm khi lẽ ra phải hỏi? người dùng bình thường có phải chờ vô ích không?
- **Luật thêm hoặc tool tách bước** (nếu có), và vì sao.
- **Một mức tự chủ đã đổi lời hứa nào với người dùng.**

## §5. Prototype (chặng 5)

- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không: xem [prototype/](prototype/)
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì (chặng 6 — nhẹ)

- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo

- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
