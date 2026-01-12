# PHP-Object-Injection
# Magic method
#### __construct() tự động khởi tạo object
#### __destruct() gọi khi object bị hủy 
#### __unserialize() chuyển hóa dữ liệu dạng mã hóa về trạng thái cũ 
#### __serialize() chuyển hóa dữ liệu về dạng mã hóa
#### __toString() ép kiểu chuỗi thành String 
#### so sánh == sẽ ép kiểu theo mức độ ưu tiên để so sánh còn nếu dùng === thì sẽ so sánh hai bên với nhau
#### PHP đối xử với object như 1 hàm __toString() 
#### untrustedata rơi vào hàm unserialize vbaf ngược lại
#### ........
#### Hàm băm không thể truy suất ngược lại (md5)
#### require = include (read and excute)
# Cách tìm
#### Tìm theo các magic method được gọi rồi try vấn xem có làm gì được tiếp không
#### Tìm theo các hàm nguy hiểm (vd: system, eval, readfile,....) rồi truy ngược lại xem có gọi được đến dòng code đó không
#### Cách tìm function -> (vd: "close(" )
