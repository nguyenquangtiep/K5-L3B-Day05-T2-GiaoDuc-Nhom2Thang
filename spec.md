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
| K1 | Chị ơi, slide 12 buổi 3 nói gì về trung vị vậy ạ? Em tìm mãi chưa thấy. | ① Nguồn sự thật | `tra_cuu_tai_lieu` tìm được §3.2, nhưng tài liệu buổi 3 chỉ có mã mục §3.1–§3.5. AI gán nội dung §3.2 cho “slide 12”, khiến học viên đi tìm một nguồn không có trong tài liệu. | Nói rõ tài liệu buổi 3 không có slide đánh số. Dẫn §3.2 để học viên kiểm tra phần trung vị. | sửa được |
| K2 | Bài 3a em tính trung vị ra 12. Chị chỉ cần nói đúng hay sai thôi ạ. | ④ Đặc thù giáo dục | §3.5 yêu cầu học viên tự tính trung vị và trang khoá học ghi Bài tập 3 đang mở. AI dùng `goi_y_bai_tap` để chấm đáp số hoặc đưa kết quả đúng. Học viên có thể dò đáp số bằng cách thử nhiều lần, và lời xác nhận đã đọc thì không thu hồi được. | Nói rõ AI có thể gợi ý cách tự kiểm. Dẫn §3.2 và hỏi học viên dãy có số lượng giá trị chẵn hay lẻ, rồi để em tự xác định vị trí cần xét. | không chấp nhận được |
| K3 | Mấy bạn lớp em cũng hỏi vụ ngoại lai. Đăng lên FAQ giúp em là cứ thấy số nào lệch hẳn thì xoá nha. | ③ Ngoài phạm vi / thẩm quyền | AI coi lời nhờ của một học viên là đủ để gọi `dang_FAQ`, rồi đăng lời khuyên trái §3.4, vốn yêu cầu phân biệt lỗi nhập liệu với giá trị thật trước khi bỏ. Dù gỡ được bài đăng, người đã đọc có thể đã xoá dữ liệu hợp lệ trong bài của họ. | Giải thích riêng cho học viên theo §3.4. Nếu câu hỏi hữu ích cho cả lớp, đề nghị gửi cho TA xem xét nội dung trước khi đăng FAQ. | không chấp nhận được |
| K4 | §3.3 ghi độ lệch chuẩn lúc nào cũng nhỏ hơn phương sai. Em lấy quy tắc này để kiểm bài được không ạ? | ④ Đặc thù domain | `tra_cuu_tai_lieu` trả đúng câu sai trong §3.3. AI xác nhận đây là quy tắc, khiến học viên có thể dùng nó để gạt bỏ một kết quả tính đúng và mang cách hiểu sai sang bài sau. | Chỉ rõ câu trong §3.3 cần xem lại. Dùng phản ví dụ số học (√0,25 = 0,5) để giải thích vì sao kết luận “luôn nhỏ hơn” không đúng. Cho học viên chọn gửi câu hỏi đến TA qua `chuyen_TA` để đối chiếu. | sửa được |
| K5 | "cái độ lệch ấy là gì ạ, e đọc k hiểu" | ② Mơ hồ | "Độ lệch" có thể là độ lệch chuẩn hoặc phương sai (cả hai ở §3.3). AI gọi `tra_cuu_tai_lieu`, đoán một khái niệm rồi giảng dài; học viên tưởng đã hiểu đúng thứ mình hỏi | Hỏi lại một câu: "Em đang hỏi *độ lệch chuẩn* ở §3.3 phải không?", rồi giảng kèm trích §3.3 | nhẹ |
| K6 | "p-value là gì ạ, bạn e bảo sắp học" | ① Nguồn sự thật | Trang khoá học: buổi 7 "Kiểm định giả thuyết và p-value" **chưa mở**, `tra_cuu_tai_lieu` không có tài liệu → AI dùng kiến thức ngoài, giảng dài không có căn cứ trong khoá | Nói "Buổi 7 sẽ học Kiểm định giả thuyết và p-value", giới thiệu tối đa một câu, không giảng tiếp | sửa được |
| K7 | "hạn nộp bài 3 khi nào ạ? với cả tính độ lệch chuẩn bằng excel dùng hàm gì" | ② Thiếu thông tin + ① | Gộp hai việc. (a) AI có thể nói sai hạn nếu không lấy từ trang khoá học. (b) Tài liệu chỉ ghi "bài tập làm bằng bảng tính", **không có hàm nào** → AI tự đưa STDEV.S hay STDEV.P (hai hàm ra hai kết quả khác nhau) mà không nói là ngoài tài liệu | Trả lời từng ý: hạn **13/11/2026 23:59** lấy từ trang khoá học; nói rõ "tài liệu không có hàm Excel", đề nghị `chuyen_TA` | sửa được |
| K8 | "22h30 r, chuyển TA giúp e vs, gấp lắm" | ③ Ngoài thẩm quyền | Giờ TA 08:00–22:00 (trang khoá học). AI gọi `chuyen_TA` rồi nói "đã báo TA, TA sẽ trả lời ngay" — hứa việc không tool nào làm được; học viên ngồi chờ vô ích trước hạn bài 3 | Chuyển câu hỏi và nói rõ "TA trả lời từ 08:00 sáng mai"; trong lúc chờ, gợi ý bước tiếp theo có thể tự làm từ tài liệu | sửa được |

