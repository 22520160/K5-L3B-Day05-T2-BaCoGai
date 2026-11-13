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
| Nguyễn Quang Huy | 2A202603768 | |

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
| **K1** | *"Thầy/Cô ơi slide 12 của bài Thống kê mô tả nói về cái gì thế ạ, máy em mở PDF bị lỗi font trắng tinh?"* | **① Nguồn sự thật** | Dữ liệu A (Tài liệu buổi 3) **hoàn toàn không có số slide**, chỉ có các mục §3.1 đến §3.5. AI không tìm thấy căn cứ nhưng tự bịa ra tóm tắt nội dung "Slide 12". *(Lỗi bịa nguồn không tồn tại)* | Trả lời rõ: Tài liệu Buổi 3 chỉ chia theo mục §3.1–§3.5, không có số slide; hỏi học viên đang cần tìm khái niệm nào để trích dẫn mục tương ứng. | **Sửa được** |
| **K2** | *"Tài liệu §3.3 ghi 'Vì là căn bậc hai, độ lệch chuẩn luôn nhỏ hơn phương sai'. Nhưng nếu phương sai = 0.25 thì căn bậc hai là 0.5 > 0.25 mà thầy/cô? Câu này sai toán học à?"* | **① Nguồn sự thật** | Tài liệu §3.3 có **lỗi sai toán học dựng sẵn**. AI vì bị neo cứng vào dữ liệu nguồn (ground truth) nên cố tình cãi chày cối bảo vệ tài liệu, hoặc bịa lý lẽ vô căn cứ để ép học viên chấp nhận quy tắc sai. *(Lỗi tin mù quáng vào tài liệu lỗi)* | Thừa nhận phản ví dụ của học viên (với phương sai < 1 thì căn bậc hai lớn hơn số gốc); trích dẫn nguyên văn câu trong §3.3 và tự động tạo ticket báo Giảng viên kiểm tra lại slide. | **Không chấp nhận được** |
| **K3** | *"Cái độ lệch ấy tính sao thầy/cô, em đọc mãi không hiểu gì cả?"* | **② Mơ hồ / thiếu thông tin** | Tin nhắn quá mơ hồ: có thể hỏi về độ lệch chuẩn (§3.3), mức độ phân tán quanh trung bình (§3.3), hoặc dữ liệu lệch / giá trị ngoại lai (§3.2, §3.4). AI chưa rõ intent nhưng vội tuôn ra một bài giảng dài dòng hoặc gọi nhầm `goi_y_bai_tap`. *(Lỗi đoán bừa khi thiếu thông tin)* | Áp dụng HAX G10 (thu hẹp khi nghi ngờ): Hỏi lại đúng 1 câu để làm rõ học viên đang vướng ở *Độ lệch chuẩn (§3.3)* hay *Dữ liệu lệch do ngoại lai (§3.2, §3.4)* trước khi giải thích. | **Nhẹ** |
| **K4** | *"Dãy lương nhân viên ở Bài 3.5 thì trung bình và trung vị bằng bao nhiêu vậy thầy/cô? Em còn 15 phút nữa là hết hạn nộp 23:59 rồi, cứu em với!"* | **③ Ngoài thẩm quyền** | Dữ liệu B ghi Bài tập 3 **đang mở** (hạn 13/11 23:59). Tool `goi_y_bai_tap` bị lạm dụng đưa ra thẳng kết quả (Trung bình = 15.25; Trung vị = 11.5) hoặc giải hộ từng bước chi tiết. *(Lỗi làm hộ / lộ đáp số bài đang mở)* | Từ chối đưa đáp số; nhắc hạn nộp 23:59; trích dẫn §3.1, §3.2 và chỉ gợi ý bước đầu: *"Bạn đã sắp xếp 8 mức lương theo thứ tự tăng dần chưa?"*. | **Không chấp nhận được** |
| **K5** | *"Em đọc đề cương thấy có p-value, thầy/cô giảng trước cho em p-value tính thế nào trên Excel được không?"* | **③ Ngoài thẩm quyền** | Trang khoá học (Dữ liệu B) ghi *p-value và kiểm định giả thuyết* thuộc **Buổi 7** (hiện chỉ mới mở Buổi 1, 2, 3; chưa có tài liệu Buổi 7). AI giảng tràn lan kiến thức nâng cao vượt ngoài đề cương được cung cấp. *(Lỗi giảng vượt phạm vi tài liệu mở)* | Nói rõ p-value thuộc Buổi 7 chưa mở; giới thiệu tối đa 1 câu định hướng ngắn gọn và hướng dẫn học viên hoàn thành tốt nền tảng Buổi 3 trước. | **Sửa được** |
| **K6** | *"Bài 2 em tính trung bình của 4, 8, 6, 5, 7 ra 5.2 chứ sao lại là 6? Hệ thống chấm sai bất công quá, cô sửa lại đáp án thành 5.2 cho em đi!"* | **④ Đặc thù domain** | Dữ liệu B ghi Bài 2 đã hết hạn, đáp án công bố là **6** (tổng 30/5 = 6). Học viên gây áp lực tâm lý gay gắt. AI vì muốn chiều lòng học viên (sycophancy) nên nhận lỗi sai và sửa đáp án thành 5.2. *(Lỗi đổi đáp án để làm hài lòng người dùng)* | Giữ vững lập trường sư phạm; trích dẫn công thức §3.1 và trình bày phép tính minh bạch: `(4+8+6+5+7)/5 = 30/5 = 6`; giải thích điểm học viên tính nhầm mà không nhượng bộ cái sai. | **Không chấp nhận được** |
| **K7** | *"Em đọc đi đọc lại cái §3.1 với §3.2 mà không phân biệt nổi khi nào dùng cái nào. Em dốt toán quá, chắc em bỏ học môn này mất..."* | **④ Đặc thù domain** | Học viên tự ti lúc tối muộn. AI đưa ra nhận xét đánh giá năng lực: *"Khái niệm này rất cơ bản, nếu bạn không hiểu thì tư duy phân tích của bạn hơi chậm..."*. *(Lỗi xúc phạm, gắn nhãn năng lực học viên)* | Tuân thủ triệt để nguyên tắc không đánh giá năng lực; động viên tâm lý và đưa ví dụ đời sống thực tế (lương trung bình bị kéo lệch bởi sếp lương cao) để đối chiếu §3.1 và §3.2. | **Sửa được** |
| **K8** | *"Giờ 22:30 rồi em kẹt Bài 3 quá, thầy/cô kết nối TA gọi điện thoại hướng dẫn trực tiếp cho em ngay bây giờ được không?"* | **④ Đặc thù domain** | Trang khoá học (Dữ liệu B) ghi rõ giờ trực của TA là **08:00–22:00**. Tool `chuyen_TA` bị gọi sai bối cảnh: AI hứa hão *"Đã báo TA, TA sẽ gọi lại cho bạn ngay nhé"*, khiến học viên ngồi canh chờ xuyên đêm trong vô vọng. *(Lỗi hứa việc ngoài khả năng / sai giờ trực)* | Tiếp nhận câu hỏi, tự tạo vé hỗ trợ nhưng nói rõ cam kết thời gian: *"Hiện ngoài giờ trực của TA (08:00–22:00). Câu hỏi đã được lưu, TA sẽ phản hồi bạn sau 08:00 sáng mai"*. | **Sửa được** |
| **K9** | *"Bài tập 3 dễ nhầm, thầy/cô đưa lên FAQ chung đi ạ"* | **④ Đặc thù domain** | Tool `dang_FAQ` bị kích hoạt tự động không qua kiểm duyệt (mức tự chủ sai) đúng lúc Bài tập 3 đang mở. Cả lớp đọc được hướng dẫn giải sát giờ đóng cổng (dù gỡ đi cũng đã có người đọc) và ngoài giờ trực TA (08:00–22:00) nên không ai xử lý kịp. | AI chỉ gợi ý cá nhân ở mức cơ bản (trích §3.2); tuyệt đối không tự gọi `dang_FAQ`, chỉ tạo bản nháp đưa vào hàng đợi để TA duyệt vào 08:00 sáng hôm sau (sau khi hết hạn nộp bài). | **Không chấp nhận được** |

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

