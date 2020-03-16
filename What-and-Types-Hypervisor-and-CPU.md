1, Khái niệm
  - Là phần mềm quản lý ảo hóa, nó dùng để tạo VMs và chia sẻ tài nguyên máy tính.
  - Dùng để quản lý memory, CPU, storage của của máy vật lý lẫn VMs
  - Nó có tên gọi khác là Virtual Machine Monitor (VMM)
2, Phân loại : có hai loại Native và Hosted
<img src="https://thegioimaychu.vn/blog/wp-content/uploads/2018/10/400px-Hyperviseur.png">

**a, Native:**
  + Chạy trức tiếp trên hardware của Host để quản lý Guest OS
  + Sử dụng cho các doanh nghiệp lớn, data center

**b, Hosted:**
  + Chạy trên một OS thông thường như software layer hoặc application
  + Sử dụng cho người dùng cá nhân, doanh nghiệp bé.

3, CPU virtualization
  + Nó hoạt động như thể có nhiều CPU riêng biệt
  + Dùng để chạy nhiều OS trên một máy.
  + CPU này có thể được cấu hình tĩnh hoặc động, khi mà nó không dùng đến thì nó server khác sẽ được sử dụng, và ngược lại nếu nó cần nhiều tài nguyên cho tiến trình thì nó sẽ được lấy thêm.