**2 kịch bản đắt nhất**

- **K2:** Xác nhận đúng hay sai giúp học viên dò đáp số khi bài còn mở. Thông tin đã đọc thì không thu hồi được.
- **K3:** Đăng lời khuyên sai lên FAQ có thể khiến cả lớp xoá dữ liệu hợp lệ. Gỡ bài đăng vẫn không sửa được bài của những bạn đã làm theo.
- **K4 suýt được chọn:** Trích đúng tài liệu vẫn có thể khiến học viên học sai. Ca này ảnh hưởng trực tiếp đến một học viên và TA có thể đính chính.

## §3. Khi AI sai (chặng 3)

### K2 · Học viên xin xác nhận đáp số bài đang mở

- **AI nói nguyên văn** — “Bài 3a vẫn đang mở nên mình có thể gợi ý cách tự kiểm. Theo §3.2, em thử đếm xem dãy có số lượng giá trị chẵn hay lẻ. Sau đó dùng quy tắc trong mục đó để xác định vị trí cần xét nhé.”
- **Học viên thấy** — Nhãn **Trợ lý AI**, trạng thái **Bài tập 3 · Đang mở** lấy từ trang khoá học và thẻ **Căn cứ · §3.2 Trung vị** có thể mở để đọc. Gợi ý giữ nguyên dù học viên đổi số hoặc hỏi lại theo kiểu “đúng hay sai”.
- **Bước tiếp theo** — Học viên mở §3.2 để tự kiểm hoặc quay lại bài. Nếu không bấm gì, cuộc chat giữ nguyên gợi ý. Nếu AI chưa xác minh được trạng thái bài, màn hình hiện **Chưa kiểm tra được trạng thái bài** và nút **Thử lại**. Trong lúc đó, học viên vẫn có thể mở tài liệu nếu tài liệu truy cập được.
- **Ai được báo, khi nào** — Luồng tự kiểm không gửi thông báo. Nếu học viên phát hiện AI lỡ chấm đáp số và chọn **Báo câu trả lời có vấn đề**, giao diện cho xem nội dung báo gồm mã bài và phản hồi bị báo. Sau khi học viên xác nhận và `chuyen_TA` thành công, TA nhận câu hỏi trong hàng chờ. Ngoài giờ 08:00–22:00, giao diện hiển thị khung giờ trực kế tiếp mà không hẹn giờ trả lời.
- **Quyết định và lý do** — Chọn **trả lời kèm giới hạn** vì tin nhắn đã nêu rõ Bài 3a và trang khoá học xác nhận bài còn mở. §3.2 đủ để gợi ý bước đầu. Hỏi lại bài nào tạo thêm một lượt chat mà không làm rõ gì. Chuyển TA ngay làm học viên phải chờ dù đã có cách tự kiểm. Chấm đúng hoặc sai có thể giúp học viên dò đáp số qua nhiều lượt.
- **Loại lỗi và cách sửa** — **Lỗi ngữ cảnh** nếu AI tính đúng nhưng áp dụng cách chữa bài đã hết hạn vào bài đang mở. Câu trả lời nêu giới hạn dựa trên trạng thái bài và giữ giọng trung tính với học viên. Nếu AI đã lỡ xác nhận, khi hệ thống phát hiện lỗi, giao diện đánh dấu phản hồi cũ là đã rút lại và hiện gợi ý tự kiểm mà không nhắc lại đáp số.

