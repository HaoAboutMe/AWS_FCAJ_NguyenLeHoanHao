---

title: "Worklog Tuần 3"
date: 2026-05-24
weight: 3
chapter: false
pre: " <b> 1.3. </b> "
----------------------


### Mục tiêu tuần 3:

* Tìm hiểu AWS Backup và cơ chế backup/restore trên AWS.
* Tìm hiểu quá trình migrate Virtual Machine từ môi trường On-premises lên AWS.
* Thực hành import/export Virtual Machine và triển khai EC2 Instance từ AMI.

### Các công việc cần triển khai trong tuần này:

| Thứ | Công việc                                                                                                                                          | Ngày bắt đầu | Ngày hoàn thành | Nguồn tài liệu                                                           |
| --- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ------------ | --------------- | ------------------------------------------------------------------------ |
| 2   | - Tìm hiểu S3 Bucket nâng cao <br> - Tìm hiểu cơ chế quản lý object và storage trên Amazon S3                                                      | 18/05/2026   | 18/05/2026      | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 3   | - Tìm hiểu AWS Backup <br>  + Backup Vault <br>  + Backup Plan <br>  + Recovery Point <br> - Thực hành Backup EC2 Instance                         | 19/05/2026 | 19/05/2026 | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 4   | - Thực hành Restore EC2 Instance từ Recovery Point <br> - Tìm hiểu quy trình restore và kiểm tra trạng thái Backup Job/Restore Job                 | 20/05/2026 | 20/05/2026 | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 5   | - Tìm hiểu VMware Workstation <br> - Tìm hiểu mô hình On-premises và Virtual Machine <br> - Chuẩn bị môi trường Virtual Machine để migrate lên AWS | 21/05/2026 | 21/05/2026 | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 6   | - Tìm hiểu Export Virtual Machine from On-premises <br> - Upload Virtual Machine lên AWS <br> - Tìm hiểu Import Virtual Machine lên AWS            | 22/05/2026 | 22/05/2026 | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |
| 7   | - Tìm hiểu triển khai EC2 Instance từ AMI <br> - Tìm hiểu quy trình tạo và sử dụng AMI <br> - Theo dõi các nội dung tiếp theo từ video 137 - 149   | 23/05/2026 | 23/05/2026 | https://www.youtube.com/playlist?list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i |

### Kết quả đạt được tuần 3:

* Hiểu được các tính năng nâng cao của Amazon S3 và cách quản lý dữ liệu trên Object Storage.

* Tìm hiểu AWS Backup và các thành phần chính:

  * Backup Vault
  * Backup Plan
  * Recovery Point
  * Backup Job
  * Restore Job

* Thực hành thành công:

  * Backup EC2 Instance
  * Kiểm tra Recovery Point
  * Restore EC2 Instance từ backup

* Hiểu được quy trình backup và restore tài nguyên trên AWS.

* Tìm hiểu mô hình Virtual Machine trong môi trường On-premises bằng VMware Workstation.

* Hiểu được quy trình migrate Virtual Machine từ On-premises lên AWS:

  * Export Virtual Machine
  * Upload Virtual Machine
  * Import Virtual Machine
  * Deploy Instance từ AMI

* Tìm hiểu cách hoạt động của Amazon Machine Image (AMI) và cách triển khai EC2 Instance từ AMI có sẵn.

* Thực hành xử lý một số lỗi thường gặp:

  * Backup Job trạng thái
  * Restore Job
  * Bucket Policy
  * CloudFormation delete stack
  * EC2 instance dependency
  * ...

* Không thực hiện các video từ 120 - 137 do các bài lab yêu cầu nâng cấp tài khoản và phát sinh thêm chi phí.

* Đã hoàn thành theo dõi và học các video từ 103 - 120 và 137 - 149 trong series First Cloud Journey Bootcamp 2025 của AWS Study Group.
