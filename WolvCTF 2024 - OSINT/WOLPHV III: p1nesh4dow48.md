## WOLPHV III: p1nesh4dow48

<img width="300" alt="Description" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/962e8941-9014-4485-85b4-146c0135346e">

## Solution:

In Discord, we have the following conversation:

<img width="500" alt="conversation" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/b3a28c42-b791-4d93-b79b-2d0baa7070d0">

<br>So, to find p1nesh4dow48's house, we'll need to pinpoint the location of the building in this image:

<img width="9000" alt="location" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/62520830-69e7-4680-b1c0-e630013b5d25">

<br>When searching for images using Google Lens, I found quite a few buildings similar to that one, but they are not what we are looking for. I also didn't get any promising results when searching with Yandex and Bing.

<img width="500" alt="gglens" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/44793ce1-cc75-4c81-81f9-a4b0c3e163de">
<img width="500" alt="yandex" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/260fb6e5-bd7e-4c9b-a6eb-1cafcb62c837">

<br>Upon analyzing the contents of the image, I noticed a signboard with the following text:``PINE RIDGE VISITOR PARKING ONLY``
<br>Okay, start searching for ``Pine Ridge Apartments`` on Google Maps, and I received a lot of results:

<img width="900" alt="gg_maps" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/b232e95e-b2b2-4630-8ad2-e35f6aadadd0">

<br>But we have a valuable clue in the challenge: [``WOLPHV I: Reconnaissance``](/WolvCTF%202024%20-%20OSINT/WOLPHV%20I%3A%20Reconnaissance.md), which is the leader of this group in Michigan. So I narrowed down the search area to Michigan:

<img width="1000" alt="pine-ridge-michigan" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/70a16f5d-63c0-4353-bfd5-b7cc18ce5c54">

<br>Luckily, I skipped over many apartments in the center, I noticed the only apartment located at the top of Michigan named ``Pine-Ridge Apartments`` 
When I accessed it and browsed with Google Street View andddd BINGO!!! I found the right place:

<img width="1000" alt="right_place" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/dacc2987-22f2-427c-a4dd-4a2f924d92d8">

<br>B/c only the last three digits after the comma need to be determined, it's quite easy to get the flag:

### Flag: ``wctf{46.546,-87.388}``
