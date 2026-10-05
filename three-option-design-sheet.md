# Three-option Design Sheet — nhóm DBH, Case B

## 1. Evidence Snapshot và Hypothesis Problem

| Practice Note Day 17 | Người học đã thực sự làm/nói gì? | Diễn giải của nhóm và giới hạn |
|---|---|---|
| Phạm Quốc Đạt | Trong buổi học liên quan RAG, interviewee nói “mình chỉ ghi những cái đề mục chính” và “mình chỉ ghi những cái từ khóa liên quan thôi”; giảng và trả lời nhanh nên không ghi kịp phần giải thích. Khi xem lại có thể không chắc nhớ đúng và phải tìm hiểu lại/hỏi AI. | Tín hiệu trực tiếp cho vấn đề ghi thiếu ngữ cảnh. Đây là một lượt practice, chưa đủ chứng minh pain phổ biến. |
| Nguyễn Văn Biển | Người được phỏng vấn dùng AI lấy ý chính từ slide, xem video, tự tổng hợp bằng Markdown. Họ nói ghi tay tốn thời gian nhưng cũng giúp nhớ. | Không kể tình huống không ghi kịp tương tự. Evidence này làm nhóm thận trọng khi khái quát vấn đề cho mọi người học. |
| Mai Tiến Huy | Ghi chép tóm tắt nêu người học dùng Ctrl+F để tìm, có lúc không xem lại ghi chú. Không có bản ghi gốc trong tài liệu nhóm cung cấp. | Liên quan việc tìm và xem lại, không xác nhận trực tiếp giả thuyết ghi không kịp. Các câu trả lời đánh dấu mock trong notes_HUY.md không dùng làm evidence. |

**Hypothesis Problem nhóm tiếp tục:** Khi một buổi học có nhiều khái niệm được trình bày nhanh, người học muốn giữ đủ phần giải thích để xem lại, nhưng không ghi kịp; ghi chú chỉ còn từ khóa hoặc thiếu ngữ cảnh, khiến họ không chắc mình hiểu đúng và phải tìm hiểu lại sau buổi học.

**Evidence hỗ trợ ban đầu:** một chuyện cụ thể trong Practice Note của Đạt về ghi từ khóa vì không kịp phần giảng và phải tìm hiểu lại.

**Chưa được chứng minh:** vấn đề này có lặp ở nhiều người không; cơ chế nào thực sự giúp người học ôn lại mà không tạo cảm giác chắc chắn sai; người học có kiểm tra nguồn và chỗ chưa biết không. Không gọi hypothesis là validated.

## 2. Comparison Contract

| Thành phần giữ chung | Nội dung |
|---|---|
| Target user | Người học từng ghi chú trong lúc học để xem lại. |
| Situation | Bài giảng nhanh, chỉ giữ được một ghi chú vội. |
| Starter note | “RAG — lấy tài liệu trước khi AI trả lời?” |
| Content fixture | Slide 12 mẫu: “Truy xuất tài liệu liên quan → đưa vào ngữ cảnh → AI tạo câu trả lời.” Slide không ghi nguyên văn lời giảng. Đây là tình huống thiết kế mẫu, không được trình bày như câu nói thực tế trong Day 17. |
| Task | Chuẩn bị một ghi chú để ngày mai ôn bài và làm bài tập. |
| Desired outcome | Lưu được ý hữu ích, biết nguồn của phần thông tin bổ sung và biết điều gì vẫn cần kiểm tra. |
| Visual scope | Cùng tiêu đề, bố cục hai cột, nội dung bối cảnh, typography và màu; khác ở critical interaction. |

## 3. Ba Solution Options có cơ chế khác nhau

| Thành phần | A — Ghi chú theo khung | B — Ghi chú gắn với nguồn | C — Bản nháp AI có kiểm chứng |
|---|---|---|---|
| Solution mechanism | Cấu trúc buộc người học tách điều nhớ, điều thiếu và bước kiểm tra. | Ghi chú được neo vào đúng slide để lần sau mở cùng nguồn. | Bản nháp đề xuất từ ghi chú vội + slide, người học kiểm tra trước khi lưu. |
| User làm gì? | Tự diễn đạt, đánh dấu chỗ thiếu, lưu/sửa. | Viết ghi chú, chọn liên kết Slide 12, lưu/sửa. | Yêu cầu bản nháp, đối chiếu slide, sửa/bỏ, xác nhận lưu. |
| AI làm gì? | Không dùng AI. | Không dùng AI; hệ thống chỉ liên kết ghi chú với slide. | Trong prototype, bản nháp cố định mô phỏng kết quả AI; không gọi mô hình thật. |
| Trigger | Người học mở khung ghi chú. | Người học bấm gắn vào Slide 12. | Người học bấm tạo bản nháp. |
| Trade-off chính | Giữ quyền tự diễn đạt, nhưng tốn công và có thể vẫn thiếu kiến thức. | Dễ truy lại ngữ cảnh gốc, nhưng slide không chứa toàn bộ lời giảng. | Tạo nội dung nhanh, nhưng dễ tin quá mức hoặc bỏ qua điều AI không biết. |

**Distance check:** A khác B ở cách tạo ngữ cảnh: tự tổ chức phần mình biết/chưa biết so với neo ghi chú vào nguồn cụ thể. B khác C ở ai tạo nội dung: người học tự viết so với hệ thống đề xuất bản nháp để người học duyệt. A khác C ở mức tự động hóa: tự tạo ghi chú so với chỉnh và xác nhận bản nháp đề xuất. Khác biệt là cơ chế thao tác và phân quyền, không chỉ là màu hay câu chữ.

