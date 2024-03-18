## WOLPHV II: Infiltrate

<img width="321" alt="Description" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9db0740f-af5a-4ffc-8b36-12a0e9abf714">

## Solution:

Now what we need to do is to find another social media account of the WOLPHV group.

Starting with Facebook, and I found it quite easily:

<img width="1094" alt="search_fb" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/f6baf07f-1349-4c1c-a04c-a18ab3c0e708">

Accessing the group, I noticed that some posts are not very relevant. What caught my attention is a post with a video: 
https://www.facebook.com/groups/921721029413388/posts/921722342746590/

After watching the entire video and looking up at the browser tabs, I found a Discord invite link, but it's using the wrong domain: ``discord.com/UbeJPeBT``
<img width="998" alt="discord_link" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/e9f020cc-93bd-4f06-a641-da7254d7c20c">
We need to correct it to https://discord.gg/UbeJPeBT to make it valid. 

If you're new to Discord, they've also posted a helpful guide in the Facebook group.

<img width="577" alt="post_in_fb" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/e44d6857-b042-43f6-b00b-9f7e4a088536">

Access Discord, we will obtain the Flag:

<img width="1229" alt="flag" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/02e767f0-1166-40bb-ab5e-502f89642bda">

### Flag: ``wctf{r0t_52_w0ulD_b3_cr4zy_fRfr}``
