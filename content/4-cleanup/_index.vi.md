

---
title: "Dọn dẹp tài nguyên"
date: 2025-08-05
weight: 4
chapter: false
pre: "<b>4. </b>"
---


Chúng ta sẽ tiến hành các bước sau để xóa các tài nguyên chúng ta đã tạo trong bài thực hành này.



#### 1.  Xóa VPC và các tài nguyên liên quan
      1.1 Trước tiên hãy **Detach Internet Gateways**
  - Truy cập vào **VPC** ở thanh task bên trái chọn **Internet Gateways**
  - Tích chọn vào **Internet Gateways** đã tạo -> chọn **Actions** -> **Detach from VPC**
  - Chọn **Actions** -> **Delete Internet gateways**
      
      1.2 Xóa **Router Table**
  Vì đã xóa **Internet Gateways** trước đó nên vào Router Table để **Remove Internet Gateways** đã thêm trong mục **Edit Router** nếu không sẽ không xóa được **Router Table**
  - Chọn vào **Router Table** đã tạo -> **Action** -> Chọn **Edit Router** tìm tới mục có Target chứa **Internet Gateways** hãy **Remove** nó và bấm **Save Changes**
  - Vẫn chọn vào **Router Table** đã tạo -> **Action** -> Chọn **Edit subnet associations** bỏ chọn 2 subnet đã tạo -> Bấm **Save Changes**
  - Chọn **Router Table** đã tạo -> Chọn **Delete Route Table**
      
      1.3 Xóa **Subnet**
  Tích chọn vào 2 Subnet đã tạo -> Chọn **Actions** -> **Delete Subnet**
      
      1.4 Xóa **YourVPCs**
  Tích chọn VPC đã tạo -> Chọn **Actions** -> **Delete VPC**