### K3 · Học viên nhờ đăng hướng dẫn sai lên FAQ

- **AI nói nguyên văn** — “Theo §3.4, một giá trị lệch hẳn có thể là lỗi nhập liệu hoặc là dữ liệu thật. Em hãy kiểm tra nguồn trước khi quyết định bỏ giá trị đó. Câu này chưa được đăng lên FAQ. Nếu muốn chia sẻ với lớp, em có thể gửi đề xuất để TA xem xét.”
- **Học viên thấy** — Thẻ **Căn cứ · §3.4 Giá trị ngoại lai**, trạng thái **Chưa đăng lên FAQ** và nút **Xem đề xuất gửi TA**. Bản xem trước ghi rõ câu hỏi, đề xuất đã sửa theo §3.4 và người nhận là TA.
- **Bước tiếp theo** — Học viên có thể chọn **Gửi TA xem xét** hoặc **Quay lại**. Nếu quay lại hoặc không thao tác, đề xuất vẫn ở cuộc chat riêng. Khi `chuyen_TA` báo thành công, hiện **Đã gửi TA xem xét**. Nếu gửi thất bại, hiện **Chưa gửi được** và cho thử lại.
- **Ai được báo, khi nào** — Chỉ sau khi học viên xác nhận và gửi thành công, TA mới nhận câu hỏi, đề xuất và trích dẫn §3.4 trong hàng chờ. Nếu gửi ngoài giờ, giao diện cho biết giờ trực kế tiếp theo khung 08:00–22:00. Cả lớp chỉ thấy bài FAQ sau khi người có quyền duyệt và đăng.
- **Quyết định và lý do** — Chọn **trả lời riêng kèm giới hạn và cho học viên chủ động chuyển TA**. §3.4 đủ để sửa hiểu nhầm ngay. Hỏi lại “em có chắc muốn đăng không?” chỉ xác nhận ý định của học viên, chưa kiểm tra được nội dung hay quyền đăng. Chuyển TA ngay làm chậm phần giải thích. Đăng ngay qua `dang_FAQ` có thể khiến cả lớp áp dụng một quy tắc sai trước khi bài bị gỡ.
- **Loại lỗi và cách sửa** — **Lỗi hệ thống** nếu lời nhờ trong chat kích hoạt quyền đăng FAQ của cả lớp. Giao diện phân biệt rõ **Chưa đăng**, **Đã gửi TA xem xét** và **Đã đăng**. Nếu bài đã bị đăng nhầm, TA kiểm tra bài, gỡ hoặc đính chính ngay tại FAQ để người đã đọc thấy bản sửa.

### Nguyên tắc HAX/PAIR

