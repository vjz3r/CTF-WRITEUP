## Night
<img width="442" alt="Screenshot 2024-07-02 021102" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/279fe866-19b8-405e-9997-c4d86d10b9aa">

[`⬇️chal.jpg`](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/3b747132-f368-4781-8eb4-55015080f30d)

## Solution:
Surely, everyone knows about [Google Lens](https://lens.google.com) by now. It is becoming more powerful and very useful for solving Geoint challenges.
<br>I will also start using Google Lens to solve this challenge.
<br>The results will vary depending on the region you choose to search. I pinpointed the exact city where this photo was taken by selecting the region around the prominent high-rise buildings in the background: -> `Boston`

<img width="800" alt="Boston" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/5057404d-a601-4d6f-920a-78981c464602">

There was even a photo quite close to the location we needed to find in the bottom right corner of the screen. However, that post did not have the exact address of the location:
https://twitter.com/berkie1/status/1731142295888502987
<br>Continuing to search by selecting the region, this time I focused on the building near the railway tracks. And I got the answer for the flag from this search:
https://twitter.com/CoStarNews/status/1806380226173129032
<img width="800" alt="CIM_office" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/5ff766e9-50cc-4b45-aff6-720f1cdd8b02">
<br>Accessing the article, I will got the address of this building: -> `95 Berkeley St.`

<img width="800" alt="95 Berkeley St" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/ae634080-80b9-4034-aefb-0a6870d11edb">

Searching for `95 Berkeley St, Boston` on Google Maps and using the perspective, we can determine that the photo was taken from `Arlington Street`:

<img width="800" alt="flag" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/8fa2cdda-9acc-4610-a1bd-4677da77314c">
<br>Double check using Google Street View, we will see a beautiful cityscape in the twilight:

<img width="800" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d812b89d-44c8-4d9a-bec8-178a9c2effc3">

### Flag: ``uiuctf{Arlington Street, Boston}``
