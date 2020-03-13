# Virtualization
1. Khái niệm
- Là công nghệ dùng để ảo hóa server, storage, network,...
- Từ một máy vật lý có thể tạo ra các máy ảo có các hệ điều hành và service khác nhau.
- Đồng nghĩa với việc các máy ảo được chia tài nguyên từ các tài nguyên vật lý.
2. Vai trò
- Tận dụng được các tài nguyên dư thừa, chưa dùng tới.
- Chạy các ứng dụng và service riêng trên từng con ảo hóa, để dễ quản lý và không bị xung đột với nhau.
- Điều đó sẽ giúp máy chủ hoạt động nhanh hơn, tăng uptime cho tiến trình.
- Sử dụng ảo hóa để không phải đầu tư thêm nhiều các máy vật lý.
3. Phân loại
a,  Storage virtualization
  + Được tạo ra từ việc pooling các disk lại với nhau 
  + Nó sẽ điều hướng các request, các I/O request từ người dùng để đến vị trí lưu trữ thích hợp.
  + RAID là một kiểu của storage virtual, nó dùng để relicate dữ liệu, giúp hạn chế tối đa nhất việc mất dữ liệu.
### Có hai loại storage virtual cơ bản: File-based, Block-based
- File-based: là trường hợp sử dụng dành riêng cho network-attached systems (NAS), được khuyến khích sử dụng để cho phép
  nhiều người dùng và các thiết bị không đồng bộ.
  + Sử dụng hai giao thức System Message Block (SMB) và Network File System (NFS)
  + File-based phá vỡ sự phụ thuộc của mảng NAS thông thường giữa dữ liệu được truy cập và vị trí của bộ nhớ vật lý => điều
  này cho phép hệ thống NAS di chuyển và handle files tố hơn => improve hiệu năng.
- Block-based: được sử dụng rộng rãi hơn File-based
  + Cho phép phần mêm quản lý ảo hóa thu thập năng suất làm việc của khối hiệu năng, memory space sau đó gộp chúng vào trong
  shared resource để áp vào bất kỳ VMs or containers nào.
  + Để người dùng truy cập dữ liệu vào bộ nhớ vật lý, phần mềm ảo hóa cần phải tạo map, hoặc có thể sử dụng thuật toán để
  tự động xác định data.
b, Desktop virtualization
    + Là công nghệ cho phép người dùng mô phỏng một workstation để truy cập từ vị trí cục bộ hoặc remote đến một máy tính khác.
    + Việc tách môi trường desktop và application từ thiết bị vật lý người dùng được dùng để truy cập nó.
    + Là một key element của digital workstation và phụ thuộc vào application virtualization.
### Có hai loại desktop virtualization: Local desktop and remote desktop
- Local desktop: 
  + Oparation systems chạy trên thiết bị client sử dụng hardware virtualization.
  + Tất cả processing và workload đều được chạy trên local hardware
  + Sử dụng khi không cần đến sự tiếp diễn của netwwork 
  + Không thể sử dụng nó để chia sẻ đến các VMs khác, hoặc thông qua network để đến client khác hoặc mobile khác 
- Remote desktop: 
  + Được sử dụng rộng rãi hơn trong môi trường client/server
  + Cho phép người dùng vận hành hệ thống và ứng dụng inside data center.
  + Tất cả các tương tác của người dùng chỉ cần trên một thiết bị có kết nối internet.
c, Application virtualization
  + Cho phép người dùng truy cập và sử dụng application trên một máy tính đã được cài đặt application
  + Admin setup remote application trên server và deliver đến người dùng.
  + Việc trải nghiệm ứng dụng này như người dùng sử dụng ứng dụng trên máy tính vật lý.
  + Deploy app lên server thay vì phải thực hiện điều đó trên từng máy của người dùng.
  + Admin có thể chặn quyền truy cập của người dùng bất cứ lúc nào.
  + Người dùng có thể remove dễ dàng trên máy vật lý của mình.
d, Hardware virtualization
  + Là một khái niệm khá trừu tượng của tài nguyên máy tính từu việc dùng phần mềm để phân phát tài nguyên cho server.
  + Nó liên quan đến việc tạo một phần mềm máy ảo lên trên thành phần phần cứng của server =>Hyperviso
  + Khả dụng cho việc cùng tồn tại nhiều OS trên một hardware
### Có 3 loại hardware virtualization Full virtualization, Emulation virtualization, Para virtualization
  + Full virtualization: có cấu trúc mô phỏng khá đầy đủ, Guest software không cần chỉnh sửa bất cứ thứ gì để chạy ứng dụng
  + Emulation virtualization: nó mô phỏng phần cứng độc lập, Guest OS không được chỉnh sửa bất cứ thứ gì.
  + Para virtualization: nó không cần thiết được mô phỏng, nhưng nó tận dụng API để sửa đổi Guest software; 
  Guest software bị cô lập.
e, User virtualization
  + Đề cập đến việc quản lý độc lập tất cả các khía cạnh của người dùng trên môi trường desktop.
  + Là giải pháp cung cấp thích hợp và liền mạch qua một chuỗi môi trường làm việc của cơ chế phân phối nội dung.
  
  
  
  
  
  
  
  