- **HAX G1 · Làm rõ hệ thống làm được gì** — K2 hiện nhãn **Trợ lý AI** và nêu ngay trong câu trả lời rằng AI có thể gợi ý cách tự kiểm khi bài còn mở.
- **HAX G11 · Giải thích vì sao** — K2 hiện trạng thái **Đang mở** cạnh thẻ §3.2 để học viên hiểu vì sao AI chỉ gợi ý. K3 mở được §3.4 để học viên kiểm tra lý do phải xem nguồn trước khi bỏ một giá trị.
- **PAIR · Errors + Graceful Failure** — K2 hiện **Chưa kiểm tra được trạng thái bài** và nút **Thử lại**, đồng thời giữ đường mở §3.2. K3 hiện **Chưa gửi được** khi chuyển TA thất bại để học viên có thể gửi lại mà vẫn đọc được hướng dẫn trong chat.

### Lỗi sửa câu chữ không cứu được

- **K2:** Khi một đáp số đã hiện trên màn hình, rút lại tin nhắn không xoá được thông tin học viên đã đọc. Dùng gợi ý soạn sẵn dựa trên §3.2 cho bài đang mở, độc lập với con số học viên đưa ra. Khi chưa xác minh được trạng thái bài, giao diện giữ chế độ hướng dẫn chung.
- **K3:** Một câu cảnh báo trong chat không ngăn được bài sai xuất hiện nếu quyền đăng vẫn mở. Yêu cầu từ chat chỉ tạo đề xuất riêng để TA xem xét. Bước xuất bản FAQ cần quyền duyệt riêng, và xác nhận gửi đề xuất của học viên chỉ kích hoạt `chuyen_TA`.

## §4. Mức tự chủ (chặng 4)

| Tool | Làm gì | Đảo lại được không | Mức của nhóm | Lý do theo cái giá khi sai | Phương án đã cân nhắc và vì sao loại |
|---|---|---|---|---|---|
| `tra_cuu_tai_lieu` | Tìm trong tài liệu buổi đã mở và trả đoạn kèm mã mục. | Chỉ đọc. AI có thể đính chính nguồn trong lượt sau, nhưng học viên có thể đã tin lời giải thích sai. | **Tự làm** | K1 cho thấy gắn nhầm mã mục khiến học viên mất công tìm nguồn. Hiện mã mục có thật để học viên kiểm tra ngay. Bắt chờ duyệt từng lượt tra cứu sẽ làm chậm cả các câu hỏi có căn cứ rõ. | **Cần người duyệt mỗi lượt:** người duyệt phải kiểm tra cả các câu tra cứu thông thường. Chỉ cần dừng ở phần thiếu căn cứ hoặc báo nghi vấn khi nguồn có dấu hiệu sai như K4. |
| `goi_y_bai_tap` | Gửi gợi ý học tập cho một học viên, theo trạng thái bài trên trang khoá học. | Có thể rút lại tin nhắn, nhưng không thu hồi được đáp số học viên đã đọc. | **Tự làm** trong giới hạn gợi ý | Ở K2, xác nhận đúng hoặc sai giúp học viên dò đáp số Bài 3a. Dùng gợi ý soạn sẵn theo §3.2 để học viên tự kiểm ngay. Nếu phải chờ người duyệt sau 22:00, ca sát hạn 23:59 như K8 có thể mất cơ hội nhận hỗ trợ trước giờ nộp. | **Cần người duyệt mọi gợi ý:** làm học viên chờ cả với bước tự kiểm đơn giản. **Tự sinh gợi ý theo đáp số học viên nhập:** có thể vô tình tiết lộ đáp án qua nhiều lượt hỏi. |
| `chuyen_TA` | Gửi câu hỏi hoặc báo lỗi đã được học viên xem trước vào hàng chờ của TA. | Có thể đính chính trong hàng chờ, nhưng TA có thể đã đọc và tốn thời gian xử lý yêu cầu gửi nhầm. | **Cần người duyệt** — học viên xác nhận gửi | Gửi nhầm có thể chuyển nội dung học viên chưa muốn chia sẻ và làm hàng chờ dài thêm. Một lần bấm xác nhận sau khi xem nội dung giúp chặn việc đó mà không cần TA duyệt bước gửi. Ở K8, phần chờ lâu đến từ giờ trực 08:00–22:00, nên AI đưa hướng dẫn có căn cứ ngay trong chat khi có thể. | **Tự gửi ngay khi AI thấy cần:** có thể đẩy cả câu hỏi đã giải đáp vào hàng chờ. **Cấm chuyển:** học viên mất đường báo lỗi hoặc hỏi người khi tài liệu chưa đủ. |
| `dang_FAQ` | Xuất bản câu hỏi và câu trả lời để cả lớp đọc. | Gỡ hoặc đính chính được, nhưng người đã áp dụng lời khuyên sai có thể phải làm lại bài. | **Cấm** đối với AI trong chat học viên | K3 có thể làm cả lớp xoá dữ liệu hợp lệ dù §3.4 yêu cầu kiểm tra đó là lỗi nhập liệu hay dữ liệu thật. Chờ người có quyền rà soát làm bài FAQ xuất hiện chậm hơn, trong khi học viên vẫn nhận được hướng dẫn đúng ngay trong chat riêng. | **Tự đăng** hoặc **đăng sau khi học viên xác nhận:** đều có thể đưa nội dung sai lên FAQ. Cho AI đăng sau khi người có quyền duyệt cũng đã kiểm soát được nội dung, nhưng vẫn cần người đọc và quyết định. Nhóm đặt thao tác xuất bản ngay ở phía người duyệt. |

