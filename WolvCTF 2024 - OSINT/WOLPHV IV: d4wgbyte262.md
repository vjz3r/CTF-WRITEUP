## WOLPHV IV: d4wgbyte262

<img width="318" alt="des" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/86f1a8c0-f606-46b7-9048-a5c113a01367">

<br>Contine with the conversations in Discord:

<img width="800" alt="conversation" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/5415263d-9fe9-474c-bdda-edb6fec50994">
  
 <br>Author has left a helpful clue: the messenger of "d4wgbyte262" in Discord: ``she's good! been taking a lot of flicks of her when i visit my neighbors and uploading them online``
 
They're talking about `flicks` and uploading pictures online, which reminds me of a famous photo-sharing website: https://www.flickr.com/
Searching for "d4wgbyte262" on Flickr, I found this account: https://www.flickr.com/photos/200261418@N03
<br>Accessing the account, can see that there are a lot of dog pictures here:

<img width="900" alt="flickrs" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9c7857ae-b0d3-493b-950c-81eaa33ae8da">

Randomly clicking on a photo, then clicking on the map section will reveal the location where the photo was taken, as well as all the photos uploaded by that person on Flickr:

<img width="900" alt="random_pic" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/05b26d7e-f4ff-4cf7-a19e-16a912085656">

We have another hint message in Discord:
<img width="748" alt="clue" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/129a44b7-711b-48dc-93d5-9091a68a656c">

Now, just need to search for a fire station near the WhiteHorn area on Google Maps:

<img width="1154" alt="check" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9764ffa0-b3a3-495d-861c-0acba6c464f5">

<br>Afterward, cross-reference it with the location where the photo was taken on Flickr to determine the precise location of the house.

<img width="1085" alt="right_place" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/070f00e2-5ad0-46f9-9863-73a152af06a4">

<br>And got the flag:

### Flag: ``wctf{51.0911, -113.9561}``
