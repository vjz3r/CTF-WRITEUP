# Challenge Description:
<img width="499" alt="Screenshot 2024-12-23 214246" src="https://github.com/user-attachments/assets/3c1076d1-a531-4e33-9cc4-7825ffcb9cee" />

# Solution:
Tìm kiếm tên "Xylya Noreena" ở các nền tảng mạng xã hội thì mình đã tìm thấy tài khoản ở Twitter:
![image](https://github.com/user-attachments/assets/071a0195-1ede-4d20-a325-51cfbc396394)
<br> Ở đây cũng không có gì, chỉ có 2 thông tin là:<br>
- Username: ``X_n0r33n4``
- Ngày tháng năm sinh: ``December 25, 2000``
<br> Dùng username thì mình tìm thêm được 2 tài khoản mới:
<img width="1266" alt="image" src="https://github.com/user-attachments/assets/1c606140-6967-495c-8267-150660b1a121" />

Ở Instagram thì không có gì hết cả còn ở Threads có 1 bức ảnh chụp chứa thông tin về tài khoản Telegram:

<img width="505" alt="image" src="https://github.com/user-attachments/assets/98cfa282-4280-4c7b-8a5b-373fd25e117f" />

Mình chỉ nhìn thấy được: "Xylya_", khi mình tìm kiếm ở trên Telegram thì không có kết quả chính xác, quay lại với bức ảnh thì mình thấy ảnh nền là bộ phim Mr.Robot nên mình lại nghĩ tới "BOT"(không biết đây có phải là chủ ý của tác giả hay không hehe)
nên mình tìm kiếm "Xylya_bot" và đã có được kết quả đúng 🥳
<br>
Nhắn tin cho bot thì không thấy phản hồi lại nên mình lại mày mò về những gì có sẵn ở Telegram và vô tình bấm vào phần ``Bot Privacy Policy``:
<img width="1280" alt="image" src="https://github.com/user-attachments/assets/49824fb4-4802-46c9-a990-6922471ca8d6" />
Sau khi bấm vào thì sẽ được chuyển đến 1 kênh tên là 1337Signal, kéo lên 1 chút có 1 file zip và ở đó có chứa 1 nửa của flag theo đường dẫn: ``StealerLog_25-11-2024.zip\1337.1337.1337.1\Accounts\credencial``
![image](https://github.com/user-attachments/assets/ee59a533-ba54-4035-acaa-f104c7b5ae46)

### FLAG_PART1: ``MSEC{m3rRy_cH1s``
Tiếp tục đi tìm phần còn lại của flag :>
Ở trong Telegram còn 1 file zip nữa có nhắc tới 1 người là "luk45"
![image](https://github.com/user-attachments/assets/031fa76f-57a8-4faa-be91-050dc3300340)

Theo đường dẫn: ``Stealog_26-11-2024.zip\235.756.234.1\Accounts\credencial`` thì mình đã thấy tài khoản mà mật khẩu của anh ta:

![image](https://github.com/user-attachments/assets/7cd7a62b-d0e6-4777-a740-66dc6478f0f4)

Nhưng mình không biết nó dùng để làm gì nên tạm bỏ qua.
Trong Threads còn 1 bài viết có đề cập tới 1 bí mật nào đó:
![image](https://github.com/user-attachments/assets/a9e17c5a-8c18-41e9-809b-bb43cbe0bfa0)

Mình có để ý tới những emoji ở dưới phần bình luận nên nghĩ đó là 1 dạng mã hoá gì đó, mình đã tốn khá nhiều thời gian để tìm kiếm cách giải mã nó và may mắn là mình đã tìm ra được đúng công cụ để giải mã:
<img width="641" alt="image" src="https://github.com/user-attachments/assets/e4289ed2-b5f0-46ac-8f05-91cdabcaaa4b" />
<br>Truy cập vào link Pastebin thì thấy file cần phải có mật khẩu để mở khoá:
![image](https://github.com/user-attachments/assets/f8fe82d6-5568-464f-9a36-10d8d7a77dc8)

Mình đã sử dụng mật khẩu ban nãy tìm thấy của ``luk45`` trong Telegram để mở khoá nhưng nó không đúng.
Có 2 dữ kiện về mật khẩu của anh chàng này:
![image](https://github.com/user-attachments/assets/9ba0982e-42bc-47ac-aa74-f7d3d82ae71b)

--> Mật khẩu của anh ta đã bị thay đổi. ``lukasim1337@signal.com:SIGNALluk4512072001`` có vẻ như anh ta cũng là 1 thành viên của hội nhóm này.

Mình đoán mật khẩu mặc định có dạng: SIGNAL + username + DOB cho nên mình đã thử đổi thành:<br>
``SIGNALX_n0r33n425122000`` (Giải thích 1 chút ở đây là: Username + DOB mình đều lấy được ở Twitter)

<br>Và........ BINGO!!!

![image](https://github.com/user-attachments/assets/21b5379b-a09b-46e7-a678-abae328f20c9)

### FLAG: ```MSEC{m3rRy_cH1sm4s_0r_merry_chrismas!!!}```

# Postscript:
Bài Writeup của mình tới đây là kết thúc, hy vọng các bạn sẽ học được thêm điều gì đó từ bài viết này.

### Thanks for reading!!!
