# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **AYOMIDE ADETUNJI**

Time spent: **29** hours spent in total

Link to project: (https://glitch.com/edit/#!/false-scarlet-tile)

## Required Functionality

The following **required** functionality is complete:

* [x] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [x] "Start" button toggles between "Start" and "Stop" when clicked. 
* [x] Game buttons each light up and play a sound when clicked. 
* [x] Computer plays back sequence of clues including sound and visual cue for each button
* [x] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [x] User wins the game after guessing a complete pattern
* [x] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [x] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![http://g.recordit.co/yKA5aJrhUv.gif]

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[https://stackoverflow.com/questions/5836833/create-an-array-with-random-values]

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
 
[I took it for granted that the code we needed to implement was made available to us and I thought that I’d never find any issues with my game. But as my Light and Sound Memory game started to get more complex with the amount of code I was implementing, I realized that I doing something wrong which made my game buggy. I noticed this when I began testing my program and found that every time I clicked on the wrong button, to purposely lose and stop the game, my code would act strangely when I tried starting again. When I clicked on the start button, it would play more than a single clue, instead of only one clue. I wasn’t sure if this was how the game was supposed to run, so I referred back to the demo video and found that this wasn’t happening in the video. Then I realized that this was definitely an issue and started visually debugging the code. I decided to do a quick check of the other files, but it only made sense that the issue was in the JavaScript file because it looked like an unwanted function call was occurring every time I lost or stopped the game. So I began looking at the previous function calls carefully to see if I could figure out what the issue was. I checked all the constant and global variables to make sure nothing was off, I checked all the functions to make sure everything looked right, and then finally I noticed something that appeared to be a mistake. I noticed that in my stopGame() function I had a call to the playClueSequence() on the last line in the function block. And instantly I knew that was the issue because after the game stopped or the player lost, nothing else was supposed to happen. To verify that this was truly the only issue in my code, I went back and forth comparing my code to the one provided to us on the SITE Program Pre-work website. I made the appropriate change and my game played perfectly. I was so happy that I figured out what the problem was because I know my program wouldn’t have run properly otherwise.
]

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
 
[Before I completed this submission, I didn’t really understand how multiple programming languages could work together as one to make an application or even a website on such an excellent level. But after I was able to see them working right in front of me and with the explanation provided on the website, I found it very interesting. This made me curious about a lot of things. Like how many languages does a web developer have to be proficient at? And when working on group projects, do groups of individuals work on different aspects of the project? Will a group of people focus on the style? While some focus on the functionality while others focus on how all connect together. Being someone who really enjoys art, it has made me even more interested and curious about how style comes into play from User Experience and User Interface design. Would the design or front-end part of the project be one that a product designer works on, while the back-end is one where the more code-intensive work takes place? A lot of the terminology used in the prework is very similar to those used in my current and previous programming classes and it makes me wonder how similar these languages are and how different they can get when it comes to learning and understanding new ones? I can imagine that as I get more exposure to more programming languages and projects I will surely have more questions.]

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
 
[If I had a few more hours to work on this project, I would spend more time on the design of the website. When working on the prework, I really enjoyed the art and style aspect of the project and found myself spending a lot of time playing around with the design of the website, and the many shapes that could have been used when designing the interface. I enjoyed just typing in different colors and seeing which ones would pop up. I also enjoyed messing around with sounds and the different pitches and intensities that the Art of Web website had to offer. It made me curious about the endless possibilities of art and design when it came to making a website. On the functional side of the game, I would have spent more time making it as cheat-proof as possible. One thing I realized after testing the game numerous times was that if the player clicks on the clues while they are being given, the game continues and counts that as correct points. I noticed this issue and used it to test some of the other functions of my program, but it is definitely something that many players would probably notice fast and use to their advantage. To fix an issue like this, one would probably have to make a condition that doesn’t allow buttons to be clickable until after the last clue has been given. This way, players don’t get to click until all clues have been given. 
]



## Interview Recording URL Link

[My 5-minute Interview Recording](https://umd.zoom.us/rec/share/5KUcMygu2g22ZuLBkJdhmzV6rUEltdFZJHCtTeX5oRH8G18T_SINDck2fccIV5VR.THZcytzb96SS9Rrk?startTime=1650495752000)


## License

    Copyright [AYOMIDE ADETUNJI]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
