# Challenge Description:
🌲🌲🌲Theo truyền thống, mỗi khi đến mùa lễ giáng sinh, những đứa trẻ trên toàn thế giới sẽ viết thư cho ông già Noel để chia sẻ những câu chuyện, thành tích trong năm vừa qua, đồng thời bày tỏ những ao ước, khao khát của bản thân.
☃☃☃Và tất nhiên, những đứa trẻ ngoan của KCSC cũng không phải ngoại lệ. Hàng chục bức thư tâm huyết từ KCSC-ers đã được viết và gửi đi. Nhưng thật không may, Elf - người chịu trách nhiệm gửi thư lại bị bắt cóc, một bức thư đe dọa khác được gửi tới ông già Noel. 
😱😱😱KCSC kêu gọi các bạn tìm cách giải cứu Elf, lấy lại thông điệp giúp chúng mình. Nội dung thư đe dọa như video bên dưới. KCSC sẽ treo thưởng cho những bạn tìm ra flag đầu tiên.

<img width="600" alt="Screenshot 2023-12-25 024132" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/63a96cb6-cf5b-48b3-b724-5a5b0e780cb6">

# Solution:
Trước tiên nhìn vào ảnh ta có thể thấy có 1 đoạn mã hexa: ``4e 67 61 6e 48 61 6e 53 6f 31 44 69 61 50 68 75`` và khi decode ra ta sẽ được 1 đoạn văn bản: ``NganHangSo1DiaPhu``, chưa biết dùng để làm gì nên tạm gác nó sang 1 bên.

<img width="400" alt="Screenshot 2023-12-25 024808" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/ba5c342e-ce0c-4933-9186-3a49e1d4229c">

Ở dưới bức thư còn để lại chữ ký của "Siêu tướng cướp" cũng như là đối tượng ta cần tìm hiểu đó là: ``Nova Serenade``.
- Như truyền thống hằng năm của KCSC thì sẽ luôn bắt đầu từ Facebook nên mình tìm kiếm ở Facebook đầu tiên và tìm ra được tài khoản này có vẻ khả nghi: https://www.facebook.com/profile.php?id=61553251516260
  * Lướt qua một vòng thì ở đây cũng chỉ có một vài gợi ý chưa dùng tới :/
- Tiếp theo tìm kiếm cái tên ở Twitter bạn sẽ thấy tài khoản này: https://twitter.com/n0v4_s3r3n4d3
   * Okay bỏ qua các tweet thử thách của năm ngoái thì ta sẽ thấy 1 bài đăng mới, đó là địa điểm ta cần tìm:

<img width="448" alt="Screenshot 2023-12-25 030258" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/fd43f421-d3c3-4613-8e26-cf72e8768654">
  
Import ảnh vào Google Lens và chọn đúng vị trí thì ta sẽ có luôn kết quả chính xác:

<img width="1279" alt="Screenshot 2023-12-25 030541" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/8f63cc26-83c2-4920-8276-be8a5d1e88bc">

Đó chính là `Trung Tâm Hội Nghị Văn Hoá Tỉnh Lai Châu` và đối diện là `Quảng Trường Lai Châu`

<img width="1271" alt="Screenshot 2023-12-25 031359" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/aa34d142-2386-4161-9180-9be447ed9499">

Tên bắt cóc này có đăng lên ở Twitter là đi đến đây để tận hưởng kỳ nghỉ ở ``Luxury Hotel`` nên mình đã tìm kiếm trên Google và có được kết quả:

<img width="965" alt="Screenshot 2023-12-25 032110" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/b08ff936-a0af-4f16-bd48-f4779eb984c1">

Tìm ``Khách sạn Hoàng Nhâm Lai Châu`` trên Google Maps -> Chọn vào phần *Đánh giá* sẽ thấy đánh giá của người dùng tên là **Moderator Discord** kèm lời nhắn:

<img width="1069" alt="Screenshot 2023-12-25 032255" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/4d7667e3-ac5d-4712-a3e5-7bb53fb05815">

Liên hệ với người dùng này qua Gmail: ``thedoubleneevec@gmail.com`` sẽ có một email tự động trả lời lại:

<img width="575" alt="Screenshot 2023-12-25 032716" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/f71eabcf-fc4a-48f0-af17-5e8bce7b3caa">

