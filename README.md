# Track 1 — Day 19: Multiple Prototype Experiment

## 1. Thông tin cá nhân và đội ngũ

- **Người nộp:** Phạm Quốc Đạt — 2A202602384
- **Nhóm:** DBH
- **Thành viên:** Phạm Quốc Đạt (2A202602384), Nguyễn Văn Biển (2A202602416), Mai Tiến Huy (2A202602914)
- **Case:** B — AI Notes: Personal Learning Notes
- **Sản phẩm nhóm:** [Three-option Design Sheet](three-option-design-sheet.md), [ba micro-prototype HTML](prototype-link.md) và [Group Feedback Synthesis](group-feedback-synthesis.md)

## 2. Hypothesis Problem

Khi một buổi học có nhiều khái niệm được trình bày nhanh, người học muốn giữ đủ phần giải thích để xem lại nhưng không ghi kịp; ghi chú chỉ còn từ khóa hoặc thiếu ngữ cảnh, khiến họ không chắc mình hiểu đúng và phải tìm hiểu lại sau buổi học.

Nhóm tiếp tục Pain Hypothesis A từ Day 17. Practice interview do Đạt thực hiện cho thấy một người học chỉ ghi được đề mục/từ khóa trong buổi học liên quan RAG vì giảng và trả lời nhanh; sau đó không chắc phần mình nhớ có đúng hay không. Practice Note của Biển không ghi nhận cùng khó khăn; notes của Huy chỉ có bản tóm tắt, không có ghi chép gốc để đối chiếu. Vì vậy đây vẫn là **giả thuyết**, không phải vấn đề đã được xác thực cho mọi người học. Xem bảng evidence và điều chưa biết trong [Design Sheet](three-option-design-sheet.md).

## 3. Three Solution Options

| Option | Cơ chế chính | Prototype |
|---|---|---|
| A — Ghi chú theo khung | Người học tự tách điều nhớ, phần còn thiếu và việc cần kiểm tra. | [Mở A](prototypes/option-a.html) |
| B — Ghi chú gắn với nguồn | Người học gắn ghi chú vội vào Slide 12 để giữ đường đối chiếu. | [Mở B](prototypes/option-b.html) |
| C — Bản nháp AI có kiểm chứng | Hệ thống đưa bản nháp mô phỏng; người học xem nguồn, sửa/bỏ và quyết định lưu. | [Mở C](prototypes/option-c.html) |

Ba option giữ cùng user, tình huống, task, ghi chú vội, nội dung Slide 12 và phong cách giao diện; khác ở cơ chế tương tác và phần việc của người học/hệ thống. Option C dùng văn bản cố định để mô phỏng AI, không gọi mô hình thật. Chi tiết cách mở và giới hạn liên kết nằm trong [Prototype Link](prototype-link.md).

## 4. Đóng góp cụ thể của tôi trong sản phẩm nhóm

- **Option phụ trách chính:** A — Ghi chú theo khung.
- Cung cấp Practice Note Day 17 về tình huống ghi chú khi học RAG; tham gia chọn tiếp tục Pain Hypothesis A làm điểm xuất phát cho ba option.
- Cùng chuẩn bị bối cảnh chung RAG/Slide 12, ba prototype HTML và phần so sánh Human–AI trong Design Sheet với sự hỗ trợ của AI. Tôi đã mở được cả ba prototype và báo lỗi bản HTML đầu tiên hiển thị trắng để AI tạo lại bản tự chứa.
- **Facilitation:** trực tiếp điều phối Ninh Quang Minh thử cả A/B/C, ghi lại thao tác, điểm vướng và lý do Minh chọn B. [Feedback Note cá nhân](prototype-feedback-note.md) tách nội dung quan sát được báo cáo khỏi diễn giải và quyết định tiếp theo.
- Cung cấp [bản tổng hợp ba phiên](group-feedback-synthesis.md) của nhóm, trong đó có kết quả hai phiên do Biển và Huy điều phối; nhóm chốt một Next Change dựa trên hành vi và trade-off, không chỉ đếm phiếu chọn.

## 5. Dữ liệu kiểm thử và bài học

- [Feedback Note của phiên tôi điều phối](prototype-feedback-note.md): Minh thử A→B→C và chọn B. Minh thấy B giữ nguồn rõ nhất; ở C, bản nháp không phản ứng với input đã đổi, có thể lưu rỗng và bản lưu không giữ nhãn nguồn riêng.
- [Group Feedback Synthesis](group-feedback-synthesis.md): theo bản tổng hợp nhóm, Vũ chọn C và An chọn C, nhưng cả ba tester đều cần nhìn rõ nguồn để quyết định tin nội dung nào. Hai bản Feedback Note cá nhân của Biển và Huy cần nằm trong repo cá nhân tương ứng để đối chiếu.
- **Next Change nhóm chốt:** giữ cơ chế AI đưa bản nháp của C, thêm nguồn theo từng câu kiểu B và cho người học giữ/sửa/bỏ từng câu; ngăn lưu rỗng, giữ nhãn nguồn ở bản lưu. Cần sửa bản nháp mô phỏng để nó phản ánh input hoặc nêu rõ giới hạn khi test vòng sau.
- **Still Unproven:** người học có tự đọc nguồn khi học một mình và vội không; ghi chú có giúp làm bài hôm sau tốt hơn không; kết quả có lặp với người mới học RAG và với nhiều slide không. Ba lượt test chưa xác thực giá trị sản phẩm.

## 6. AI Support Log

AI được dùng để rà tài liệu Day 17/Lab 19, gợi ý và viết Design Sheet, tạo prototype HTML, chuyển ghi chép test do nhóm cung cấp thành file theo mẫu và rà format repo. Tôi đã kiểm tra trực tiếp ba HTML mở được, phát hiện và báo lỗi bản cũ hiển thị trắng; dữ liệu của Minh và bản tổng hợp hai phiên còn lại do con người cung cấp. AI không tham dự các buổi test. Chi tiết điểm AI sai/hời hợt và việc cần đối chiếu nằm trong [AI Support Log](ai-support-log.md).

### Ghi chú trước khi nộp

Sáu file Markdown theo mẫu nằm ở thư mục gốc; ba HTML nằm trong `prototypes/`. Các liên kết HTML tương đối mở được sau khi tải hoặc clone repo. Repo GitHub người nộp và thư mục nộp đều dùng đúng tên Day19. Sau khi tải file lên, bật GitHub Pages và kiểm tra ba URL công khai theo [Prototype Link](prototype-link.md). Đã ghi ngày test và tiêu chí sàng lọc của Minh theo thông tin tôi cung cấp; hình thức gặp chưa được nêu.