## 4. Human–AI Design Pass

Chỉ xét critical interaction “từ ghi chú vội đến ghi chú để ôn”. Với A/B, phần AI là “không có”; vẫn nêu rõ vai trò hệ thống và quyền của người học.

| Human–AI decision | Option A | Option B | Option C |
|---|---|---|---|
| User làm gì? AI/hệ thống làm gì? | User tự điền và quyết định lưu; hệ thống hiển thị lại. | User chọn nguồn và viết nội dung; hệ thống giữ liên kết với Slide 12. | User yêu cầu, sửa, xác nhận hoặc bỏ; bản nháp mô phỏng được hệ thống đưa ra. |
| Act / Ask / Don't Act? Vì sao? | Don't Act: không tự bổ sung phần giảng không có evidence. | Ask: cần user bấm gắn nguồn; không tự nhận slide là toàn bộ lời giảng. | Ask trước khi tạo và trước khi lưu; không tự lưu để tránh bản nháp chưa kiểm chứng thành “sự thật”. |
| User hiểu capability và giới hạn ra sao? | Khung ghi “tự điền”; không hàm ý hệ thống biết câu trả lời. | Hiển thị tên Slide 12 và cảnh báo slide không có nguyên văn lời giảng. | Ghi rõ bản nháp mô phỏng, dựa trên ghi chú + slide, không biết lời giảng ngoài slide. |
| Evidence và uncertainty được thể hiện thế nào? | Có trường “Phần còn thiếu hoặc chưa chắc” và “Việc cần kiểm tra”. | Bản lưu hiện nguồn Slide 12 và trường cần kiểm tra. | Bản nháp có nhãn “cần kiểm tra”, vùng nội dung có nguồn, cảnh báo phần giải thích chưa xác minh. |
| User sửa khi sai hoặc muốn lấy lại quyền kiểm soát thế nào? | Sửa ghi chú đã lưu. | Mở lại nguồn/sửa ghi chú; có thể bỏ liên kết trước khi lưu. | Sửa trực tiếp, bỏ bản nháp, sửa bản đã lưu hoặc quay về ghi chú vội. |
| Nếu sai, hệ quả gì? | Người học có thể tự điền sai; chỗ chưa chắc được giữ riêng. | Người học có thể tưởng slide đủ lời giảng; nhãn giới hạn nguồn giúp phát hiện. | Người học có thể tin bản nháp như lời giảng; bước review, nhãn nguồn và xác nhận giảm rủi ro, chưa chứng minh người dùng sẽ chú ý. |

## 5. Prototype scope và chú thích

Mỗi prototype có ba trạng thái chính: bối cảnh chung → critical interaction → ghi chú đã lưu/quyết định người học. Nội dung slide, ghi chú vội, task và visual giữ chung. Xem [ba HTML](prototype-link.md).

| Option | Điểm cần người test thử | Đường lấy lại quyền kiểm soát |
|---|---|---|
| A | Người học có hiểu và điền được phần “còn thiếu/chưa chắc” mà không bị ép bịa lời giảng? | “Sửa ghi chú”. |
| B | Người học có nhận ra ghi chú đã liên kết nguồn và hiểu giới hạn của slide? | “Xem lại nguồn / sửa ghi chú”. |
| C | Người học có phân biệt bản nháp với nguồn, xem và sửa trước khi lưu? | “Bỏ bản nháp”, “Sửa bản đã lưu”, “Bỏ và quay về ghi chú vội”. |

## 6. Test Prompt và Observation Focus

**Relevant context:** người học trong buổi học mẫu chỉ kịp ghi “RAG — lấy tài liệu trước khi AI trả lời?”; Slide 12 mẫu cho ba bước của RAG, không có nguyên văn lời giảng.

**Task chung:** “Ngày mai bạn cần xem lại ý này để làm bài tập. Hãy dùng cách đang mở để chuẩn bị một ghi chú cho lúc ôn bài. Khi nghĩ mình đã xong, hãy nói với người điều phối.” Mỗi tester thử cả ba option; ba thứ tự A→B→C, B→C→A và C→A→B giúp giảm ảnh hưởng thứ tự.

**Outcome cần quan sát:** tester tự tạo/lưu được ghi chú; hiểu phần nào từ ghi chú vội, phần nào từ slide/bản nháp; nhận ra điều chưa chắc; tìm được cách sửa hoặc bỏ. Người điều phối không chỉ nút cần bấm.

**Observation focus:** first action; chỗ dừng/hiểu sai; nhãn nguồn và giới hạn có được đọc; cách lấy lại quyền kiểm soát; option được chọn cùng lý do và trade-off. Sau mỗi option hỏi người học ghi chú nói gì và họ sẽ sửa/kiểm tra ở đâu. Sau cả ba hỏi chọn A/B/C trong tình huống này, vì sao, và điều gì ở phương án đã chọn vẫn khiến họ chưa thoải mái.

Kết quả phiên Đạt điều phối nằm trong [Feedback Note cá nhân](prototype-feedback-note.md); pattern ba phiên và quyết định nhóm ở [Group Feedback Synthesis](group-feedback-synthesis.md). Nội dung thiết kế ở các mục trên mô tả prototype đã đem đi thử. Các lỗi được phát hiện sau test, đặc biệt bản nháp C cố định và có thể lưu rỗng, không được sửa vào bản gốc trước khi ba phiên hoàn tất.