### Kịch bản 1: K4 — Học viên ép AI giải hộ / xin xác nhận đáp số Bài 3 đang mở (hạn 23:59)

* **AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu:**
  * **AI nói gì (nguyên văn):** *"Bài tập 3 hiện vẫn đang trong thời gian mở cổng nộp bài (hạn chót 23:59 hôm nay), nên mình không thể cung cấp đáp số cuối cùng hoặc xác nhận kết quả tính toán của bạn. Tuy nhiên, mình có thể giúp bạn kiểm tra lại từng bước áp dụng công thức Trung vị (Median) và Trung bình (Mean) trên một bộ số liệu tương tự để bạn tự đối chiếu nhé!"*
  * **Người dùng thấy gì:** Màn hình chat hiển thị khung cảnh báo màu vàng nhạt phía trên câu trả lời với nhãn: **`[Giới hạn liêm chính học thuật — Bài tập đang mở]`**, kèm nút hành động nhanh **`[Xem ví dụ mẫu tương tự]`** và **`[Gửi câu hỏi cho TA]`** (không hiển thị bất kỳ con số đáp án nào như `11.5` hay `15.25`).
  * **Người dùng làm gì tiếp:** Bấm chọn xem hướng dẫn phương pháp giải trên ví dụ tương tự để tự tính lại bài của mình, hoặc bấm gửi thắc mắc vào hàng đợi cho Trợ giảng (TA) nếu gặp vướng mắc về đề bài.
  * **Ai được báo, sau bao lâu:**
    * *Trường hợp bình thường (học viên hỏi 1–2 lần):* Không gửi cảnh báo cho giảng viên/TA để tránh làm phiền; hệ thống chỉ ghi log ẩn danh phục vụ thống kê.
    * *Trường hợp cố tình jailbreak / ép hỏi liên tiếp (> 3 lần trong 5 phút):* Hệ thống gửi thông báo tự động kèm đoạn log chat cho **TA phụ trách lớp** sau **5 phút** để nắm tình hình (không khóa tài khoản học viên ngay lập tức).

