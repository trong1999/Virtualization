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
4, Phân loại CPU virtualization
  + <img src="https://cdn.educba.com/academy/wp-content/uploads/2020/01/Types-of-CPU-Virtualization-1.jpg">
  ### Software-Based CPU Virtualization
  + mã ứng dụng sẽ thực thi trên bộ xử lý
  + Mã chương trình hoặc mã ứng dụng được dựa trên các thành phần của mã đặc quyền để gọi đến hệ thống, nó sẽ chạy với tốc độ chậm trong môi trường ảo.
  ### Hardware-Assisted CPU Virtualization
  + Là phần cứng hỗ trợ CPU virtual từ những bộ xử lý nhất định 
  + Guest code sẽ chạy trên guest mode.
  + Được sử dụng để hỗ trợ phần cứng, do đó, hệ thống sẽ chạy nhanh hơn mong đợi.
  ### Virtualization and Processor-Specific Behavior
  + Chế độ xử lý khác nhau dựa trên CPU vsự đa dạng của các tính năng mà nó cung cấp trong khi các ứng dụng tạo đầu ra thường sử dụng các tính năng đó.
  ### Performance Implications of CPU Virtualization
  + Các ứng dụng như vậy yêu cầu sử dụng ảo hóa CPU để nhận lệnh hoặc thực thi cần thiết để được thực thi trước => làm mất thời gian xử lý chung, giảm hiệu xuất.
  
  
