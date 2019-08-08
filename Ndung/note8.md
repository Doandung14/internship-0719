**mount & umount**

1.Mount là để truy cập một hệ thống tập tin trong Linux. Bạn có thể gắn hệ thống tập tin vào bất kỳ thư mục nào và truy cập nội dung bằng cách vào thư mục đó. Theo thuật ngữ Linux, các thư mục này được gọi là điểm gắn kết. Hướng dẫn này sẽ giúp bạn gắn kết và ngắt kết nối hệ thống tập tin trong hệ thống Linux.

- Sử dụng lệnh mount

Hầu hết, mỗi hệ điều hành Linux / Unix đều cung cấp lệnh mount. Lệnh này được sử dụng để gắn bất kỳ hệ thống tập tin trên bất kỳ thư mục. Sau đó, bạn có thể truy cập nội dung hệ thống tập tin.

 `mount [-t fstype] filesystem mountpoint`
 
 2.Sử dụng lệnh umount để ngắt kết nối mọi hệ thống tập tin được gắn trên hệ thống của bạn. Chạy lệnh umount với tên đĩa hoặc tên điểm gắn kết để ngắt kết nối đĩa hiện được gắn

vd: `umount /data`

**fdisk**

1.Xem tất cả phân vùng ổ đĩa trong linux

# fdisk -l

2. Xem phân vùng đĩa cụ thể trong Linux

# fdisk -l /dev/sda

3. Kiểm tra tất cả các lệnh fdisk có sẵn

[root@tecmint ~]# fdisk /dev/sda


4.In tất cả Bảng phân vùng trong Linux

`# fdisk /dev/sda`

5.Cách định dạng phân vùng trong Linux

[root@tecmint ~]# mkfs.ext4 /dev/sda4

6.Cách kiểm tra kích thước của phân vùng trong Linux

`# fdisk -s /dev/sda2`
