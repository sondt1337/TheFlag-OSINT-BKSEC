# Writeup-_-MISC_BKsec

Tải 2 file First_layer.exe và Second_layer.exe về thì ta có thể thấy không thể mở được bình thường, check file kỹ hơn thì ta thấy thực ra ban đâu First_layer là file zip và Second_layer là file Rar (file này có 1 đoạn mô tả nhỏ có thể liên quan đến 1 link google drive)

![image](https://user-images.githubusercontent.com/87920408/218775422-7df37a9d-4da5-4809-a78b-d5bdf8c4b00e.png)

![Screenshot_20230214_100158](https://user-images.githubusercontent.com/87920408/218776027-dd505f4e-9f7f-4531-ae57-25d017150461.png)

Sau khi để các file về đúng dạng của nó thì 2 file này đều bị khoá, điều cần làm bây giờ là crack được file First_layer vì trong file này có chứa `P@55W0RD.jpg` (có thể là pass giải khoá file Rar) và chính sự khác biệt giữa Zip và Rar này nên chúng ta có thể dùng tới 1 tool để bruteforce passwd là [John The Ripper](https://github.com/piyushcse29/john-the-ripper) hoặc sử dụng trực tiếp `zip2john` trong kali linux 