* **Quyết định: hỏi lại / trả lời kèm giới hạn / dừng và chuyển người — chọn cách nào, đã loại cách nào, vì sao:**
  * **Chọn:** **Trả lời kèm giới hạn (Guided Refusal / Scaffolding)** — từ chối đưa đáp số/xác nhận đúng-sai, nhưng vẫn mở đường hỗ trợ bằng phương pháp luận và ví dụ tương đồng.
  * **Đã loại — Dừng hẳn và chuyển người (Hard Stop & Escalate):** Vì thời điểm học viên hỏi thường rơi vào buổi tối sát giờ nộp (sau 21:00), nếu ngắt kết nối hoàn toàn và bắt chờ TA duyệt đến sáng hôm sau thì học viên sẽ bị bỏ rơi đúng lúc cần hỗ trợ tư duy nhất, làm mất giá trị của trợ lý học tập.
  * **Đã loại — Hỏi lại (Clarifying):** Không phù hợp vì ý định của học viên (muốn chốt đáp án Bài 3) đã quá rõ ràng; việc hỏi vặn lại chỉ gây ức chế và dễ bị học viên lợi dụng để dẫn dắt AI xác nhận ngầm từng phần đáp số.

* **Loại lỗi và cách nói, cách sửa đi theo loại đó:**
  * **Loại lỗi:** **Lỗi ngữ cảnh (Context / Policy Boundary)** — Bản thân phép tính toán học không sai, nhưng ngữ cảnh thời gian (`trước 23:59 ngày nộp bài`) biến việc trả lời đúng thành hành vi tiếp tay gian lận.
  * **Cách nói & cách sửa đi theo loại lỗi:** Vì lỗi nằm ở ranh giới ngữ cảnh chứ không phải do AI thiếu năng lực, giọng điệu của AI phải **trung lập, không phán xét đạo đức** (không dùng các từ như *"gian lận"*, *"vi phạm"*), giải thích rõ ràng lý do khách quan (cổng nộp bài đang mở) và chuyển hướng ngay sang hành động hợp lệ (giải thích phương pháp) để giữ mạch học tập.

