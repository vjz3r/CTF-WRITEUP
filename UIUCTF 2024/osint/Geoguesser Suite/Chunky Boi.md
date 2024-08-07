## Chunky Boi

<img width="437" alt="Screenshot 2024-07-02 021255" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/4330b213-e286-46f5-82db-6723f3e28666">

[⬇️chal.jpg](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/df45e3e8-6911-4b02-b210-cf822cb284bc)

## Solution:
Here is the initial information I have after searching for the details in the photo:

![first](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/61a7a32a-f950-475a-a667-6068e6f4e262)

Starting with the military airplane was not a good idea; I only found one website with its past locations, but none matched the airport in the photo:
 https://www.airhistory.net/photo/179798/07-7182/77182

<img width="600" alt="Screenshot 2024-07-07 015433" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/20afc026-8d7d-4c72-8ce8-d7373db2696a">

I went back to Google Lens and selected different search areas. I will prioritize checking the results with images of the forest edge outside the airport:
<br>There are three results pointing to `Seattle–Tacoma International Airport`
<img width="1000" alt="gues" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/d5920c6b-fdd4-4a69-86e7-a43eafce585e">

Checking on Google Maps, I see a long building in the corner of the airport near the forest, which looks quite similar to the one in the photo:

<img width="400" alt="Screenshot 2024-07-07 022016" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/8736c5b2-9133-4131-beef-8b4d2f6f9682">

<br>Using Google Street View, I'm quite sure I've found the right place.
<img width="1000" alt="Screenshot 2024-07-07 022113" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/af16bcb3-bb66-40b2-8542-65997403c2cb">

 We need to find the coordinates of the aircraft. In the picture, we can see the airplane right next to the ``PROLOGIS`` warehouse, so we will have the flag as:
 
 <img width="383" alt="flag" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/128c1892-5ba8-4a25-96e5-ff9ac0aef7fc">

### Flag: ``uiuctf{Boeing C-17 Globemaster III, 47.462, -122.303}``

## Postscript:
During the CTF, with some magical ability, I thought the airport I found with Google Lens wasn't the correct one `(╯°□°）╯︵ ┻━┻`
<br>So I kept searching, and I accidentally found a faster way to solve this challenge LOL
<br>**`I'll prioritize this way because sometimes we may not get the desired results when selecting the wrong search area in Google Lens, even just a little.`**
<br>Just search for Alaska Airlines and read the information on Wikipedia:
<img width="965" alt="Screenshot 2024-07-07 111802" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/08c7846c-fa41-4904-99fc-c2ea83764e77">
