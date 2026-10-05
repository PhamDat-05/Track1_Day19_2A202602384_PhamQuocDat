# Prototype Feedback Note 1 — Ninh Quang Minh

**Nguồn ghi chép:** Phạm Quốc Đạt trực tiếp điều phối, chuyển lại thao tác và câu trả lời của **Ninh Quang Minh (2A202602432)** để biên tập theo mẫu. AI hỗ trợ biên tập tài liệu, không tham gia buổi test.

- **Tester/context:** Ninh Quang Minh (2A202602432); theo thông tin Đạt cung cấp, Minh đã ghi chú/lưu nội dung khi học trong 7 ngày trước buổi thử.
- **Người facilitate:** Phạm Quốc Đạt.
- **Ngày test:** 05/10/2026. Hình thức gặp trực tiếp hay trực tuyến chưa được nêu.
- Thứ tự: A → B → C
- **Task:** “Trong buổi học mẫu về RAG, bạn chỉ kịp ghi: ‘RAG — lấy tài liệu trước khi AI trả lời?’. Ngày mai bạn cần xem lại ý này để làm bài tập. Hãy dùng cách đang mở để chuẩn bị một ghi chú cho lúc ôn bài.” Cùng task cho cả A/B/C.

| Observation | Note thực tế |
|---|---|
| First action ở A, B, C | **A:** bấm “Lưu ghi chú” khi ô RAG đã có sẵn. **B:** bấm “Lưu cùng nguồn” khi ghi chú đã có sẵn. **C:** bấm “Tạo bản nháp AI”. |
| Chỗ dừng, do dự hoặc hiểu sai | **A:** cần điền điều nhớ hoặc điều còn thiếu mới lưu được; Minh không chắc lời giảng nên điền phần còn thiếu. **B:** hệ thống yêu cầu bấm “Gắn ghi chú vào Slide 12” dù nguồn đã hiển thị cạnh ghi chú; bước này dễ bỏ sót. **C:** đổi ghi chú đầu vào nhưng bản nháp vẫn y nguyên; xóa trắng bản nháp rồi vẫn lưu được. |
| Evidence/nguồn được đọc hay bỏ qua | **A:** Minh thấy Slide 12 ở cột bối cảnh, nhưng bản lưu không giữ nhãn nguồn. **B:** bản lưu ghi “Nguồn: Slide 12” và nội dung slide; Minh nhận ra đây chỉ là thẻ nội dung mẫu, chưa mở được slide gốc. **C:** ở bước duyệt, nhãn Slide 12 và cảnh báo giới hạn lời giảng rõ; bản cuối chỉ giữ văn bản, không giữ nhãn nguồn và trạng thái chưa chắc riêng. |
| Cách tester sửa hoặc lấy lại control | **A:** nút “Sửa ghi chú” đưa về các ô đã điền. **B:** nút “Xem lại nguồn / sửa ghi chú” mở phần nhập; có thể bỏ liên kết rồi gắn lại. **C:** có thể bỏ bản nháp, sửa bản đã lưu hoặc quay về ghi chú vội; khi bấm lưu trước khi xác nhận, trang yêu cầu đánh dấu đã xem lại nguồn. |
| Option được chọn | **B — Ghi chú gắn với nguồn.** |
| Lý do và trade-off | Minh muốn khi xem lại biết ý nào từ ghi chú vội và đối chiếu được với Slide 12; B giữ mối liên hệ này rõ nhất và vẫn có chỗ ghi điều slide chưa giải đáp. A giúp ghi trung thực điều chưa biết nhưng đòi người học tự khôi phục gần như toàn bộ ngữ cảnh. C viết nhanh nhưng bản nháp cố định không phản ứng với ghi chú đầu vào; công kiểm tra nội dung và nguồn khiến Minh chưa tin C hơn B. |
| Evidence chống lại kỳ vọng nhóm | **B:** nguồn hiện ngay cạnh ghi chú vẫn không khiến thao tác gắn nguồn trở nên hiển nhiên. **C:** bước xác nhận không ngăn được bản nháp không khớp input hoặc bản lưu rỗng; thông tin nguồn/độ bất định cũng mất ở màn cuối. |

## Tách bốn lớp

- **OBSERVED — đã thấy/nghe theo ghi chép được chuyển lại:** Minh thử lưu A/B ngay; cả hai hiện yêu cầu bổ sung trước khi lưu. Minh hoàn tất ba option và dùng được các đường sửa/bỏ. Minh thử thay input và xóa bản nháp ở C, phát hiện bản nháp không đổi và vẫn lưu được nội dung rỗng. Sau khi thử cả ba, Minh chọn B và nêu lý do là liên hệ giữa ghi chú vội và Slide 12 rõ nhất.
- **INTERPRETED — nhóm nghĩ điều đó có thể có nghĩa:** trạng thái nhập sẵn của A/B khiến Minh kỳ vọng có thể lưu ngay. Ở B, hiện nguồn không đồng nghĩa hành động gắn nguồn đã được hiểu. Ở C, bản nháp cố định có thể làm người học hiểu sai rằng hệ thống đã xử lý ghi chú đầu vào; màn kết quả thiếu nhãn nguồn làm mất dấu vết kiểm chứng.
- **DECIDED — NEXT CHANGE:** Trong riêng phiên Minh, chưa quyết định thắng/thua. Sau khi nhóm tổng hợp cả ba phiên, nhóm chọn giữ cơ chế bản nháp C và thêm nguồn theo từng câu kiểu B; người học giữ/sửa/bỏ từng câu, không lưu rỗng và vẫn thấy nguồn ở bản đã lưu. Xem [Group Feedback Synthesis](group-feedback-synthesis.md) để biết cơ sở của quyết định nhóm.
- **STILL UNPROVEN:** Riêng phiên này chưa cho biết người học có thực sự ôn/làm bài tốt hơn ngày hôm sau hay không; thẻ Slide 12 mẫu có đủ để thay slide gốc trong tình huống thật không. Dù đã có ba phiên, nhóm chưa xác thực giá trị sản phẩm.

Các quan sát trên được Đạt báo cáo từ phiên của Minh, tách khỏi phần diễn giải. Không đưa lượt tự kiểm tra kỹ thuật của AI vào Feedback Note này.