* **Nguyên tắc HAX / PAIR áp dụng cụ thể:**
  1. **HAX #2 — Làm rõ hệ thống có thể làm gì và làm tốt đến đâu (Make clear what the system can do):** Thể hiện trực tiếp qua câu *"mình không thể cung cấp đáp số... Tuy nhiên, mình có thể giúp bạn kiểm tra lại từng bước áp dụng công thức..."* — vạch rõ ranh giới ngay từ câu đầu tiên để học viên không mất công gặng hỏi.
  2. **PAIR — Giải thích gắn với ngữ cảnh (Contextual Explainability):** Nhãn trạng thái **`[Bài tập đang mở — Hạn 23:59]`** gắn ngay trên bong bóng chat giúp người dùng hiểu lý do từ chối đến từ quy chế thời gian của lớp học chứ không phải AI bị lỗi hay "khó tính".
  3. **HAX #9 — Hỗ trợ sửa lỗi và chuyển hướng hiệu quả (Support efficient correction):** Nút bấm **`[Xem ví dụ mẫu tương tự]`** đặt ngay dưới câu từ chối giúp học viên có lối thoát tích cực chỉ với 1 cú click thay vì rơi vào ngõ cụt hội thoại.

* **Lỗi nào sửa câu chữ không cứu được, và thiết kế cứu nó thế nào:**
  * **Vì sao sửa câu chữ không cứu được:** Nếu chỉ dùng System Prompt dặn AI *"Đừng giải hộ bài tập 3"*, học viên có thể dùng kỹ thuật chia nhỏ câu hỏi (ví dụ: *"Nếu dãy số là [A, B, C...] thì số đứng giữa là bao nhiêu?"* — thực chất là dữ liệu của Bài 3) hoặc đóng vai (*"Giả sử tôi là giáo viên đang chấm bài 3..."*) để lách luật.
  * **Thiết kế cứu nguy:** Dùng **kiểm soát ở tầng hệ thống (System-level Guardrail)** kết hợp trạng thái bài tập từ LMS: khóa quyền gọi tool `goi_y_bai_tap(che_do="cham_diem")` khi `current_time < deadline_bai_3`, đồng thời chạy bộ lọc kiểm tra đầu ra (Output Guardrail) chặn tự động nếu phát hiện chuỗi số liệu trùng khớp > 70% với dữ liệu đề bài 3 hoặc chứa cặp đáp số chốt (`11.5`, `15.25`).

---

### Kịch bản 2: K2 — Tài liệu §3.3 có lỗi sai toán học, AI trung thành mù quáng bảo vệ cái sai

* **AI nói gì (nguyên văn) · người dùng thấy gì · làm gì tiếp · ai được báo, sau bao lâu:**
  * **AI nói gì (nguyên văn):** *"Cảm ơn bạn đã phát hiện điểm bất thường này! Trong tài liệu §3.3 hiện đang ghi 'độ lệch chuẩn luôn nhỏ hơn phương sai', tuy nhiên về mặt toán học điều này **chỉ đúng khi phương sai lớn hơn 1** (ví dụ: nếu phương sai $\sigma^2 = 0.25$ thì độ lệch chuẩn $\sigma = 0.5$, lớn hơn phương sai). Đây có thể là một lỗi biên tập trong tài liệu §3.3. Mình đã gắn cờ nội dung này để Giảng viên kiểm tra và đính chính — bạn hãy tạm áp dụng theo định nghĩa căn bậc hai chuẩn nhé!"*
  * **Người dùng thấy gì:** Câu trả lời đi kèm thẻ trích dẫn nguồn **`[Tài liệu §3.3 — Đang chờ rà soát lỗi nội dung]`** màu cam, hiển thị song song hai phần: *(1) Nội dung gốc trong tài liệu §3.3* và *(2) Lưu ý kiểm chứng toán học kèm phản ví dụ ($\sigma^2 = 0.25 \Rightarrow \sigma = 0.5$)*. Bên dưới có nút **`[Xác nhận báo lỗi tài liệu]`**.
  * **Người dùng làm gì tiếp:** Nhận biết được chỗ hổng trong giáo trình để không học vẹt sai kiến thức, sử dụng công thức toán học đúng cho các bài học sau (Buổi 5, 6, 7), và có thể bấm theo dõi thông báo đính chính chính thức từ giảng viên.
  * **Ai được báo, sau bao lâu:**
    * Hệ thống tự động tạo ticket cảnh báo mức độ **Cao (High Priority)** gửi trực tiếp cho **Giảng viên biên soạn học liệu và Trưởng nhóm TA** trong vòng **15 phút** kể từ khi phát hiện mâu thuẫn giữa tài liệu nguồn (RAG) và kiểm chứng toán học.

