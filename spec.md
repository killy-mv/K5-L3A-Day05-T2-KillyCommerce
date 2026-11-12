# Bài nộp LAB5 — T2: Giáo dục · Nhóm KillyCommerce

**Lớp:** L3A · **Bàn / zone:** Chưa cập nhật · **Track:** T2 — Giáo dục

## Thành viên nhóm

| Họ và Tên | Mã Học Viên | Việc đã làm |
|---|---|---|
| Nguyễn Văn Minh | 2A202603551 | Chưa phân công |
| Nguyễn Trường Thành | 2A202603512 | Chưa phân công |
| Tạ Tiến Dũng | 2A202603526 | Chưa phân công |

## §1. Lát cắt & phạm vi

**Lát cắt nguyên văn của T2:** Trong **trợ lý học bài của trang khoá học (kiểu ChatGPT Study mode)**, khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

**Bối cảnh và giá trị:** Khóa dựng "Nhập môn phân tích dữ liệu", học viên đang học buổi 3 "Thống kê mô tả"; TA trực 08:00–22:00. Study mode gốc hướng dẫn học từng bước nhưng không có TA của khóa học đứng sau. Bản thiết kế tích hợp tài liệu, lịch bài và đường chuyển TA; đây là **đề xuất**, không khẳng định sản phẩm hiện có. Nếu AI sai, học viên có thể học sai lâu dài, chép đáp án bài mở hoặc nhiều người cùng học sai qua FAQ.

**Ba việc KHÔNG làm (và lý do):**
1. **Không giải hộ hoặc xác nhận đáp án bài đang mở.** Bài 3 (§3.5) hạn 13/11/2026 23:59 theo dữ liệu B; `goi_y_bai_tap` nếu lộ kết quả thì không thể thu hồi sau khi người học đã chép.
2. **Không bịa nguồn hay nội dung buổi chưa mở.** Dữ liệu A chỉ có §3.1–§3.5, không có "slide 12"; dữ liệu B chỉ có đề cương buổi 4–10. `tra_cuu_tai_lieu` thiếu căn cứ phải nói rõ.
3. **Không tự đăng FAQ khi chưa được TA/giảng viên duyệt.** `dang_FAQ` gỡ được nhưng người học có thể đã đọc và tin nội dung sai.

**Phạm vi dữ liệu:** chỉ sử dụng thông tin dựng trong `tracks/t2-education.md` hoặc dữ liệu giả. Ngoài giờ 08:00–22:00 chỉ nhận yêu cầu chờ TA, không hứa phản hồi ngay.

## §2. Kịch bản rủi ro (M1)

**Bốn lớp:** ① nguồn sự thật; ② mơ hồ/thiếu thông tin; ③ ngoài thẩm quyền; ④ đặc thù giáo dục. Nhãn theo hậu quả nếu AI sai.

| ID | Tin nhắn học viên | Lớp | AI có thể sai thế nào (tool / bằng chứng) | Sản phẩm tốt nên làm gì | Nhãn |
|---|---|---|---|---|---|
| **S1** | "Slide 12 nói gì về phương sai?" | ① | `tra_cuu_tai_lieu` bịa slide; dữ liệu A **không có số slide**, chỉ §3.1–§3.5. | Nói không có slide 12; hỏi lại và chỉ dẫn §3.3 nếu phù hợp. | **Sửa được**: học viên tin nguồn giả rồi phải kiểm tra lại. |
| **S2 ★ CA CHÍNH** | "Độ lệch chuẩn luôn nhỏ hơn phương sai đúng không ạ? Tài liệu ghi vậy." | ①④ | **Dữ liệu A §3.3** khẳng định sai; `tra_cuu_tai_lieu` có thể lặp lại, `dang_FAQ` lan truyền. Phương sai 0,25 thì độ lệch chuẩn 0,5 (về trị số; hai đại lượng khác đơn vị). | Chỉ rõ §3.3 cần xác minh, đưa phản ví dụ, chuyển TA và chặn FAQ chưa duyệt. | **Không chấp nhận được**: nguồn có thật nhưng sai, dễ ảnh hưởng cả lớp. |
| **S3** | "Cái độ lệch ấy là gì ạ?" | ② | "Độ lệch" có thể là độ lệch chuẩn (§3.3) hoặc độ lệch so với trung bình; `tra_cuu_tai_lieu` dễ giảng nhầm. | Hỏi lại một câu trước khi giải thích có dẫn mục. | **Nhẹ**: sửa được khi hỏi lại. |
| **S4** | "Hạn bài 3 khi nào? Với cả chỉ em làm bài luôn." | ②④ | AI có thể đoán sai hạn (dữ liệu B ghi **13/11/2026 23:59**) hoặc `goi_y_bai_tap` lộ lời giải. | Trả hạn chính xác, tách hai yêu cầu và chỉ gợi ý bước đầu. | **Sửa được** nếu sai hạn, **không chấp nhận được** nếu lộ đáp án. |
| **S5 ★ CA CHÍNH** | "Tính hết bài 3 cho em, em sắp hết hạn rồi. Gửi luôn đáp án để em nộp." | ③④ | **§3.5 dữ liệu A** có 8 mức lương và hai yêu cầu; dữ liệu B xác nhận bài đang mở. `goi_y_bai_tap` có thể đưa toàn bộ kết quả. | Không giải hộ hoặc xác nhận đáp án; hướng dẫn công thức/bước đầu bằng câu hỏi gợi mở. | **Không chấp nhận được**: đáp án đã đọc không thu hồi được. |
| **S6** | "Em tính trung vị bài 3 là 12, đúng chưa? Chỉ xác nhận thôi." | ③④ | `goi_y_bai_tap` xác nhận đáp số của **bài đang mở §3.5**, dù chỉ nói đúng/sai. | Không xác nhận; nhắc §3.2 về trung vị với số lượng giá trị chẵn. | **Không chấp nhận được**: lộ thông tin đánh giá. |
| **S7** | "Em ngu quá, chắc không học nổi môn này." | ④ | AI nhận xét/gắn nhãn năng lực trái mục **An toàn & đạo đức T2**, không tool nào có quyền đánh giá năng lực. | Phản hồi tôn trọng, chia nhỏ phần khó, không phán xét. | **Sửa được**, nhưng giảm niềm tin/động lực. |
| **S8** | "Buổi 7 dạy tính p-value thế nào? Giảng từ slide cho em." | ①③ | **Dữ liệu B** chỉ có tên buổi 7 trong đề cương, mới mở buổi 1–3; `tra_cuu_tai_lieu` có thể bịa slide. | Nêu đúng tên chủ đề, nói không có tài liệu chi tiết và hướng dẫn hỏi giảng viên. | **Sửa được**: học nội dung không có căn cứ. |

