## WOLPHV V: luvh4ck573

<img width="313" alt="des" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/cb5152f9-4b09-4b73-a263-e62785d209d3">

## Solution:

Searching for this guy's name, I found his Tinder account: https://tinder.com/@luvh4ck573

<img width="900" alt="tinder_acc" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/494c14ef-bb79-4192-b3ab-c18716fd3825">

<br> Inside his photo, there's another hidden message: ``nathan-rizz-blog67945``

<img width="500" alt="tinder_img" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9d63a928-4c57-478c-8284-ca9b632135f5">

Looking at it I knew it was a username, but I didn't know which social media platform it belonged to. 
I felt very stuck, but then I tried a different approach to searching, and I found something interesting on YouTube:

<kbd><img width="430" alt="search_youtube" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/11ef9241-0a78-4075-84ac-23585b56287c"></kbd>
<kbd><img width="430" alt="search_ytb_2" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/7f7625a2-6879-4f91-a72d-c0b0b2acdf11"></kbd>

Reviewing this YouTube channel, there's only one video and no other useful information. Here is the link to the video: 
https://www.youtube.com/watch?v=ZEJdSXbglZs
<br>Checking the archive page, there's an archive from March 14, 2024, but unfortunately, I couldn't access it :sob:

<img width="900" alt="web archive" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/b5393472-e645-414f-929d-a16f376aa3e7">

<br>By a sudden thought, I searched the title of this video on Google hoping to find the account with the username ``nathan-rizz-blog67945``, and I also accidentally found an email address from the archive of the video on YouTube:
<img width="953" alt="gg_search" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/e628071e-9e6d-4798-8b67-08f62362036d">

Besides that, you can use Google Web Cache to view it using this link: 
https://webcache.googleusercontent.com/search?q=cache:https://www.youtube.com/watch?v=ZEJdSXbglZs

Even though it will lead you to the current YouTube page, you can still view the page's source to get the email:

<img width="900" alt="source" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/3c0d795d-7b92-48ff-bd01-68eba19d3d7b">

<br>I used https://tools.epieos.com/(Ghunt) to got this guy's real name behind email address:

<img width="651" alt="gg_account" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/e41170e1-01bb-4c96-9f57-4582bb7a26b1">
<br>I found this guy's Instagram account (same pfp as Google):
https://www.instagram.com/nathaniel_sterling2/
<img width="350" alt="ins_acc" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/f396c324-95cc-4206-a810-db2b8d9fbfb2">

So now we have two clues: one on Discord and one on Instagram

<kbd><img width="444" alt="clue1" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/34cd84c2-02e2-4bd1-b88d-7e00bd7a03cb"></kbd>
<kbd><img width="444" alt="clue2" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/bc5e28f6-fc6b-4a2b-81d0-356ae950cafb"></kbd>

Searching for "Subway" in Collingwood, Ontario, I found only 2 stores, and I found the one near "McDonald's":

<img width="1028" alt="subway_and_mcdonald" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/5fafbd1f-ab97-4cb7-bee1-ac9db2904e02">

There is still one missing data: ``nathan-rizz-blog67945``
Cuz I didn't have it so I guessed the result and accidentally found the right place is: ``King George Apartments``

<img width="838" alt="King_George_Apartments" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/36808fac-c2e8-4c71-aee7-16246d3515cc">

### Flag: ``wctf{44.499,-80.228}``

And here is what I was missing LOL

https://www.tumblr.com/nathan-rizz-blog67945/

<img width="421" alt="Screenshot 2024-03-19 015040" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/457efb0f-b436-4797-9442-c5219a401cf0">

<br>The clue to identify the house:

<img width="442" alt="clue3" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/52a9e417-49e5-437e-a846-30ff41dfd92e">

