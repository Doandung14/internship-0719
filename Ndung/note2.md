### Use ‘tac’, ‘sort’, ‘split’, ‘uniq’, ‘nl’

**tac command**

tương tự như cat command nhưng hiện thị ngược về trình tự nội dung

**sort command**

Dùng để sắp xếp văn bản: `sort [OPTION]... [FILE]..`

Sort hỗ trợ loại bỏ các text trùng lặp với optiopn uniq (Lệnh uniq dùng để bỏ các dòng liên tiếp trùng lặp trong một tệp văn bản rất hữu ích để đơn giản hóa hiển thị văn bản): `sort file1 file2 | uniq > file3`

**split command**

Lệnh split sử dụng để chia (hoặc tách) một tệp thành các phân đoạn có kích thước bằng nhau để xem và thao tác dễ dàng hơn và thường chỉ được sử dụng trên các tệp tương đối lớn. Theo mặc định, lệnh split tệp thành các phân đoạn 1000 dòng. Tệp gốc không thay đổi và một tập hợp các tệp mới có cùng tên cộng với tiền tố được thêm vào được tạo. Theo mặc định,tiền tố x được thêm vào. Để chia một tập tin thành các phân đoạn, sử dụng lệnh split infile.

syntax: `split infile <Tiền tố>`

**nl command**

Lệnh nl dùng để đánh số dòng trong 1 tệp: `nl [OPTION]... [FILE]...`

**head, tail command**

Xem nhanh 5 dòng đầu tiên với lệnh head:

syntax: `cat /etc/profile | head -n 5 > file1.txt`

Xem nhanh 5 dòng cuối với lệnh tail:

syntax: `cat /etc/profile | tail -n 5 > file1.txt`

**less command**

Xem nội dung file với lệnh less 

syntax: `less /etc/securetty`

Các phím thao tác trong khi mở file với less:

- SPACE BAR: để qua một trang khác

- ESC + V: để lùi lại một trang

- /<keyword> : để tìm kiếm theo từ khóa (case sensitive), nhấn n để di chuyển con trỏ đến kết quả tìm kiếm tiếp theo.

- g<line number>: để đi đến dòng mình muốn.

- q: để thoát khoi chương trình
