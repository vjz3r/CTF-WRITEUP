### WOLPHV I: Reconnaissance

<img width="320" alt="Screenshot 2024-03-18 111523" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/2da2d5f3-be5c-42d9-9c91-3675b182c639">

### Solution

As the title, flags found on the web are all fake flags. But I'll list them here anyway :v

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/c0a348a1-b0c1-4c84-84a1-f5026c9dfd42" width="250">
<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d7d5f000-2363-4a84-9c92-85e4ee4bb07a" width="390">
<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/ad7e662d-50d9-45af-bda5-1b7d729d29a4" width="360">


Skip that and start searching for what we have on the website.

Searching by the group name and the group logo doesn't seem very useful:

![search_byname_and_logo](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/4f43b279-e54d-4377-9d34-8e6726634e5b)

Hmmm reading the information in the "About Us" section also provides a lot of useful information here. I tried searching for it on Google and found an article about this group:

![Search_by_aboutus](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/c2b71b7e-57ca-42cc-b94e-f3c37f118d6d)
https://thecyberexpress.com/new-wolphv-ransomware-group-on-the-dark-web

Accessing the article, we immediately have the Twitter account name of this group: ``wolphvgroup``.
At first, I didn't pay much attention to it because in the title, there was a note:

``NOTE: Wolphv's Twitter/X account and https://wolphv.chal.wolvsec.org/ are out of scope for all these challenges. Any flags found from these are not a part of these challenges`` 

So I thought it might just have fake flags like on the website.

After about 3 hours of searching for more articles about this group and finding nothing 😅 And my friend found the flag in the comments section of this post :Đ

https://twitter.com/FalconFeedsio/status/1706989111414849989

Here is the Flag:
![flag](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d6a11cb7-b5c5-4fc9-a37e-4626513a3e9a)
``wctf{0k_1_d0nT_th1Nk_A1_w1ll_r3Pl4c3_Us_f0R_4_l0ng_t1me}``
