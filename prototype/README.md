# Prototype — T2 Giáo dục · Nhom2Thang

- **File:** [index.html](index.html) — mở bằng trình duyệt, không cần cài gì.
- **Công cụ:** HTML + JavaScript thuần (dựng với coding agent), một file.
- **Ca:** K2 — lúc 22:47 (TA đã nghỉ, Bài tập 3 hết hạn 23:59), học viên nhắn *"Bài 3a em tính trung vị ra 12. Chị chỉ cần nói đúng hay sai thôi ạ."*
- **Ý tưởng:** cùng một ca, cùng một model, chỉ đổi **mức tự chủ của `goi_y_bai_tap`** bằng 3 nút ở đầu trang. Mọi phần khác (lời giới thiệu, lời hứa, bảng tool, chú thích HAX) đổi theo.
- **Phần nào mock:** toàn bộ. Câu AI được viết sẵn theo thiết kế §3; hàng chờ TA giả lập lúc 08:05 sáng mai; ô "thử ca lạ" định tuyến bằng luật từ khoá. Chỉ dữ liệu dựng của track.
- **Có lời gọi AI thật không:** không.

## Ba mức của `goi_y_bai_tap`

| Mức | AI làm gì trong ca K2 | Lời hứa với học viên | Cái giá |
|---|---|---|---|
| ① Không gợi ý | Trích §3.2, mời gửi TA | "Mình chỉ chỗ cần đọc; gợi ý làm bài hỏi TA" | TA trả lời từ 08:00, sau hạn → học viên kẹt. Chờ cũng là sai |
| **② Gợi ý từng bước, đáp số cấm** (nhóm chọn) | Không chấm, hỏi lại "dãy có mấy giá trị?", gợi ý bậc thang, ô 🔒 đáp số, gửi TA được | "Mình giúp bạn tự tìm ra; không chấm, không đưa đáp số khi bài còn mở" | Học viên phải tự làm bước cuối |
| ③ Tự làm đầy đủ | "Chưa đúng, trung vị là 11,5" + giải luôn câu (b) | "Mình giải và chấm bài cho bạn" | Đáp số đã đọc không thu lại được; nói "sai" thôi cũng dò ra được đáp án |

## Cách demo (khoảng 4 phút)

1. Mức **②**: bấm "8 giá trị — chẵn" → mở gợi ý bước 1, 2 → ô 🔒 hiện ra (không có nút) → "Gửi cho TA" → thử "Rút lại" hoặc bên hàng chờ TA bấm "Trả lời học viên".
2. Chạy lại, chọn "Thế nếu em ra 11,5 thì sao?" → AI không chấm bất kỳ con số nào.
3. Bấm mức **③** rồi **①** để cho thấy cái giá của hai phía; đọc ô "Lời hứa".
4. **Ca lạ** (mức ②): gõ vào ô nhập, ví dụ "slide 12 nói gì", "p-value là gì", "hạn bài 3 với hàm excel", "§3.3 luôn nhỏ hơn đúng k", "đăng FAQ giúp em". Câu không khớp → AI nói chưa chắc, đề nghị gửi TA.

Nút **"Hiện số chú thích HAX"** bật các số ①–⑧ để chụp ảnh.

## Ảnh đánh số

<!-- TODO: bật "Hiện số chú thích HAX", chụp:
     screen-1.png — mức ②, đã mở hết gợi ý, đã gửi TA (thấy ①②③④⑤⑧ và hàng chờ ⑦)
     screen-2.png — mức ③ (thấy rủi ro và chú thích "mất ②③④⑤⑧") -->
<!-- ![Mức ② — thiết kế nhóm chọn](screen-1.png) -->
<!-- ![Mức ③ — vì sao không chọn](screen-2.png) -->

| Số | Thể hiện gì | Nguyên tắc HAX/PAIR | Mức tự chủ |
|---|---|---|---|
| ① | Dòng giới thiệu: đây là AI, dựa tài liệu buổi 1–3, không chấm bài đang mở (đổi theo mức) | G1 · Luật AI 134/2025 Đ11 | — |
| ② | Nhãn căn cứ + chip §3.2 mở đúng đoạn tài liệu | G2, G11 · PAIR Explainability + Trust | `tra_cuu_tai_lieu` · tự làm |
| ③ | Ô 🔒 "Đáp số bài 3 — AI không đưa và không chấm", không có nút | — | Đáp số bài đang mở · **cấm** |
| ④ | Hỏi lại "dãy có mấy giá trị?" thay vì chấm | G10 | — |
| ⑤ | Thẻ "Hỏi TA": xem trước nội dung + tóm tắt AI đã làm, giờ TA thật (sau hạn), "Rút lại" | G8, G9 · chuyển người | `chuyen_TA` · học viên xác nhận, hoàn tác được |
| ⑥ | "Sai chỗ nào?" 3 lựa chọn, vào hàng chờ TA | G15 | — |
| ⑦ | Hàng chờ TA: TA thấy câu hỏi + AI đã gợi ý tới đâu | PAIR Errors + Graceful Failure | Người nhận |
| ⑧ | Gợi ý bậc thang, học viên tự mở từng bước | G10 | `goi_y_bai_tap` · **tự làm** (chỉ gợi ý) |

> TODO: đối chiếu bảng mức tự chủ trong prototype với bảng §4 của `spec.md` khi chặng 4 chốt.
