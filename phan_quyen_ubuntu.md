#1. Quản lý người dùng (user)
Trong Linux có 3 dạng đối tượng:
* User: là tài khoản người dùng - người dùng có thể truy cập tới hệ thống

Có hai loại user:
<li> root: toàn quyền trên hệ thống</li>
<li> regular user: người dùng bình thường ( user1, user2 ..)

Mỗi người dùng có mã định danh riêng là UID. UID của người dùng bình thường bắt đầu từ 500.
* Group: nhóm người dừng

Mỗi người dùng là một thành viên của 1 group. Khi tạo user thì mặc định tạo ra group. Mã định danh riêng của group là GID.
* Other: tất cả người dùng khác trên hệ thống
#2. Phân quyền 
##2.1 Đối tượng:
* Owner (người sở hữu)
* Group owner (Nhóm sở hữu)
* Other users (những người khác).

Các Quyền:
* Read -r --4: cho phép đọc nội dung
* Write -w --2: dùng để tạo, thay đổi hoặc xóa
* Execute -x --1: thực thi chương trình.

##2.2 Cấp quyền cho file và directory
>chmod [quyền] [tên file, thư mục]

VD: *chmod 755* /tocxu.txt

Trong đó, 7 là toàn quyền cho  Owner= 4+2+1: rwx =được phép đọc, thay đổi, sửa xóa và thực thi file/thư mục

Số 5 đầu tiên là quyền dành cho Group owner = 4+0+1: r-x =được phép đọc và thực thi nhưng không thể thay đổi file/thư mục

Số 5 cuối cùng là dành cho Other users , ý nghĩa quyền tương tự như trên.

Ngoài ra, trong lệnh **chmod** còn có thể có thểm các tùy chọn sau:
* -v : hiển thị báo cáo sau khi chạy lệnh. Nếu bạn chmod nhiều file/folder cùng một lúc thì sau mỗi lần đổi quyền cho một file/folder xong sẽ hiện báo cáo
* -c : giống như trên nhưng chỉ hiện khi nó đã làm xong tất cả
* -f : không thông báo dù có lỗi xảy ra
* -R : nếu chmod một folder thì các file/folder con cũng  chịu ảnh hưởng của quyền
* -help : hiển thị thông báo trợ giúp

##2.3 Thay đổi chủ sở hữu file/folser
Mặc định các file và folder sẽ thuộc sở hữu của người tạo ra nó. Để đổi chủ sở hữu sử dụng lệnh :
>chown -R [tên user]:[tên group] [file/folder]




