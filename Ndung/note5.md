**awk command**

AWK là một ngôn ngữ lập trình. Nó có thể xử lý các tác vụ liên quan đến text phức tạp chỉ với một vài dòng code. AWK là một ngôn ngữ lập trình thông dịch. Nó được thiết kế đặc biệt và mạnh mẽ cho việc xử lý text. Nó được ứng dụng để xử lý text với các file .txt, .csv với kích thước lên tới GB, các thao tác như đọc file, ghi chép theo dòng, cột,.. một cách nhanh chóng. AWK có thể sử dụng một shell scripting trong Ubuntu, có thể chạy dưới định dạng .sh

syntax: `awk [options] file ...`

Ví dụ muốn in ra cột 3 và cột 4 của file ta sử dụng lệnh sau:

`awk '{print $3 "\t" $4}' marks.txt`

- Sử dụng biến

Với awk, bạn có thể xử lý tệp văn bản. Awk gán một số biến cho từng trường dữ liệu được tìm thấy:

$ 0 cho toàn bộ dòng.

$ 1 cho trường đầu tiên.

$ 2 cho trường thứ hai.

$ n cho trường thứ n.

ARGC     Retrieves the number of passed parameters.(lấy các tham số đã truyền)

ARGV     Retrieves the command line parameters.( lấy tham số các dòng lệnh)

ENVIRON     Array of the shell environment variables and corresponding values.(Mảng của các biến môi trường shell và các giá trị tương ứng.)

FILENAME    The file name that is processed by awk

NF     Fields count of the line being processed.( Các lĩnh vực đếm của dòng đang được xử lý)

NR    Retrieves total count of processed records.(Lấy tổng số hồ sơ được xử lý.)

FNR     The record which is processed.(bản ghi đc xử lí)

IGNORECASE     To ignore the character case.

- Formatted Printing

c              Prints numeric output as a string.

d             Prints an integer value.

e             Prints scientific numbers.

f               Prints float values.

o             Prints an octal value.

s             Prints a text string.
