# Install Ubuntu Desktop on VirtualBox

Ubuntu là HĐH mã nguồn mở miễn phí được xây dựng trên Debian GNU/Linux, tức là 
mọi người có thể tự do chỉnh sửa, thay đổi và cải tiến nó.

Ubuntu có 2 dòng sản phẩm chính
-	Ubuntu Desktop: Cài đặt trên máy tính cả nhân, phục vụ cho những người dùng thông thường.
-	Ubuntu Server: Cài đặt trên các máy chủ, phục vụ cho các doanh nghiệp.

Bài viết này mình sẽ hướng dẫn các bạn cài đặt Ubuntu Desktop dựa trên VirtualBox
 

## 1. Chuẩn bị
### 1.1. Download VirtualBox
Để Download VirtualBox bạn truy cập địa chỉ sau:
https://www.virtualbox.org/wiki/Downloads

Và tải phiên bản phù hợp với máy vật lý.

![download_virualbox](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_1.png)

Sau khi tải xong, tiến hành cài đặt.
### 1.2. Download Ubuntu Desktop 

Cũng như các hệ điều hành khác Ubuntu cũng có file ISO để bạn tải về.

Truy cập địa chỉ sau: https://www.ubuntu.com/download/desktop

Hiện tại phiên bản mới nhất là Ubuntu 18.04. Nếu bạn muốn tải các phiên bản cũ hơn 
thì click *** Alternative downloads *** và tải phiên bản mong muốn.

![download_ubuntu](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_2.png)

Không nên lựa chọn phiên bản Ubuntu beta vì nó còn đang phát triển và dễ xảy ra lỗi.
Nên chọn phiên bản ** Ubuntu LTS **. LTS là viết tắt của Long Term Support, 
có nghĩa là phiên bản đó sẽ được hỗ trợ lâu dài tận 5 năm. 
Vì vậy, bạn sẽ nhận được nhiều lợi ích như cập nhật lỗi bảo mật và các 
bản vá lỗi.

## 2. Tạo máy ảo Ubuntu

Đầu tiên, bạn cần tạo 1 máy ảo mới trên VirtualBox. Mở VirtualBox, nhấn **New** 
để tạo máy ảo mới. 

![img src](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_3.png)

Trong cửa sổ ** Name and Operating system**, đặt tên cho máy ảo ở mục **Name**(ví dụ Ubuntu), **Type** là Linux và **Version** ví dụ là Ubuntu (64-bit). 
Nhấn ** Next** để qua phần Memory Size.

![anh4](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_4.png)

VirtualBox khuyến nghị Ram tối thiểu là 1024MB . Bạn có thiết lập RAM phù hợp cho máy ảo của mình.
Nhấn **Next **

![anh5](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_5.png)


Trong phần **Hard disk**, chọn **Create a virtual hard disk now** và 
nhấn **Create** để tạo ổ đĩa ảo mới cho máy ảo Ubuntu.

![anh6](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_6.png)

**Hard disk file type**

Chọn **VDI** theo mặc định là tốt nhất. VDI là định dạng ổ đĩa ảo của VirtualBox,
 **VMDK** là định dạng ổ đĩa ảo của VMware và nó tương thích với hầu hết các 
 nền tảng ảo hóa. Tuy nhiên, bạn vẫn có thể chuyển định dạng VDI sang 
 VMDK bất cứ lúc nào. Nhấn **Next**
 
 ![anh7](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_7.png)
 
**Storage on physical hard disk**

Nên chọn **Dynamically allocated** thay vì **Fixed size**. 
Dynamically allocated  Tạo ta ổ đĩa ảo dùng đến đâu cấp phát bộ nhớ đến đấy.
  Nếu bạn chọn Fixed size thì dung lượng của file ổ đĩa ảo được tạo ra sẽ 
  cố định trên ổ cứng của bạn. Ví dụ bạn tạo ra ổ đĩa ảo Fixed size 20Gb thì
  ổ cứng của bạn sẽ mất 20Gb mặc dù máy ảo của bạn có sử dụng hết số đó hay 
  không. Dùng Dynamically allocated lợi thế hơn về mặt dung lượng nhưng  tốc độ ko 
  bằng fixed size tuy nhiên vẫn nên chọn vẫn chọn Dynamically allocated.
  
![anh8](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_8.png)

**File location and size**

Bạn cần thiết lập dung lượng ổ đĩa ảo phù hợp cho máy ảo của bạn. Nếu như 
bạn sử dụng Dynamically allocated thì phần này thiết lập dung lượng cao lên 
một chút cũng không sao cả.

Nhấn **Create** để kết thúc quá trình tạo máy ảo Ubuntu trên VirtualBox.

![anh9](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_9.png)

Chọn **Setting** để thiết lập 1 số cài đặt cho HĐH

![anh10](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_10.png)

![anh11](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_11.png)

![anh12](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_12.png)


Nhấp chuột vào “CD/DVD icon" (biểu tượng CD/DVD) có dấu "+" và chọn ISO để cài đặt.

Chọn file ISO bạn đã tải về trước đó.

![anh13](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_13.png)

![anh14](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_14.png)


Chọn máy ảo. Ấn nút **Start** để khởi động

Tiếp theo bạn có 2 lựa chọn:
- Try Ubuntu Dùng thử Ubuntu, bạn có thể sử dụng Ubuntu ngay lập tức mà không cần cài đặt.
- Install Ubuntu Cài đặt Ubuntu

Ở đây mình sẽ cài đặt Ubuntu mà không cần dùng thử, chọn ngôn ngữ sử dụng English 

Nhấn **Install Ubuntu**.


![anh15](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_15.png)

Chọn vị trí (thiết lập múi giờ)

![anh16](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_16.png)

Chọn kiểu bàn phím.

![anh17](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_17.png)

Phần tiếp theo rất quan trọng bạn cần tạo 1 account để đăng nhập.
 Trong cửa sổ **Who are you?** Nhập đầy đủ các thông tin
 
 Nhấn **Continue**. Và chờ Ubuntu cài đặt
![anh19](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_19.png)

Sau khi cài xong, bạn sẽ nhận được thông báo trên màn hình. 
Ấn **Restart Now** để khởi động lại

![anh20](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_20.png)

Sau khi máy ảo khởi động, bạn cần đăng nhập vào account bằng mật khẩu đã tạo trong quá trình cài đặt trước đó.

![anh21](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_21.png)

Đây là màn hình Ubuntu khi mới cài đặt:

![anh22](https://github.com/chinguyen97/Install-Ubuntu-on-VirtualBox/blob/master/images/Screenshot_22.png)

Vậy là bạn đã hoàn thành việc cài đặt Ubuntu trên máy ảo VirtualBox.

Để sử dụng full màn hình VirtualBox, copy paste hoặc copy file trong 
VirtualBox, bạn cần phải cài đặt **Guest dditions** trên máy ảo Ubuntu 
trong Virtualbox

Chúc các bạn thành công!

### Tài liệu tham khảo: https://tutorials.ubuntu.com/tutorial/tutorial-install-ubuntu-desktop#7

