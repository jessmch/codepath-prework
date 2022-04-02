# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Chau Ho**

Time spent: **4.5** hours spent in total

Link to project: [Glitch Project](https://glitch.com/edit/#!/harmless-polarized-dragonfly?path=index.html%3A1%3A0)

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

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [ ] Buttons use a pitch (frequency) other than the ones in the tutorial
* [x] More than 4 functional game buttons
* [x] Playback speeds up on each turn
* [x] Computer picks a different pattern each time the game is played
* [ ] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn


## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![](https://i.imgur.com/YF95lYE.gif)
![](https://i.imgur.com/KpXDDox.gif)
![](https://i.imgur.com/CIIudIb.gif)
![](https://i.imgur.com/rbMmRTT.gif)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
[Link 1](https://hackernoon.com/how-does-javascripts-math-random-generate-random-numbers-ef0de6a20131)
[Link 2](https://stackoverflow.com/questions/22679445/how-to-have-a-constant-value-for-a-variable-across-many-html-pages-using-javascr)
[Link 3](https://stackoverflow.com/questions/33999948/react-native-attempted-to-assign-to-readonly-property)
[Link 4](https://stackoverflow.com/questions/43787006/typeerror-attempted-to-assign-to-readonly-property-when-typing-in-a-text-fiel)
[Link 5](https://stackoverflow.com/questions/30035932/how-do-i-use-this-javascript-variable-in-html)

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
- Most challenges I encountered were during writing up script.js. One of them was when I had to make the Stop button change back to Stop when the user wants to pause the game. I thought there was something wrong with my other functions that caused the button to not respond when interacted. However, I saw that the Start button can change to Stop button, so it meant my stopGame() function was the root of the problem. In the function, I set the Start button to remain visible (add(“hidden”)), which I was supposed to make it hidden by doing (remove(“hidden”)). Moreover, I had to do the opposite thing for the Stop button within stopGame() function. As expected, after I made some modifications to the function, both Start and Stop buttons can change to one another when interacted. Another challenge I had that was also in script.js was when I tried to implement a feature that makes playback speed up on each turn. I was trying to assign constant clueHoldTime to a variable so that I could use it playClueSequence() function and reduce it after every time a sequence is finished. I decided to leave it as a constant, then I went ahead and create a variable called reduceHoldTime inside that function, and set it to be equal to the constant clueHoldTime. However, when I manipulated the variable inside the for loop, I forgot to set it to be equal to the variable “delay”, so when the setTimeOut() function was called, I did not notice any difference to the speed of the game. I was struggling for a moment, then I found that I forgot to set the “delay” variable to be equal to reduceHoldTime.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
- I have noticed that we have to have HTML, CSS, JavaScript files in order to make a fully functional page in this prework project. I would like to ask if it is possible to only have HTML file to build a website or not because CSS is just a user interface feature (enhance the layouts), and Javascript is scripting that helps the website become interactive. I also wonder why we do not combine JavaScript file with CSS file because I see that they seem to use the same language format. Is it because of the code structure issue or is there any other reason why that cannot be done? I also have a question regarding frontend and backend. From what I understand, what we have done so far in prework project is fundamental of fullstack, which includes frontend and backend features, what are other things we can do to improve our webpage?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
- First of all, I would add some more features. What I would like to implement is to allow people to play together on the same webpage session (both offline and online). For example, I can choose the number of players I want to compete against. Then, if I play the game in offline mode with my friends (without Internet), we do not have to create an account to play as we all can play on the same device. However, if I decide to play online, then each person has to create an account, then join a room with total number of players specified so that I can start a game with other people. Second, I would like to enhance the layouts of the webpage. I want to add more complicated tones to the game, which can be piano rhythms. Moreover, I want to add multiple themes to each of the buttons so that the user can choose which theme they would want each button to have. 



## Interview Recording URL Link

[My 5-minute Interview Recording](https://drive.google.com/file/d/1g4UmgtArj4vWog5VsEerNgOe3_zPfHSc/view?usp=sharing)


## License

    Copyright [Chau Ho]

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.