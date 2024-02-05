# Challenge Description:
Theo thông tin từ trinh sát thành phố Hà Nội, cô gái tên Kagami là Việt Kiều Nhật, đã bị bắt cóc trong lúc đi bộ tại công viên, cảnh sát điều tra trong điện thoại cô gái có một tệp tin khả nghi nhưng đã bị khóa, đóng vai một điều tra viên bạn hãy điều tra và tìm ra hung thủ.

Format: MSEC{}

Author: h1n4m

[diary.zip](https://github.com/vjz3r/CTF-WRITEUP/files/14168656/diary.zip)

<img width="363" alt="Screenshot 2024-02-05 232425" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/92282d67-0003-447e-a001-c67a35c92d76">

# Solution:

Đề cho ta một file zip cần mật khẩu để giải nén, mình đã thử crack nhưng không được, chắc là do mình gà TvT Vậy hướng đi sẽ là tìm thông tin về `Kagami` chắc chắn sẽ có password ở đâu đó. Ban đầu mình đã nghĩ sẽ dễ dàng tìm ra tài khoản của người dùng này trên mxh nhưng không :)) Mình đã mất khá nhiều thời gian để có thể tìm thấy nó và tất cả là do Facebook ***

Đây là tài khoản của người cần osint:
https://www.facebook.com/k4g4m11

<img width="1277" alt="Screenshot 2024-02-05 231344" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/05e9b0b5-36e1-4b0c-a783-b283411e4791">

Truy cập vào trang cá nhân thì mình thấy có một bài viết author có để lại comment về cách đặt mật khẩu nên mình nghĩ mật khẩu sẽ liên quan đến địa điểm trong hình:

<img width="568" alt="Screenshot 2024-02-05 234141" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/5d4e673a-1cf5-4908-a73d-736cd90109b7">

Sử dụng Lens để tìm kiếm thì có ngay kết quả là ``Công Viên Lênin``

<img width="1244" alt="Screenshot 2024-02-05 234434" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/f38e7a64-0c97-4dd7-a66f-d6d4dd5a4193">

Mình đã nghĩ là người này sẽ để lại đánh giá địa điểm này kèm với mật khẩu trên google maps nhưng không có nên mình đã nhập thử tên của địa điểm vào thì vô tình lại giải nén được file LOL
Vậy password là: ``congvienlenin``

Sau khi giải nén mình có được file `diary.docx` mình đã đem file này đi scan kiếm Macros và nhận lại cái nịt (´。＿。｀)

Mở file ra đọc thì ngoài những nhật ký thường ngày thì mình còn thấy được có một đoạn chữ bị ẩn đi nhưng vẫn bị mình phát hiện do author viết tiếng việt nên Word nó gạch chân là chữ sai :}}}

<img width="1280" alt="Screenshot 2024-02-05 235134" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/0b68e119-6369-45b5-a626-60439f2a2f57">

Ctrl + A rồi copy hết mọi thứ bỏ sang Notepad thì sẽ đọc được nội dung bị thiếu. Việc cần làm bây giờ là phải liên hệ với bạn thân của cô ấy vì anh ấy đang nắm giữ chìa khoá:

<img width="727" alt="Screenshot 2024-02-05 235405" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/70af64bf-8044-4e8a-be33-87ef6428857a">

Quay lại Facebook thì có thể thấy rõ ràng bạn thân của cô ấy là author :Đ

<img width="524" alt="Screenshot 2024-02-05 235803" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/dd397b44-a953-42e2-9ec3-766c36379146">

Nhắn tin cho fanpage đó thì sẽ nhận lại được một dường link google drive:

<img width="245" alt="Screenshot 2024-02-06 000058" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/645e3472-4863-4e0e-86f1-37050746a331">

Truy cập vào đường link sẽ có được 1 file`flag.dat`, mở file ra mình thấy nội dung bên trong toàn là kí tự hex nên đem đi giải mã và thu được một file png:

<img width="1027" alt="Screenshot 2024-02-06 000437" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/963ed769-0214-4ad1-9c76-d13b8301dba0">

🤯🤯🤯🤯 ta đã có được flag: **MSEC{thU_pH4m_l4_cHu_kiM}**

# Postscript:
Bài Writeup của mình tới đây là kết thúc, hy vọng các bạn sẽ học được thêm điều gì đó từ bài viết này.

### Thanks for reading!!!
