---
title : "tạo IAM Role"
date: 2025-08-05
weight : 1 
chapter : false
pre : " <b> 2.1 </b> "
---
### Tạo IAM Role

Trong bước này chúng ta sẽ tiến hành tạo IAM Role.

1. Truy cập vào [giao diện quản trị dịch vụ IAM](https://console.aws.amazon.com/iamv2/)  
![role](/images/2.prerequisite/001-iam.png)

Ở thanh task bên trái chọn User
![role](/images/2.prerequisite/002-iam.png)
Sau đó bấm chọn Create User

![role](/images/2.prerequisite/003-iam.png)

Tiến hành đặt tên và tích chọn vào Provide user access to the AWS Management Console Bạn có thể chọn tự tạo mật khẩu hoặc để AWS tự tạo cho bạn sau đó bấm **Next** Bạn sẽ được đưa tới giao diện setpermissions Chọn các lựa chọn như trong ảnh 

- **AdministratorAccess**

sau đó bấm **Next**
![role](/images/2.prerequisite/004-iam.png)
Xem và kiểm tra kỹ các lựa chọn

Sau khi thành công mà hình sẽ hiển thị như sau:

có thể chọn tải Download .csv file để lưu lại tài khoản
Sau đó copy link ở phần **Console sign-in URL**
![role](/images/2.prerequisite/005-iam.png)

Sau đó tiến hành đăng nhập vào account được cung cấp và tiến hành đổi mật khẩu
![role](/images/2.prerequisite/006-iam.png)

Sau khi đăng nhập thành công sẽ hiện thị ra như sau
![role](/images/2.prerequisite/007-iam.png)
và tiến hành thực hiện các bước tiếp theo