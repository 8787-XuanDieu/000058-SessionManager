---
title : "Kết nối Peering"
date: 2025-08-05
weight : 1 
chapter : false
pre : " <b> 3.1 </b> "
---
### Tạo kết nối Peering

Ở Bước này, bạn sẽ tạo kết nối **VPC Peering (VPC Peering Connection)**.
- **WebApp ↔ Hub**
- **Management ↔ Hub**
- **Hub ↔ Database**
**VPC Peering** cho phép các tài nguyên trong hai **VPC** khác nhau giao tiếp với nhau như thể chúng đang nằm trong cùng một mạng.
1. Đăng nhập vào AWS Management Console
- Tìm VPC
- Chọn VPC  

![role](/images/3.connect/001-vpc.png)

2. Trong giao diện VPC
- Chọn Peering Connections
- Chọn Create Peering Connection

![role](/images/3.connect/002-vpc.png)

3. Trong giao diện Create Peering Connection
- Nhập Name **Hub-to-WebApp**
- Chọn **VPC ID (Requester)** Hub-vpc
- Chọn **My account**
- Chọn **This Region (us-east-1)**
- Chọn **VPC ID (Accepter)** Web-App-vpc
- Chọn **Creat peering connection**

![role](/images/3.connect/004-vpc.png)

4. Accept request cho Peering Connection

- Chọn **Actions**
- Chọn **Accept request**

![role](/images/3.connect/005-vpc.png)

5. Tiếp tục lập lại các bước trên với **Hub-to-Management**

![role](/images/3.connect/006-vpc.png)

- Chọn **Actions**
- Chọn **Accept request**

6. Tiếp tục tạo Peering Cross-region giữa Hub và Database.
Lấy ID Database-vpc
- Chuyển sang region Oregon (us-west-2)
- Chọn **Your VPC**
- Copy **VPC ID Database-vpc**

![role](/images/3.connect/007-vpc.png)

Tạo Peering Cross-region.
- Quay về N. Virginia (us-east-1)
- Chọn Peering Connections
- Chọn Create Peering Connection

![role](/images/3.connect/008-vpc.png)
- Nhập Name **Hub-to-Database-CrossRegion**
- Chọn **VPC ID (Requester)** Hub-vpc
- Chọn **My account**
- Chọn **Another Region**
- Chọn **Oregon (us-west-2)**
- Dán **VPC ID Database-vpc đã copy từ Oregon (us-west-2)**
- Chọn **Creat peering connection**

![role](/images/3.connect/009-vpc.png)

Accept request cho Hub-to-Database-CrossRegion.
- Chuyển sang region Oregon (us-west-2)
- Chọn **Actions**
- Chọn **Accept request**

![role](/images/3.connect/010-vpc.png)

7. Kiểm tra kết quả.
- Quay về N. Virginia (us-east-1), sẽ thấy 3 Peering Connection được tạo.

![role](/images/3.connect/011-vpc.png)