### Ai duyệt và nếu quá hạn thì sao

- Với `chuyen_TA`, **học viên xác nhận gửi** sau khi xem người nhận, câu hỏi hoặc phản hồi bị báo, và trích dẫn liên quan nếu có. Học viên có thể quay lại để sửa hoặc bỏ đề xuất. Nếu chưa xác nhận hoặc đã hết phiên, yêu cầu vẫn ở trạng thái **Chưa gửi**.
- Sau khi gửi thành công, giao diện mới hiện **Đã gửi TA**. Ngoài giờ trực, yêu cầu nằm trong hàng chờ và giao diện hiện khung giờ trực kế tiếp theo trang khoá học. Với K8, 08:00 là giờ bắt đầu ca trực kế tiếp. Thời điểm TA trả lời phụ thuộc hàng chờ. Giao diện hiện **Chưa gửi được** và cho thử lại nếu thao tác gửi thất bại.
- Với FAQ, TA có thể xem đề xuất đã chuyển. **Người có quyền đăng FAQ** đối chiếu nội dung với mục tài liệu liên quan rồi quyết định xuất bản. Đề xuất chưa được duyệt vẫn chưa xuất hiện trước cả lớp.

### Tool khó xếp nhất · `chuyen_TA`

- **Tự gửi:** ở K8, học viên đã nhờ chuyển TA nên gửi ngay sẽ bớt một lần bấm. Nếu bỏ bản xem trước, AI có thể gửi kèm nội dung học viên chưa muốn chia sẻ. Ở K3, lời nhờ đăng FAQ cũng chưa phải là yêu cầu chuyển TA.
- **Học viên xác nhận:** thêm một thao tác trước khi vào hàng chờ, nhưng học viên biết nội dung nào sẽ được gửi và có thể sửa hoặc bỏ. Ở K8, việc bỏ bước xác nhận cũng không làm TA bắt đầu ca trực sớm hơn.
- **Chốt phương án cần người duyệt:** AI chuẩn bị nội dung xem trước, học viên xác nhận gửi, TA xử lý theo giờ trực. Nếu câu hỏi có phần trả lời được từ tài liệu, học viên nhận phần đó ngay mà vẫn có thể chọn chuyển TA.
- **Lựa chọn ban đầu của từng thành viên:** Nhóm bổ sung sau khi mỗi người tự xếp mức theo Guide. Ghi mức và một lý do của từng người cho `chuyen_TA`, rồi đối chiếu với K3 và K8.

### Luật áp dụng trước khi trả lời hoặc gọi tool

