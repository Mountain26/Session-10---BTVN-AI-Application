## Bài 1. Phân Tích & Lựa Chọn Chiến Lược Tài Liệu Hóa

### Đáp án chọn

- Phương án B

### Lý do chọn

- Antigravity có lợi thế khi cần đọc xuyên suốt nhiều file trong một workspace lớn.
- Bài toán checkout flow nằm rải ở Controller, Service, Repository và JWT Security Filter, nên cần giữ ngữ cảnh liên kết giữa các lớp thay vì đọc từng đoạn rời rạc.
- Prompt ở phương án B yêu cầu AI đóng vai System Analyst và xuất ra SRS theo cấu trúc rõ ràng, nên đầu ra gần mục tiêu tài liệu hóa hơn.
- Cơ chế index toàn bộ thư mục giúp giảm thất thoát ngữ cảnh khi logic nghiệp vụ được điều khiển qua nhiều điểm vào.
- Cách này phù hợp với bài học Session 10 vì trọng tâm là dùng AI để đọc hệ thống thật rồi tái cấu trúc thành đặc tả, không phải chỉ giải thích từng đoạn code.

### Lý do loại trừ phương án A

- Chỉ làm việc trên từng đoạn code được bôi đen nên ngữ cảnh bị cắt nhỏ.
- Logic checkout flow liên kết nhiều lớp, nên Copilot Chat dễ trả lời đúng cục bộ nhưng sai toàn cục.
- Người dùng vẫn phải tự ghép các mảnh giải thích thành SRS, dẫn tới tăng rủi ro thiếu bước, thiếu ngoại lệ và thiếu ràng buộc nghiệp vụ.
- Đây là kiểu hỗ trợ đọc code, không phải kiểu tổng hợp tài liệu hệ thống ở mức end to end.

### Lý do loại trừ phương án C

- Copy thủ công 5 file vào chat web làm ngữ cảnh dễ đứt, nhất là khi file dài hoặc có nhiều phụ thuộc.
- Không có workspace index nên AI khó truy lần liên kết giữa endpoint, service, repository và filter.
- Cách này phụ thuộc nhiều vào việc người dùng chọn đúng file và dán đủ nội dung, nên rủi ro thiếu dữ liệu đầu vào cao.
- Khi cần sửa hoặc mở rộng đặc tả sau đó, luồng làm việc rất khó lặp lại và kiểm chứng.

### Kết luận

- Phương án B là lựa chọn tối ưu vì phù hợp nhất với bài toán tài liệu hóa hệ thống lớn, giữ được ngữ cảnh liên lớp và tạo đầu ra gần chuẩn SRS nhất.
