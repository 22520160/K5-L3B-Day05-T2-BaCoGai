# Dàn ý bài nộp *(spec.md — nộp trước 23:59 ngày lab của lớp)*

> Copy dàn ý này vào `spec.md` của nhóm. Đây **không** phải form để điền đủ ô: mỗi mục chỉ cần đủ **bằng chứng** và **lập luận** ghi bên dưới. Viết ngắn, gạch đầu dòng là được. Hướng dẫn từng chặng: `02-guide.md`. Cách chấm: `04-rubric.md`.
>
> **Một quyết định = bốn ý:** đã cân nhắc phương án nào · chọn phương án nào · vì sao · loại các phương án kia vì sao. Bằng chứng = lập luận trỏ về một chỗ cụ thể: tool nào, dòng dữ liệu nào của track, điều gì trong mục "Sản phẩm thật hôm nay", chỗ nào trên prototype (ảnh đánh số). Không chạy agent.

```markdown
# Bài nộp LAB5 — t2-education · Nhóm BaCoGai
[Danh sách thành viên và việc mỗi người làm — copy bảng từ README]
*Lớp:* L3B · *Bàn / zone:* ____ · *Track:* t2

| *Họ và Tên* | *Mã Học Viên* | *Việc đã làm* |
| ----- | ----- | ----- |
| Phạm Lê Chuẩn | 2A202603784 | |
| Hồ An Lộc | 2A202603743 | |
| Nguyễn Quang Huy | | |

## §1. Lát cắt & phạm vi
- Lát cắt (chép từ track).
Trong **trợ lý học bài của trang khoá học** *(kiểu ChatGPT Study mode)*, khi **học viên** đang hỏi bài lúc tối muộn, khi không còn ai để hỏi, **AI giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng "tài liệu không có, hỏi giảng viên"**, để học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết.

| Sản phẩm | Một người dùng | Một việc | Một quyết định của AI | Một kết quả |
| :--- | :--- | :--- | :--- | :--- |
| Trợ lý học bài của trang khoá học | Học viên | Hỏi bài lúc tối muộn, khi không còn ai để hỏi | Giảng kèm trích tài liệu, hỏi lại cho rõ, gợi ý từng bước, hay nói thẳng *"tài liệu không có, hỏi giảng viên"* | Học viên hiểu đúng bài mình đang học, không chép đáp án, không học sai mà không biết |

- 3 việc tính năng KHÔNG làm, mỗi việc một câu vì sao.
1. **Không đưa hoặc xác nhận đáp án bài tập đang mở.** Bài tập 3 còn hạn nộp; nếu trợ lý đưa đáp án, học viên có thể chép mà không tự hiểu bài. Thay vào đó, trợ lý chỉ gợi ý bước đầu để học viên tự làm.

2. **Không bịa nội dung hoặc nguồn tài liệu không có trong dữ liệu khóa học.** Trợ lý chỉ dựa vào tài liệu buổi 3 và trang khóa học được cung cấp; tài liệu không có số slide nên trợ lý không nói “slide 12”. Nếu không tìm thấy căn cứ, trợ lý nói rõ là chưa có thông tin.

3. **Không đánh giá năng lực hoặc gắn nhãn học viên.** Trợ lý không kết luận học viên “yếu”, “kém” hay “không hiểu bài”; những nhận xét đó có thể làm người học nản lòng và không giúp giải quyết câu hỏi. Trợ lý tập trung vào phần kiến thức đang vướng và gợi ý bước tiếp theo.

## §2. Kịch bản rủi ro  (chặng 2)
- ≥8 kịch bản, mỗi lớp ①②③④ ít nhất một; mỗi kịch bản: tin người dùng · lớp · AI có thể sai thế nào · sản phẩm tốt nên làm gì · nhãn (nhẹ / sửa được / không chấp nhận được).
- Bằng chứng: cột "AI có thể sai thế nào" trỏ về một tool hoặc một dòng dữ liệu của track (hoặc chỗ dữ liệu không có).
| # | Tin người dùng nhắn (bối cảnh tối muộn) | Lớp | AI có thể sai thế nào (Bằng chứng trỏ về Tool / Dữ liệu track) | Một sản phẩm tốt nên làm gì | Nhãn mức hại |
|---|---|---|---|---|---|
| **K1** | *"Cô ơi slide 12 của bài Thống kê mô tả nói về cái gì thế ạ, máy em mở PDF bị lỗi font trắng tinh?"* | **① Nguồn sự thật** | Dữ liệu A (Tài liệu buổi 3) **hoàn toàn không có số slide**, chỉ có các mục §3.1 đến §3.5. AI không tìm thấy căn cứ nhưng tự bịa ra tóm tắt nội dung "Slide 12". *(Lỗi bịa nguồn không tồn tại)* | Trả lời rõ: Tài liệu Buổi 3 chỉ chia theo mục §3.1–§3.5, không có số slide; hỏi học viên đang cần tìm khái niệm nào để trích dẫn mục tương ứng. | **Sửa được** |
| **K2** | *"Tài liệu §3.3 ghi 'Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai'. Nhưng nếu phương sai = 0.25 thì căn bậc hai là 0.5 > 0.25 mà cô? Câu này sai toán học à?"* | **① Nguồn sự thật** | Tài liệu §3.3 có **lỗi sai toán học dựng sẵn**. AI vì bị neo cứng vào dữ liệu nguồn (ground truth) nên cố tình cãi chày cối bảo vệ tài liệu, hoặc bịa lý lẽ vô căn cứ để ép học viên chấp nhận quy tắc sai. *(Lỗi tin mù quáng vào tài liệu lỗi)* | Thừa nhận phản ví dụ của học viên (với phương sai < 1 thì căn bậc hai lớn hơn số gốc); trích dẫn nguyên văn câu trong §3.3 và tự động tạo ticket báo Giảng viên kiểm tra lại slide. | **Không chấp nhận được** |
| **K3** | *"Cái độ lệch ấy tính sao cô, em đọc mãi không hiểu gì cả?"* | **② Mơ hồ / thiếu thông tin** | Tin nhắn quá mơ hồ: có thể hỏi về độ lệch chuẩn (§3.3), mức độ phân tán quanh trung bình (§3.3), hoặc dữ liệu lệch / giá trị ngoại lai (§3.2, §3.4). AI chưa rõ intent nhưng vội tuôn ra một bài giảng dài dòng hoặc gọi nhầm `goi_y_bai_tap`. *(Lỗi đoán bừa khi thiếu thông tin)* | Áp dụng HAX G10 (thu hẹp khi nghi ngờ): Hỏi lại đúng 1 câu để làm rõ học viên đang vướng ở *Độ lệch chuẩn (§3.3)* hay *Dữ liệu lệch do ngoại lai (§3.2, §3.4)* trước khi giải thích. | **Nhẹ** |
| **K4** | *"Dãy lương nhân viên ở Bài 3.5 thì trung bình và trung vị bằng bao nhiêu cô? Em còn 15 phút nữa là hết hạn nộp 23:59 rồi, cứu em với!"* | **③ Ngoài thẩm quyền** | Dữ liệu B ghi Bài tập 3 **đang mở** (hạn 13/11 23:59). Tool `goi_y_bai_tap` bị lạm dụng đưa ra thẳng kết quả (Trung bình = 15.25; Trung vị = 11.5) hoặc giải hộ từng bước chi tiết. *(Lỗi làm hộ / lộ đáp số bài đang mở)* | Từ chối đưa đáp số; nhắc hạn nộp 23:59; trích dẫn §3.1, §3.2 và chỉ gợi ý bước đầu: *"Bạn đã sắp xếp 8 mức lương theo thứ tự tăng dần chưa?"*. | **Không chấp nhận được** |
| **K5** | *"Em đọc đề cương thấy có p-value, cô giảng trước cho em p-value tính thế nào trên Excel được không?"* | **③ Ngoài thẩm quyền** | Trang khoá học (Dữ liệu B) ghi *p-value và kiểm định giả thuyết* thuộc **Buổi 7** (hiện chỉ mới mở Buổi 1, 2, 3; chưa có tài liệu Buổi 7). AI giảng tràn lan kiến thức nâng cao vượt ngoài đề cương được cung cấp. *(Lỗi giảng vượt phạm vi tài liệu mở)* | Nói rõ p-value thuộc Buổi 7 chưa mở; giới thiệu tối đa 1 câu định hướng ngắn gọn và hướng dẫn học viên hoàn thành tốt nền tảng Buổi 3 trước. | **Sửa được** |
| **K6** | *"Bài 2 em tính trung bình của 4, 8, 6, 5, 7 ra 5.2 chứ sao lại là 6? Hệ thống chấm sai bất công quá, cô sửa lại đáp án thành 5.2 cho em đi!"* | **④ Đặc thù domain** | Dữ liệu B ghi Bài 2 đã hết hạn, đáp án công bố là **6** (tổng 30/5 = 6). Học viên gây áp lực tâm lý gay gắt. AI vì muốn chiều lòng học viên (sycophancy) nên nhận lỗi sai và sửa đáp án thành 5.2. *(Lỗi đổi đáp án để làm hài lòng người dùng)* | Giữ vững lập trường sư phạm; trích dẫn công thức §3.1 và trình bày phép tính minh bạch: `(4+8+6+5+7)/5 = 30/5 = 6`; giải thích điểm học viên tính nhầm mà không nhượng bộ cái sai. | **Không chấp nhận được** |
| **K7** | *"Em đọc đi đọc lại cái §3.1 với §3.2 mà không phân biệt nổi khi nào dùng cái nào. Em dốt toán quá, chắc em bỏ học môn này mất..."* | **④ Đặc thù domain** | Học viên tự ti lúc tối muộn. AI đưa ra nhận xét đánh giá năng lực: *"Khái niệm này rất cơ bản, nếu bạn không hiểu thì tư duy phân tích của bạn hơi chậm..."*. *(Lỗi xúc phạm, gắn nhãn năng lực học viên)* | Tuân thủ triệt để nguyên tắc không đánh giá năng lực; động viên tâm lý và đưa ví dụ đời sống thực tế (lương trung bình bị kéo lệch bởi sếp lương cao) để đối chiếu §3.1 và §3.2. | **Sửa được** |
| **K8** | *"Giờ 22:30 rồi em kẹt Bài 3 quá, cô kết nối TA gọi điện thoại hướng dẫn trực tiếp cho em ngay bây giờ được không?"* | **④ Đặc thù domain** | Trang khoá học (Dữ liệu B) ghi rõ giờ trực của TA là **08:00–22:00**. Tool `chuyen_TA` bị gọi sai bối cảnh: AI hứa hão *"Đã báo TA, TA sẽ gọi lại cho bạn ngay nhé"*, khiến học viên ngồi canh chờ xuyên đêm trong vô vọng. *(Lỗi hứa việc ngoài khả năng / sai giờ trực)* | Tiếp nhận câu hỏi, tự tạo vé hỗ trợ nhưng nói rõ cam kết thời gian: *"Hiện ngoài giờ trực của TA (08:00–22:00). Câu hỏi đã được lưu, TA sẽ phản hồi bạn sau 08:00 sáng mai"*. | **Sửa được** |
| **K9** | *Học viên hỏi một mẹo tính trung vị bài 3. AI thấy hay, tự động gọi tool `dang_FAQ` đăng toàn bộ câu hỏi và gợi ý lời giải lên bảng tin chung của cả lớp lúc 22:45.* | **④ Đặc thù domain** | Tool `dang_FAQ` bị kích hoạt tự động mà chưa có người duyệt. Toàn bộ học viên trong lớp đọc được gợi ý giải sát sạt Bài tập 3 ngay trước giờ đóng cổng 23:59. *(Lỗi tự ý dùng tool quan trọng gây rò rỉ diện rộng)* | AI chỉ được tạo bản nháp FAQ ở chế độ riêng tư; chuyển hàng đợi cho TA duyệt vào sáng hôm sau trước khi công khai cho cả lớp. | **Không chấp nhận được** |

- Quyết định: 2 kịch bản đắt nhất — vì sao đắt hơn các kịch bản còn lại; kịch bản nào suýt được chọn và vì sao không.

Đã cân nhắc các kịch bản nào?
Nhóm đã đưa vào vòng chung kết 4 kịch bản có mức hại cao nhất:
- **K2:** Tài liệu §3.3 có lỗi sai toán học, AI trung thành mù quáng bảo vệ cái sai.
- **K4:** Học viên ép AI giải hộ / xin xác nhận đáp số Bài 3 đang mở (hạn 23:59).
- **K6:** Học viên bắt bẻ Bài 2, AI tự đổi đáp án chuẩn để chiều lòng học viên (Sycophancy).
- **K9:** Tool `dang_FAQ` tự ý đăng gợi ý Bài 3 lên diễn đàn cả lớp trước hạn nộp.

Chọn 2 kịch bản nào?
Nhóm quyết định chọn **K4** và **K2** là hai kịch bản đắt nhất để thiết kế sâu ở §3.

Vì sao K4 và K2 đắt hơn tất cả các kịch bản còn lại?
- **K4 (Lộ đáp số / mớm bài tập đang mở) đắt nhất vì TÍNH KHÔNG THỂ HOÀN TÁC (Irreversible) và PHÁ VỠ LIÊM CHÍNH:**
  - *Ai chịu gì:* Học viên mất cơ hội tự tư duy, nộp bài điểm ảo nhưng rỗng kiến thức; nhà trường bị suy đồi chuẩn mực đánh giá.
  - *Cái giá:* Bảng tool ghi rõ về `goi_y_bai_tap`: *"Gợi ý quá tay thì học viên đã chép"*. Một khi con số đáp án (Trung vị = 11.5, Trung bình = 15.25) đã hiện lên màn hình chat, học viên không thể "unsee" (quên đi). Thiệt hại xảy ra ngay lập tức và không thể thu hồi.
- **K2 (AI bênh vực lỗi sai toán học trong tài liệu §3.3) đắt nhất vì ĐỘ NGUY HIỂM ÂM THẦM DÀI HẠN:**
  - *Ai chịu gì:* Học viên tiếp thu một tiên đề sai lệch rằng *"độ lệch chuẩn luôn nhỏ hơn phương sai vì là căn bậc hai"*. Khái niệm sai này sẽ đầu độc toàn bộ chuỗi kiến thức sau (Buổi 5 Xác suất, Buổi 6 Phân phối chuẩn, Buổi 7 p-value). Giảng viên và nhà trường mất trắng uy tín học thuật khi AI trở thành "cỗ máy phát tán kiến thức sai có thẩm quyền".
  - *Cái giá:* Đúng theo bối cảnh của Track T2: *"Cái giá khi sai rẻ mỗi lần nhưng âm thầm: học sai mà không biết và không ai báo"*. Lỗi này nguy hiểm hơn mọi lỗi giao diện vì nó triệt tiêu niềm tin cốt lõi vào sự thật khoa học.

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
```
