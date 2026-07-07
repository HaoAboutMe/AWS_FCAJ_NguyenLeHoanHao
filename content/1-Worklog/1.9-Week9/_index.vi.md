---
title: "Worklog Tuần 9"
date: 2026-07-04
weight: 9
chapter: false
pre: " <b> 1.9. </b> "
---

### Mục tiêu tuần 9:

* Cải tiến và tối ưu hóa giao diện trang web, phát triển thiết kế giao diện mới hoạt động mượt mà trên nhiều độ phân giải khác nhau.
* Triển khai lưu trữ tĩnh (Static Web Hosting) cho Frontend sử dụng Amazon S3 kết hợp với Amazon CloudFront làm CDN để tối ưu hóa tốc độ tải trang toàn cầu.
* Giải quyết triệt để lỗi khởi động lạnh (Cold Start) của dịch vụ AWS Lambda để cải thiện hiệu năng và giảm độ trễ phản hồi của hệ thống.
* Nghiên cứu, chuẩn hóa cấu trúc hệ thống và vẽ sơ đồ kiến trúc ứng dụng (AWS Architecture Diagram) chi tiết cho Cloud Battleship.

### Công việc thực hiện trong tuần:

| Ngày | Công việc | Ngày bắt đầu | Ngày hoàn thành |
| ---- | --------- | ------------ | --------------- |
| 2 | - Tái cấu trúc mã nguồn CSS và các thành phần giao diện, bắt đầu thiết kế giao diện web mới theo phong cách hiện đại <br> - Tối ưu hóa bố cục hiển thị thông tin trận đấu và khu vực chuẩn bị phòng chờ | 29/06/2026 | 29/06/2026 |
| 3 | - Tiếp tục hoàn thiện giao diện mới: tinh chỉnh các hiệu ứng hover, đổ bóng, và thiết kế kính mờ (glassmorphism) ở cả Light và Dark mode <br> - Sửa các lỗi lệch phần tử giao diện, căn chỉnh responsive của thanh menu điều khiển và nút chức năng trên di động | 30/06/2026 | 30/06/2026 |
| 4 | - Nghiên cứu cơ chế giảm độ trễ khởi động lạnh (Cold Start) của AWS Lambda <br> - Xây dựng Lambda Function điều phối (Warm-up Lambda) gửi tín hiệu heartbeat định kỳ đến các Lambda nghiệp vụ chính <br> - Thiết lập EventBridge Rules trong SAM template để tự động kích hoạt tiến trình warm-up mỗi 5 phút | 01/07/2026 | 01/07/2026 |
| 5 | - Triển khai hosting Frontend tĩnh trên Amazon S3 và cấu hình S3 Bucket Policies phù hợp <br> - Tạo và thiết lập Amazon CloudFront Distribution làm CDN phía trước S3, cấu hình Caching Policies và tích hợp chứng chỉ SSL cho kết nối bảo mật HTTPS <br> - Khắc phục các vấn đề liên quan đến cấu hình Redirect URI khi tích hợp Facebook Login với Amazon Cognito | 02/07/2026 | 02/07/2026 |
| 6 | - Nghiên cứu và xây dựng sơ đồ kiến trúc hệ thống (AWS Architecture Diagram) chi tiết hiển thị đầy đủ luồng dữ liệu REST API, WebSocket (APIGW), Lambda, DynamoDB và S3/CloudFront <br> - Thiết kế và hoàn thiện sơ đồ kiến trúc bằng định dạng Mermaid để tích hợp vào tài liệu dự án | 03/07/2026 | 03/07/2026 |
| 7 | - Tiến hành kiểm thử toàn diện hiệu năng hệ thống sau khi triển khai Warm-up Lambda và phân phối CDN CloudFront <br> - Hoàn thiện tài liệu kiến trúc kỹ thuật, sửa các lỗi giao diện tồn đọng và viết báo cáo tiến độ tuần 9 | 04/07/2026 | 04/07/2026 |

### Kết quả đạt được:

* **Nâng cấp và cải tiến giao diện người dùng (UI) đột phá:**
  * Thay đổi toàn diện giao diện sang phong cách hiện đại, cải thiện độ trực quan của bảng đấu và các ô hiển thị tàu tự vẽ.
  * Tối ưu hóa responsive toàn diện cho các thiết bị di động, loại bỏ hoàn toàn hiện tượng tràn chữ hay lệch nút bấm.

* **Deploy Frontend thành công lên AWS:**
  * Đưa ứng dụng Frontend lên Amazon S3 dưới dạng Static Web Hosting, giảm đáng kể chi phí vận hành.
  * Tích hợp Amazon CloudFront giúp phân phối nội dung tĩnh với tốc độ nhanh, tăng tính bảo mật nhờ kết nối HTTPS.

* **Khắc phục triệt để lỗi Cold Start Lambda:**
  * Giảm độ trễ phản hồi của API trong lần gọi đầu tiên từ vài giây xuống dưới 200ms nhờ cơ chế Warm-up tự động định kỳ bằng EventBridge.

* **Hoàn thiện sơ đồ kiến trúc AWS chuyên nghiệp:**
  * Thiết kế sơ đồ kiến trúc chi tiết giúp người ngoài dễ dàng hình dung toàn bộ luồng xử lý và mối liên kết giữa các dịch vụ serverless trong ứng dụng Cloud Battleship.
