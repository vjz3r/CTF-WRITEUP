## New Dallas

<img width="442" alt="Screenshot 2024-07-02 021207" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/6d263c64-8205-4439-a5f7-7afe5125e487">

[`⬇️chal.jpg`](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/99c36cb9-49a4-4084-9204-03ecdfed974a)

## Solution:

After solved this challenge, I had to get my eyes checked again (´。＿。｀)
<br>The photo doesn't have any useful information. Using Google Lens, we found out that this is a type of subway train in China:

<img width="1000" alt="Screenshot 2024-07-07 135001" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/ab72d924-ff54-45aa-b7cc-04876dd6c80f">

<br>I really believed that Line 6 (Shenzhen Metro) was the correct answer. I meticulously tracked its route to find where the tracks cross the highway:

<img width="753" alt="Screenshot 2024-07-08 005310" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/df193421-23c0-4e89-a464-e82afdea3030">
<br>It took me a long time to realize I was wrong. Then I fell into a silent period because I wasn't sure about the colors on the train, so I checked many lines with various shades of green.

<br><img width="300" alt="huhuhu" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/8fc124e8-d6a7-4b0c-8bd8-7e0eb89d8640">

***` Take a deep breath...`
<br>`...and get back to the challenge.`***

Using [Overpass-Turbo](https://overpass-turbo.eu) for the search wasn't effective:

![image](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/7c5d2666-9660-4eea-ba73-025c65dc7f25)

because we need to know the exact hex color code. Example:

<img width="245" alt="Screenshot 2024-07-08 011336" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/b512d9d0-a176-4d11-8ea1-1783729b8e94">

<br>After that, I found this page:
https://en.wikipedia.org/wiki/Urban_rail_transit_in_China
<img width="900" alt="Screenshot 2024-07-08 005212" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/325965dc-b288-4674-abec-fb4481facbfe">

<br>This page has everything I need, but it still has too much information. So I came up with the idea of using ChatGPT to list all the metros in China, then filter out the ones that don't have green train lines and elevated tracks crossing highways:

<img width="950" alt="chatgpt_result" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/dc9f21f4-55e6-4911-a19d-3a594a85cb5e">

After cross-referencing between the results from ChatGPT and Wikipedia, I was able to eliminate quite a few options because the shape and decoration of the trains didn't match the ones in the picture.
<br>After a painful search, I finally found it:

<img width="750" alt="Screenshot 2024-07-08 014732" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/68921c61-15b4-4b96-a77d-ce0a40ef40d9">

<br>Because this is China, there are very few street view images on Google Maps, so I used Baidu Maps to check it:
![image (2)](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/593c3b3b-af14-4adc-aa1f-12af55c7ff6f)

Identifying the exact location, I switched to Google Maps to determine the coordinates (because I dont know how to do it on Baidu Maps 😅)
<br>Turn on terrain mode to see the exact road. In satellite mode, the road is skewed:

![flag](https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/9da08c6f-714f-488b-a83f-f3e589840c98)

The nightmare is over, here is the flag:

### FLAG: ``uiuctf{31.579, 120.388}``
