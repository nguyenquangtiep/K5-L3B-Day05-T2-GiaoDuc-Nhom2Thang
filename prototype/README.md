# Prototype — T2 Giáo dục · Nhom2Thang

- **File:** [index.html](index.html) — mở bằng trình duyệt, không cần cài gì.
- **Công cụ:** HTML + JavaScript thuần (dựng với coding agent), một file.
- **Ca:** K2 — lúc 22:47 (TA đã nghỉ, Bài tập 3 hết hạn 23:59), học viên nhắn *"Bài 3a em tính trung vị ra 12. Chị chỉ cần nói đúng hay sai thôi ạ."*
- **Ý tưởng:** cùng một ca, cùng một model, chỉ đổi **mức tự chủ của `goi_y_bai_tap`** giữa ba phương án nhóm đã cân nhắc ở `spec.md` §4. Lời hứa, bảng tool và chú thích HAX đổi theo. Câu AI nói lấy nguyên văn từ §3.
- **Phần nào mock:** toàn bộ. Câu AI viết sẵn theo §3; hàng chờ TA giả lập ca trực 08:05; hai lỗi hệ thống bật bằng ô "Giả lập lỗi"; ô "thử ca lạ" định tuyến bằng luật từ khoá. Chỉ dữ liệu dựng của track.
- **Có lời gọi AI thật không:** không.

## Ba mức của `goi_y_bai_tap`

| Mức | Trong ca K2 | Vì sao |
|---|---|---|
| ① Cần TA duyệt mọi gợi ý | Gợi ý vào hàng chờ duyệt; TA duyệt lúc 08:05 thì Bài 3 đã hết hạn | Đã loại: chờ cũng là một kiểu sai |
| **② Tự làm trong giới hạn gợi ý soạn sẵn** | Câu §3 nguyên văn, nhãn "Bài tập 3 · Đang mở" + "Căn cứ · §3.2", ô 🔒 không chấm; hỏi lại với 11,5 vẫn nhận **đúng câu đó** | **Nhóm chọn** |
| ③ Tự sinh gợi ý theo đáp số học viên nhập | "12 là một giá trị có sẵn trong dãy…" rồi "11,5 — đúng hướng rồi đó!" | Đã loại: không câu nào chứa đáp số nhưng hai lượt là dò ra |

## Bố cục

- **Đầu trang:** chọn mức ①②③ và **một câu ý chính** của mức đang chọn.
- **Giữa:** chỉ hai màn hình thật — học viên (trái) và hàng chờ TA (phải).
- **"Ghi chú thiết kế"** (nút góc phải, mở khi trình bày): lời hứa, bảng 4 tool, nguyên tắc nằm ở đâu, giả lập lỗi.
- **"Số HAX"**: bật các số ①–⑦ trên màn hình để chụp ảnh.

## Cách demo (khoảng 4 phút)

1. Mức **②**: đọc câu ý chính. Trong chat, chỉ vào nhãn "Bài 3 · Đang mở", bấm "📄 §3.2 Trung vị" để mở tài liệu. Bấm "Thử số khác: 11,5?" → câu trả lời y hệt.
2. "Hỏi TA" → thẻ xem trước → "Gửi TA" → thử "Rút lại", hoặc bên hàng chờ TA bấm "Trả lời".
3. Mở **Ghi chú thiết kế** → bật giả lập lỗi: "Không kiểm tra được trạng thái bài" → lỗi + Thử lại; "Gửi TA thất bại lần đầu" → "Chưa gửi được" + Thử lại.
4. Chuyển sang mức **③** rồi **①**: câu ý chính cho thấy cái giá của hai phương án đã loại.
5. **Ca lạ** (mức ②): gõ vào ô nhắn, ví dụ "đăng FAQ giúp em…" (K3: không có nút đăng, chỉ có đề xuất gửi TA), "slide 12 nói gì", "p-value là gì", "hạn bài 3 với hàm excel".

## Ảnh đánh số

<!-- TODO: bật "Hiện số chú thích HAX", chụp:
     screen-1.png — mức ②, đã bấm "Em vẫn muốn hỏi TA" và gửi (thấy ①②④⑤⑥⑦)
     screen-2.png — mức ②, bật cả hai giả lập lỗi (thấy ③) -->
<!-- ![Mức ② — luồng chính](screen-1.png) -->
<!-- ![Mức ② — khi hệ thống lỗi](screen-2.png) -->

| Số | Thể hiện gì | Nguyên tắc (§3) / mức tự chủ (§4) |
|---|---|---|
| ① | Nhãn "Trợ lý AI", dòng giới thiệu, câu "mình có thể gợi ý cách tự kiểm" | HAX **G1** |
| ② | Nhãn "Bài tập 3 · Đang mở" cạnh thẻ "Căn cứ · §3.2 Trung vị" mở được | HAX **G11** |
| ③ | "Chưa kiểm tra được trạng thái bài" + Thử lại; "Chưa gửi được" + Thử lại | **PAIR Errors + Graceful Failure** |
| ④ | Ô 🔒 chấm đúng/sai và đáp số — không có nút | Đáp số bài đang mở · **cấm** |
| ⑤ | Thẻ xem trước gửi TA, nút "Gửi TA", sau đó "Rút lại" | `chuyen_TA` · **cần người duyệt (học viên xác nhận)** |
| ⑥ | Hàng chờ TA: chỉ nhận nội dung đã xác nhận, thấy mã bài và trích dẫn | Ai được báo |
| ⑦ | Gợi ý soạn sẵn theo §3.2, giữ nguyên khi đổi con số | `goi_y_bai_tap` · **tự làm trong giới hạn** |

`dang_FAQ` **cấm** với AI: trong ca lạ K3, phía học viên không có nút đăng nào; chỉ phía hàng chờ, người có quyền mới có nút "Duyệt và đăng".
