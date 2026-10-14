# -CNTT2-_-NhapMonCNTT-_Session08_Ex03

phần 1:

pipeline powershell dùng dấu | để nối các lệnh: gc đọc tệp, select-string lọc từ khóa timeout, where-object loại dòng not timeout, cuối cùng Measure-Object đếm kết quả. khác với cmd/bash truyền văn bản, powershell truyền các object có cấu trúc, giúp xử lý dữ liệu thuận tiện hơn

phần 2:

(Select-String ".\file.txt" "TIMEOUT" | Where-Object { $_.Line -notmatch "NOT TIMEOUT" }).Count