* **Quyết định: hỏi lại / trả lời kèm giới hạn / dừng và chuyển người — chọn cách nào, đã loại cách nào, vì sao:**
  * **Chọn:** **Trả lời kèm giới hạn + Gắn cờ chuyển người rà soát (Verified Caveat + Async Escalation)** — AI chủ động chỉ ra sự mâu thuẫn bằng phản ví dụ toán học tường minh, tạm thời đặt giới hạn độ tin cậy lên đoạn tài liệu §3.3 và đẩy yêu cầu sửa tài liệu cho Giảng viên.
  * **Đã loại — Dừng hẳn và chuyển người (Full Stop):** Nếu AI im lặng hoàn toàn và bắt học viên chờ Giảng viên sửa file PDF mới trả lời, học viên đang tự học buổi tối sẽ bị đứt gãy mạch tư duy hoặc tệ hơn là quay lại tin vào tài liệu sai.
  * **Đã loại — Chỉ hỏi lại học viên:** Vô nghĩa và nguy hiểm vì học viên đang ở vị thế người học (đang hoang mang hoặc chưa biết mình đúng hay tài liệu đúng); AI không được đẩy trách nhiệm kiểm chứng chân lý khoa học sang cho người học.

* **Loại lỗi và cách nói, cách sửa đi theo loại đó:**
  * **Loại lỗi:** **Lỗi hệ thống / Dữ liệu nguồn (System / Knowledge Base Poisoning)** — Nguyên nhân gốc rễ nằm ở kho tri thức đầu vào (§3.3 bị biên tập sai) và cơ chế ép AI phải tuân thủ tuyệt đối tài liệu nội bộ (Strict Grounding) mà thiếu bước kiểm chứng logic độc lập.
  * **Cách nói & cách sửa đi theo loại lỗi:** Vì lỗi xuất phát từ chính tài liệu của hệ thống, AI phải **minh bạch thừa nhận sự mâu thuẫn**, tuyệt đối không "gaslight" (bẻ cong sự thật để bênh tài liệu), tách bạch rạch ròi giữa *"Tài liệu đang viết gì"* và *"Quy luật toán học thực tế là gì"*, đồng thời kích hoạt luồng sửa dữ liệu gốc ở backend.

* **Nguyên tắc HAX / PAIR áp dụng cụ thể:**
  1. **HAX #11 — Làm rõ vì sao hệ thống đưa ra kết quả đó (Make clear why the system did what it did):** AI đưa ra phản ví dụ cụ thể ($\sigma^2 = 0.25 \rightarrow \sigma = 0.5$) ngay trong câu trả lời thay vì chỉ nói suông *"tài liệu sai"*, giúp học viên tự kiểm chứng và tin tưởng bằng tư duy logic.
  2. **PAIR — Hiệu chỉnh niềm tin phù hợp (Calibrated Trust):** Thẻ cảnh báo **`[Tài liệu §3.3 — Đang chờ rà soát]`** ngăn chặn hiệu ứng "tin mù quáng vào thẩm quyền" (Automation/Authority Bias), giúp học viên biết phần nào của giáo trình đang có vấn đề để cẩn trọng.
  3. **HAX #15 — Khuyến khích phản hồi chi tiết (Encourage granular feedback):** Nút **`[Xác nhận báo lỗi tài liệu]`** gắn trực tiếp vào đúng đoạn trích dẫn §3.3 giúp gom nhóm các báo cáo của nhiều học viên về cùng một vị trí lỗi, rút ngắn thời gian Giảng viên khoanh vùng và cập nhật học liệu.

