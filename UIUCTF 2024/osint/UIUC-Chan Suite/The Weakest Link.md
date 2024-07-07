## The Weakest Link

<img width="444" alt="The Weakest Link" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/fe970813-29b8-4629-a82b-97422518c313">

## Solution:
Still applying the old formula to search for information on LinkedIn that I mentioned in the article [An Unlikely Partnership](/UIUCTF%202024/osint/UIUC-Chan%20Suite/An%20Unlikely%20Partnership.md) 

I found this person's Spotify link:

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/ae2f7f9a-7031-41e3-a98b-e2d6a22c104b" width="560">

On the Spotify profile, there is only one public playlist and this playlist doesn't have flag or any information either:

![spotify_account](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/0700df9a-de4e-4d4a-9139-b179b4fb425e)

I spent quite a lot of time on this challenge, trying to go back to the existing accounts to check thoroughly for any past archives 
or to find more information about `UIUC Chan` in the hope of finding another account *`X﹏X`*

<br>After a long time, I noticed a sudden increase in followers for this account, and as more people solved this challenge, I also followed suit. 
I found the flag in the ``Friend Activity section`` on the Spotify app:

<img width="700" alt="FLAG" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d33ee46c-88ef-442b-b63d-d90d5829ea54">

### Flag: ``uiuctf{7rU1Y_50N65_0F_7H3_5UMM3r_432013}``

## Postscript:
<br>I really appreciate the author's idea ＼（〇_ｏ）／
<br>After discovering it, you realized the author had left a hint about it on LinkedIn that you hadn't noticed. This shows how crucial a deep understanding of applications in OSINT can be:

<img width="589" alt="Screenshot 2024-07-02 020620" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9b211505-c8ca-498e-8b00-ef25ff76e1d4">