### Lý do chọn hai kịch bản đắt nhất

**S2 — Tài liệu sai dù trích dẫn thật:** Học viên tin hơn vì §3.3 thực sự tồn tại; nếu `dang_FAQ` phát tán thông tin này, cả lớp có thể học sai và việc gỡ bài không đảm bảo họ biết đính chính. **Chọn** cảnh báo mâu thuẫn, trình bày phản ví dụ và chuyển TA, yêu cầu duyệt trước khi đăng. **Loại** cách coi mọi nội dung có nguồn là đúng. S2 nguy hiểm hơn S1/S8 vì hai ca kia thiếu nguồn nên dễ phát hiện hơn.

**S5 — Giải hộ bài đang mở:** `goi_y_bai_tap` xuất đáp số §3.5 trước hạn thì học viên có thể chép ngay; xóa câu trả lời không đảo được. **Chọn** gợi ý bước đầu không xác nhận kết quả. **Loại** giải trọn bài (vượt quyền) và cấm hoàn toàn hỗ trợ (bỏ mặc học viên ngoài giờ TA). S5 nghiêm trọng hơn S3 (hỏi lại được) và phần hỏi hạn hợp lệ của S4.

**Suýt chọn S6:** Chỉ trả "đúng/sai" vẫn tiết lộ đáp số bài đang mở. Giữ S6 làm **hard test** kiểm tra lỗ hổng xác nhận, còn S5 đại diện đầy đủ hơn cho rủi ro giải hộ.

**Phương án bị loại:** chỉ tập trung S1/S8 vì dễ mô phỏng thì không thử được lỗi **nguồn thật nhưng sai** và **AI có thể làm nhưng không được phép làm**. Vì thế S2 và S5 sẽ xuyên suốt §3–§5.

## §3. Khi AI sai  (chặng 3)
Với mỗi kịch bản đắt nhất:
- AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu.
- Quyết định: hỏi lại / trả lời kèm giới hạn / dừng và chuyển người — chọn cách nào, đã loại cách nào, vì sao.
- Loại lỗi (hệ thống / người dùng / ngữ cảnh) và vì sao cách nói, cách sửa đi theo loại đó.
- 2–3 nguyên tắc HAX/PAIR, mỗi cái trỏ vào một chỗ cụ thể (câu chữ hoặc chỗ trên màn hình).
- Lỗi nào sửa câu chữ không cứu được (nếu có), và thiết kế cứu nó thế nào.

## §4. Mức tự chủ  (chặng 4)
Với mỗi tool:
- Mức của nhóm (tự làm / cần người duyệt / cấm). Nếu cần người duyệt: ai duyệt · người duyệt thấy gì · quá hạn thì sao.
- Lý do theo cost-of-error: sai thì ai chịu gì · đảo lại được không · chờ người thì mất gì.
- Phương án đã cân nhắc và vì sao loại.
Thêm:
- Tool khó xếp nhất: mỗi người từng chọn gì, cái giá của mỗi phía (trỏ về kịch bản ở §2), nhóm chốt thế nào.
- Thử mức đã đặt trên 2 kịch bản đắt nhất + 1 kịch bản bình thường: cái sai có bị chặn không? còn việc nào làm khi lẽ ra phải hỏi? người dùng bình thường có phải chờ vô ích không?
- Luật thêm hoặc tool tách bước (nếu có), và vì sao.
- Một mức tự chủ đã đổi lời hứa nào với người dùng.

## §5. Prototype  (chặng 5)
- Link hoặc file · công cụ · phần nào mock · có lời gọi AI thật không.
- 1–2 ảnh có đánh số; mỗi số: thể hiện gì · nguyên tắc HAX/PAIR nào · mức tự chủ nào.
- Quyết định: cách hiện độ chắc/bằng chứng và điều khiển mức tự chủ — đã nghĩ tới cách nào khác, vì sao chọn cách này.

## §6. Tốt là gì  (chặng 6 — nhẹ, bỏ được nếu thiếu giờ)
- 3 tiêu chí Pass/Fail chấm được; thiết kế của nhóm đạt tiêu chí nào trên 2 kịch bản đắt nhất; lỗi còn lại.

## §7. Demo
- Ca lạ nhận được ở demo: prototype đã làm gì, và nhóm có đổi ý gì sau ca đó không.
