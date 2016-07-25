#Nhóm lệnh liên quan đến bàn phím
##Bật-tắt touchpad bằng dòng lệnh trên terminal 
>sudo modprobe -r psmouse** *tắt*

>sudo modprobe psmouse** *bật
#Nhóm câu lệnh kiểm tra dung lượng
##2.1 Kiểm tra dung lượng ổ cứng mà các file hệ thống sử dụng
>df
##2.2 Hiển thị thông tin ổ đĩa các file hệ thống sử dụng
>df -a

>df -h
##2.4 Hiển thị 
>df -hT /home
##2.5 Hiển thị 
>df -k

#Nhóm lệnh cơ bản
* Tạo thư mục
>mkdir
 
*mkdir /tocxu-folder_name

* Xem thư mục hiện hành
>pwd

* Xem thông tin về thư mục và tập tin
>ls
>ls -l

liệt kê kích thước tập tin, người tạo ra, các quyền người sử dụng
>ls -a

hiển thị cả tập tin ẩn

* Di chuyển tập tin hoặc thư mục
>mv vi_tri1 vi_tri2

* Sao chép tập tin
>cp vi_tri1 vi_tri2

* Tìm kiếm 1 tập tin
>find

>file <path> -name <tên tập tin>

* Xóa thư mục rỗng
>rmdir

* Xóa tập tin và thư mục
>rm

>rm -fr /ten_file

xóa thư  mục hiện hành mà trong đó thư mục hiện hành có thể có thư mục con hoặc tập tin

* Hiển thị nội dung của tập tin
>more
>cat

* Nén và giải nén tập tin
>gzip
>gunzip

* Lệnh thêm một thiết bị
> mount <dev/ten_thiet_bi> <vi_tri_mount>
> umount

* Tạo người dùng
> useradd ten
> passwd ten

* Tạo nhóm
> groupadd ten_nhom

Thêm tài khoản vào nhóm
> usermod -g <tên_nhóm><tài_khoản>

* Lệnh tạo tập tin
> touch <đường_dẫn> <tập_tin>
> vim <path> <file>

#How to check an software is installed on ubuntu
> dpkg --get-selections | grep ten-goi

> dpkg --get-selectioins | grep mysql

#Clean

> echo "Cleaning Up" && 

> sudo apt-get -f install && 

> sudo apt-get autoremove && 

> sudo apt-get -y autoclean && 

> sudo apt-get -y clean
 