- Email này cung cấp một đường link chưa hoàn thiện: ``https://**********/9Ugx4Ysjpc``
  * Ban đầu mình tưởng đây là link https://pastebin.com có chứa flag và kết thúc thử thách nhưng nó lại không đúng 😓. Nhìn lại thấy tên của người dùng là ``Moderator Discord`` nên mình đoán đây là link Invite vào server Discord, thay đoạn ********** thành ``discord.gg`` and Bingo!: https://discord.gg/9Ugx4Ysjpc.

<img width="449" alt="Screenshot 2023-12-25 033755" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/327025b9-7eb0-434f-8d4e-b6bbeec78f24">

- Truy cập vào Server ta thấy có 3 kênh và 2 kênh chứa nội dung.

  * Kênh buôn-flag có ``free flag giải D*ctf: Flag{1m_w4rl0ck_wr**th_n07_a_K1dn4pp3r_nor_a_Ch4ll_Th13f}``, mình thắc mắc giải D*ctf là giải gì mà sao có ăn trộm với ăn cắp ở đây nhỉ? 🤡 Ngoài free flag của giải CTF ~~ă̵n̵ ̵t̵r̵ộ̵m̵ ~ thì còn có một đường link file Mega: https://mega.nz/file/g2dyQCKC#5iiEMObr9OVCf3IUeeLmPGfA3Ki3jAv6GnXhErTk2tM cùng với một cái bánh trông cũng ngon.

<img width="1034" alt="Screenshot 2023-12-25 034527" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/13bfccb0-25b1-407f-a477-3828a723185a">

  * Kênh buôn-elf thì đề cập tới người dùng có tên ``Elf cầm flag``, xem ở phần giới thiệu ta sẽ có một nửa flag được encode base64: `S0NTQ3sxdCdzX24wN19XaEA3JzVfdU5kM3JfNw==` -> Decode:  `KCSC{1t's_n07_Wh@7'5_uNd3r_7`

<img width="1058" alt="Screenshot 2023-12-25 034620" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/16346494-393d-4f53-ae8d-aafe0e2750ed">

Tải file Mega về cần mật khẩu để giải nén, còn đoạn văn bản: ``NganHangSo1DiaPhu`` từ đầu chưa dùng đến mình nghĩ đó là mật khẩu nên nhập thử. Thật bất ngờ nó không đúng :))

Quay trở lại Facebook, mình thấy có một bài viết tên này nói đến việc hắn sử dụng một tool ở Github:

<img width="515" alt="Screenshot 2023-12-25 040634" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d51b1620-52f9-4181-91db-4e626751a21e">

nên mình đã lấy username ở Twittter để tìm kiếm trên Github. Kết quả là tìm được tài khoản này: https://github.com/S3r3n4d3theDiscordMod.

Có 4 Repo, 3 cái là của người khác hắn lưu về tài khoản còn 1 cái là hắn tự tạo:

<img width="1254" alt="Screenshot 2023-12-25 041756" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/fd9b9789-5d46-4b24-8af6-2d7d1f148589">

Bên trong repo ``Tool-For-Saved-Thing`` có một file Markdown ghi một đường link:

<img width="789" alt="Screenshot 2023-12-25 042059" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/434ac32e-efd6-44f4-aaab-983dbbb555fc">

Đây là link của một trang web dùng để "Lưu trữ một trang web". Sau nhiều lần thử với các đường link khác nhau thì cuối cùng mình cũng đã tìm thấy bản lưu trữ chứa cách để tìm được mật khẩu:

<img width="1250" alt="Screenshot 2023-12-25 041510" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/57a9cce3-b018-4ca4-9445-cf53a7e2dbfb">

-> Tỉnh từng đến là tỉnh "Lai Châu" nên mật khẩu để giải nén sẽ là **laichau**

Giải nén ra sẽ có được nửa còn lại của Flag: ``h3_TR33_tH4t_m4773r5,_1t'5_wh0'$_g4th3r3d_4r0und_1T}``

<img width="671" alt="Screenshot 2023-12-25 042651" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/aff01e13-4575-471b-9137-3fd3fa539a43">

Ghép 2 nửa lại sẽ có FLAG: **KCSC{1t's_n07_Wh@7'5_uNd3r_7h3_TR33_tH4t_m4773r5,_1t'5_wh0'$_g4th3r3d_4r0und_1T}**

# Postscript:
Bài Writeup của mình tới đây là kết thúc, hy vọng các bạn sẽ học được thêm điều gì đó từ bài viết này.

### Thanks for reading!!!
