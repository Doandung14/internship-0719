**du command**

Lệnh du (Sử dụng đĩa) là một lệnh Unix / Linux tiêu chuẩn, được sử dụng để kiểm tra thông tin sử dụng đĩa của các tệp và thư mục trên máy. Lệnh du có nhiều tùy chọn tham số có thể được sử dụng để nhận kết quả ở nhiều định dạng. Lệnh du cũng hiển thị các tệp và kích thước thư mục.

-Option 

- Sử dụng tùy chọn -h của lệnh du để hiển thị thông tin người đọc có thể dễ dàng đọc được Có nghĩa là bạn có thể thấy kích thước tính theo Byte, Kilobytes, Megabyte, Gigabyte, v.v.

- Sử dụng -A với lệnh du hiển thị việc sử dụng đĩa của tất cả các tệp và thư mục.

- Sử dụng -ah hiển thị mức độ sử dụng đĩa của tất cả các tệp và thư mục ở định dạng dễ đọc của con người. Đầu ra dưới đây dễ hiểu hơn vì nó hiển thị các tệp trong Kilobytes, Megabyte, v.v.

- Find out the disk usage of a directory tree with its subtress in Kilobyte blcoks. Use the “-k” (displays size in 1024 bytes units).

- Để có được bản tóm tắt về việc sử dụng đĩa của cây thư mục cùng với các cây con chỉ bằng Megabyte (MB). Sử dụng tùy chọn -mh . -m đếm các khối theo đơn vị MB và -h là viết tắt của định dạng con người có thể đọc được

- Hiển thị mức sử dụng đĩa dựa trên việc sửa đổi thời gian, sử dụng -time

**df command**

lệnh df trên linux sẽ giúp báo cáo về dung lượng đang sử dụng của các phân vùng ổ cứng, bên cạnh đó có thể xem được cả loại file system của partion hoặc disk với option -T
cú pháp : `df [OPTION]... [FILE]...`

1.Check File System Disk Space Usage:`df`

2.Display Information of all File System Disk Space Usage:`df -a`

3.Show Disk Space Usage in Human Readable Format:`df -h`

4.Display Information of /home File System:`df -hT /home`

5.Display Information of File System in Bytes:`df -k`

6.Display Information of File System in MB:`df -m`

7.Display File System Inodes:`df -i`

8.Display File System Type:`df -T`

9.Include Certain File System Type:`df -x ext3`