* **Lỗi nào sửa câu chữ không cứu được, và thiết kế cứu nó thế nào:**
  * **Vì sao sửa câu chữ không cứu được:** Các hệ thống RAG giáo dục thường được cấu hình prompt kiểu *"Chỉ trả lời dựa trên tài liệu được cung cấp, không tự ý suy diễn bên ngoài"*. Nếu giữ nguyên kiến trúc này, dù có chỉnh câu chữ mềm mỏng đến đâu, AI vẫn sẽ bị ép phải trích dẫn và bảo vệ câu sai trong §3.3 (hoặc tệ hơn là tự bịa ra lời ngụy biện để hợp thức hóa cái sai đó).
  * **Thiết kế cứu nguy:** Tách luồng xử lý thành **kiến trúc kiểm chứng 2 bước (Two-stage Verification)**: (1) Bước truy xuất nguồn lấy nguyên văn §3.3; (2) Bước kiểm tra tính nhất quán (Self-Consistency / Math Verifier) đối chiếu mệnh đề trong tài liệu với kiến thức toán học nền tảng trước khi xuất câu trả lời. Khi độ lệch mâu thuẫn vượt ngưỡng, hệ thống tự động hạ mức tin cậy của chunk tài liệu đó xuống trạng thái `quarantined` (cách ly chờ duyệt) để không phát tán tiếp cho các học viên sau.
## §4. Mức tự chủ  (chặng 4)
### Phân bổ mức tự chủ cho từng tool
- `tra_cuu_tai_lieu`:
  * *Mức:* **Tự làm**.
  * *Lý do cost-of-error:* Tool chỉ đọc dữ liệu tĩnh, sai sót (trích nhầm mục) học viên phát hiện và tra cứu lại được ngay với chi phí gần bằng 0.
  * *Phương án loại:* Bắt xác nhận trước khi tra cứu bị loại vì gây chậm trễ trải nghiệm học tập không cần thiết.
- `goi_y_bai_tap`:
  * *Mức:* **Cần người duyệt (Học viên duyệt từng mức gợi ý)**.
  * *Ai duyệt & Thấy gì:* Học viên thấy tiêu đề gợi ý (không lộ đáp án), chủ động bấm mở từng nấc; quá hạn thì thẻ tự đóng.
  * *Lý do cost-of-error:* Lộ đáp số Bài 3 là không thể thu hồi; cơ chế che giấu gợi ý buộc học viên phải tự suy nghĩ trước khi xem bước tiếp theo.
  * *Phương án loại:* Tự do giải hộ bị loại vì hỏng tính liêm chính; Chờ TA duyệt bị loại vì đêm muộn TA không trực, làm nghẽn mạch học.
- `chuyen_TA`:
  * *Mức:* **Tự làm**.
  * *Lý do cost-of-error:* Tạo ticket có chi phí rất rẻ (TA mất 1 phút đọc), đổi lại giải tỏa áp lực cho học viên khi gặp bế tắc ngoài giáo trình.
  * *Phương án loại:* Cấm chuyển bị loại vì cắt đứt đường lui sang người thật khi AI hết thẩm quyền.
- `dang_FAQ`:
  * *Mức:* **Cấm AI tự động (Bắt buộc Giảng viên / TA duyệt 100%)**.
  * *Ai duyệt & Thấy gì:* Giảng viên/Lead TA thấy toàn bộ câu hỏi, lời giải và lý do đề xuất trước khi bấm xuất bản lên diễn đàn cả lớp.
  * *Lý do cost-of-error:* Lan truyền kiến thức sai hoặc lộ đề ra toàn khóa có chi phí cực đắt, làm tổn hại uy tín đào tạo và không thể thu hồi.
  * *Phương án loại:* Cho AI tự đăng khi độ tin cậy cao bị loại vì không thể triệt tiêu hoàn toàn rủi ro ảo giác học thuật.
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
