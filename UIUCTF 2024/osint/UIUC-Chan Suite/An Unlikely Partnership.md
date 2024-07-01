## An Unlikely Partnership

<img width="443" alt="An Unlikely Partnership" src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/6c4fdaca-8149-4abc-8755-b1197d876b25">

## Solution:
Continuing with the challenge ``Hip With the Youth``, we get a LinkedIn link attached to the Threads profile:

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/eda376c3-d97a-466b-8b0d-6e31523e5f16" width="460">

https://www.linkedin.com/in/long-island-subway-authority/

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/78872146-a6df-45f1-863d-892f70812260" width="360">

In this challenge, we need to find a business partner, and there's no other place to look than LinkedIn ╰(*°▽°*)╯

For LinkedIn, I always search in the following order:
`Contact info -> About -> Activity -> Experience -> Skills`

And found a person endorsed for the Transportation skill in the `Skills` section:
https://www.linkedin.com/in/uiuc-chan/

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/e821aa4b-1045-48fd-91e2-ea1071e155e5" width="560">


Access this profile, we can easily see the flag in the `About` section:

<img src="https://github.com/vjz3r/CTF-WRITEUP/assets/83077449/6678344f-57a2-4ad7-a0e8-0a2092ffe763" width="500">

### Flag: ``uiuctf{0M160D_U1UCCH4N_15_MY_F4V0r173_129301}``
