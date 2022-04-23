# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: JohnJoshua Etta 

Time spent: ~13 hours spent in total

Link to project: https://groovy-delirious-stage.glitch.me/

## Required Functionality

The following **required** functionality is complete:

* [ ] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [ ] "Start" button toggles between "Start" and "Stop" when clicked. 
* [ ] Game buttons each light up and play a sound when clicked. 
* [ ] Computer plays back sequence of clues including sound and visual cue for each button
* [ ] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [ ] User wins the game after guessing a complete pattern
* [ ] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](gif1-link-here)
![](gif2-link-here)
![](gif3-link-here)
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[I used outside resources to help me add all the additional optional features. A couple of websites really helped: 
w3schools.org
developer.mozilla.org
stackoverflow.org
linterrors.com]

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
[Challenges that presented themselves to me were two of the four additional optional features that I integrated. Specifically, I found speeding the game up by a consistent increment each round a little difficult, as well as using a random secret pattern. The speed of the game is originally constant, with each hint playing at the same speed each round. I made a couple friends play, and as I watched, I noted that it was a tad bit too easy for most of them. Making the pace of the game increase over its duration makes for more of a challenge, so I saw that as a feature that I had to implement to spice things up. To accomplish this, I first commented out the constant “clueHoldTime” and created a new variable of the same name. I then went into the for loop of the “playClueSequence” function and shaved off 8.5 milliseconds each round. I experimented with other amounts of time before settling with 8.5, starting off with 50, then 30, then 25, 15, and 12.5. The problem with the former times was that the game would speed up a considerable amount before being unplayable towards the end due to hints that only lasted the blink of an eye. Shaving off 8.5 milliseconds was more practical because it’s a much more gradual transition in speed. On the other hand, there’s the randomized secret pattern. Originally, the code comes with a preset array of integers that determines the pattern every single time. This gets repetitive and one could easily just play time and time again to memorize the pattern and win. Randomizing the pattern fixes this problem. To do this, I created a function called “generatePattern” that uses Math.random. Inside of a for loop that iterates until 16, I assign each index a random number. And then, every single time the game is started, the method is called, and a new array is formed.]

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
[Web development has always interested me due to my generation growing up on the internet. I grew up watching YouTube, playing adobe flash games, and reading random articles on Wikipedia. Over the course of time, I have seen websites become increasingly interactive and complex in design. Things that I wonder are how websites get their addresses, how websites can be linked to one another, and how sound and images are added to your site to give it life. How do you toggle certain animations/sounds when things are clicked or hovered over? I am still new to the subject(s), and continue to educate myself, but I have heard of terms like “front-end” and “back-end” engineer. To the best of my knowledge, front end has more to do with the aesthetic of a website. Back-end is a concept that needs to be explained to me more clearly. These are two distinct roles, and someone that contributes to both is considered a “full stack” engineer. Things like streaming services amaze me as well. How do sites like YouTube and Netflix work? Netflix has hours upon hours of content on it, various movies, and series available to you at the simple action of a click. The same goes for YouTube. YouTube is a pioneer in the sense that ordinary people can also contribute to the site, not just the developers. I would really love to learn the ins and outs of web development and software engineering.]

`   4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words)` 
[If I had a few more hours to work on the project, I would have put more effort towards completing the last two optional features and then seeing what I could do even more to make my project more personalized and unique. After a couple attempts, I settled for what I had. Adding the ticking clock cost me a lot to work on. I was going to give some life to my buttons by adding images and sound but as I am nearing the deadline, I decided to play it safe. After doing those two things, I would have loved to add a “GAME OVER!” voice track when you lose, and a “YOU WIN!” voice track when you win, the same as the classic ones you hear in arcade games and such. Maybe even some images to look at around the website because my game looks a little bland. ]



## Interview Recording URL Link

[My 5-minute Interview Recording](your-link-here)


## License

    Copyright [JohnJoshua Etta]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.