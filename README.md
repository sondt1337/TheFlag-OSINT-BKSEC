
# Writeup: The Flag (OSINT)
**Given file**: [Message](/Problem/Message.zip)

**Category**: Osint

**Author**: Spid3r

### Phân tích
Trong file message có nhắc đến 1 đối tượng là **Penda Luke**  có 2 điều cần phải lưu ý:
- Nghĩ đến việc osint người 
- Tìm kiếm trên các nền tảng mạng xã hội là điều đầu tiền cần làm

Thử tìm kiếm trên Facebook, Instagram, Twitter thì thấy có được duy nhất 1 tài khoản là có ích trong việc điều tra (Hầu hết các tài khoản khác tìm được đều là 1 clone nào đó) `@pendar9912`

![](https://i.imgur.com/gdsYL7y.png)

Đọc qua các tweet của người này 1 lượt (2 bài viết), thì thấy là không thể khai thác được gì từ cái ảnh ở sân bay (check metadata, ... tuỳ các bạn)

Có lẽ thứ có thể dùng được trong bài này đấy là bài viết về những món ăn tại Việt Nam

![](https://i.imgur.com/CVggALz.png)

Đến đây có 2 cách để làm (thực ra bài này mình thêm thông tin trực tiếp vào từng ảnh để dễ hơn, cách 2 đấy chính là ngồi bấm mấy cái ALT kia rùi tự nhận ra thui :}}}}) 

Cách 1: Nhìn đoạn `Foｏd ｉn Vｉetnam iｓ dｅlｉcious` trông có vẻ rất khả nghi, có lẽ là giấu 1 cái gì đó trong này, thử search **how to see hide message in twitter** thì thấy có 1 link như chúng ta cẩn [How to hide secret messages in your Twitter updates
](https://www.engadget.com/2014-05-09-twitter-steganography.html)

![](https://i.imgur.com/4hWzMDL.png)

--> thứ mình cần quan tâm là banh mi (món bánh mì trong bài post của Penda Luke)

![](https://i.imgur.com/sCFXgpN.png)

Trong post về bánh mì có chứa 1 cái tên là Daisy, thử tìm mối liên hệ của Daisy với Penda Luke

Thử tìm trong mục Following và Follower thì thấy có 1 tài khoản chứa cái tên này `@GeorgeDaisy11`

![](https://i.imgur.com/tG98lOo.png)

account này cũng chỉ đăng 2 tweet:

![](https://i.imgur.com/Nc5aarJ.png)

Thông qua kiểm tra thì thấy ảnh đầu không chứa gì lạ cả (Giống như  tweet của Penda Luke)

Để ý bài post mới nhất: Daisy than thở về việc lỡ xoá nhầm những tấm ánh về Việt Nam và không biết cách để tìm lại chúng --> thấy có 1 comment

![](https://i.imgur.com/g4X5Nlc.png)

Điều này lại đưa chúng ta đến với 1 account mới :))) @Daisygonnaplay --> nghe có vẻ liên quan đến Daisy, chắc crush giúp đỡ :))

![](https://i.imgur.com/MNjNLCH.png)

Có vẻ đúng là thứ mà Daisy cần đây rồi, check 1 bài viết duy nhất của tài khoản Timer_Timer

![](https://i.imgur.com/g5F6AAD.png)

Sau khi bấm vào link thì chuyển hướng tới notebin và muốn đọc được chúng thì cần phải có mật khẩu. Đọc lại tweet đó thì có *I think it will be helpful for you, passwd are the characters you used to have before you lost them.* Tức là password của link notebin này chính là những ký tự mà Daisy đã làm mất

Điều mình có đến hiện tại chỉ là account của Daisy, nên có lẽ muốn xem Daisy đã từng mất gì thì chỉ có thể trông chờ vào nền tảng twitter này thôi. Thử search **how to see a tweet that was deleted** thì tìm được [How to Find Deleted Tweets on Twitter](https://youtu.be/dsDpkKJxBt8)

![](https://i.imgur.com/efd6w84.png)

--> Sẽ dùng đến [Waybach Machine](https://web.archive.org/) để tìm những twitter có thể đã bị xoá của Daisy

Thấy có 2 bản snapshot (Trong đó có 1 bản snapshot cũ hơn là Daisy chưa xoá tweet)

![](https://i.imgur.com/f3KSXCk.png)

![](https://i.imgur.com/M0vvhd1.png)

Truy cập vào link thì thấy rằng drive này bị hỏng 

![](https://i.imgur.com/he4XuET.png)

Có lẽ do việc Daisy xoá nhầm tuy nhiên Timer_Timer đã có 1 cách để lấy lại chúng 

Bây giờ thì quay trở lại việc tìm password cho cái link notebin kia. 

--> Sử dụng những ký tự mà Daisy đã làm mất chính là mật khẩu :)))) đến đây thì 100% là dùng cái link hỏng kia chính là pass

password: `https://drive.google.com/drive/folders/1KKCg2A5Ks9eeRBer8Y_4LFfsbk-ZHgy2?usp=sharing`

Lại mở ra 1 cái link khác :)))) (Haizz tự chê Spid3r ra đề khó nha)

![](https://i.imgur.com/v0xRqs6.png)

https://mega.nz/folder/SF5kDRiC#wFEdtZS1MH10_CFaWfejRA

![](https://i.imgur.com/tpmyX9X.jpg)

Đến đây có lẽ việc tìm flag phải nhờ đến các bạn vậy (95% quá trình rùi)
*Nhớ là để ý đến đoạn tin nhắn ban đầu để tìm lá cờ nhé (Chưa chắc đã giòn đâu)*

###  flag: **BKSEC{HoangSaTruongSaVN}**