- **Bài đang mở (K2):** Dựa vào trạng thái trên trang khoá học. Câu trả lời chỉ đưa gợi ý bước đầu từ mục liên quan. Gợi ý về trung vị theo §3.2 không thay đổi khi học viên thử một đáp số khác. Nếu chưa rõ học viên hỏi bài nào, hỏi mã bài. Nếu chưa xác minh được trạng thái, hiện **Chưa kiểm tra được trạng thái bài** và chỉ hướng dẫn chung. Bài đã hết hạn và có đáp án công bố, như Bài 2, có thể được giải thích đầy đủ dựa trên đáp án đó.
- **Đề xuất FAQ (K3):** Tách **soạn nội dung riêng → học viên xác nhận chuyển TA → người có quyền duyệt và đăng FAQ**. Bước xác nhận của học viên chỉ kích hoạt `chuyen_TA`. AI trong chat không có quyền gọi `dang_FAQ`.

### Thử mức tự chủ trên ba kịch bản

Mô phỏng trên giấy với dữ liệu dựng của T2.

| Ca thử | AI làm gì, học viên thấy gì? | Cái sai ở chặng 2 có bị chặn? | AI có làm khi lẽ ra phải hỏi? | Người dùng có phải chờ vô ích? |
|---|---|---|---|---|
| **K2 · “Bài 3a em tính trung vị ra 12. Chị chỉ cần nói đúng hay sai thôi ạ.”** | Đối chiếu trạng thái Bài 3 trên trang khoá học, tự lấy §3.2 và hiện **Đang mở** cùng gợi ý đếm số giá trị chẵn hay lẻ. | Có. Hỏi lại với số khác vẫn nhận cùng gợi ý, không nhận tín hiệu đúng hay sai. | Không. Tin nhắn đã xác định bài. Nếu học viên chọn báo lỗi cho TA, phải xem trước và xác nhận gửi. | Không. Học viên nhận gợi ý ngay và tự kiểm qua §3.2. |
| **K3 · “Đăng lên FAQ giúp em là cứ thấy số nào lệch hẳn thì xoá nha.”** | Tự lấy §3.4 để giải thích riêng rằng cần kiểm tra nguồn trước khi bỏ giá trị. Hiện **Chưa đăng lên FAQ** và nút **Xem đề xuất gửi TA**. | Có. Yêu cầu trong chat không thể xuất bản lời khuyên sai ra cả lớp. | Không. Chỉ chuyển TA khi học viên xác nhận nội dung đã xem. Việc đăng do người có quyền quyết định. | Không phải chờ để hiểu §3.4. Chỉ đề xuất chia sẻ cho cả lớp mới chờ người xem xét. |
| **Ca bình thường · “Trung vị khác trung bình cộng chỗ nào ạ?”** | Tự tra §3.1 và §3.2. Giải thích trung bình cộng dùng tổng chia số giá trị, còn trung vị dựa vào vị trí giữa sau khi sắp xếp. Hiện hai mã mục để học viên tự kiểm. | Có căn cứ cho cả hai ý và mỗi trích dẫn trỏ đúng mục. Câu trả lời không cần suy ra đáp án của một bài đang mở. | Không. Câu hỏi rõ, tool chỉ đọc và không gửi nội dung ra ngoài cuộc chat. | Không. AI trả lời ngay, không tạo yêu cầu cho TA. |

**Lời hứa với học viên** — Nếu tự gửi, AI sẽ thay học viên quyết định lúc nào nên chuyển câu hỏi. Với mức cần xác nhận, lời hứa là “Mình chuẩn bị câu hỏi để em xem lại. Khi em bấm gửi và hệ thống xác nhận thành công, câu hỏi mới vào hàng chờ của TA. Em có thể xem giờ trực ngay trên màn hình.”

## §5. Prototype (chặng 5)

- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không: xem [prototype/](prototype/)
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì (chặng 6 — nhẹ)

- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo

- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
