# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by:Yihua Shen

Time spent: **#** hours spent in total

Link to project: https://glaze-thundering-answer.glitch.me

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
* [x] Buttons use a pitch (frequency) other than the ones in the tutorial
* [ ] More than 4 functional game buttons
* [ ] Playback speeds up on each turn
* [ ] Computer picks a different pattern each time the game is played
* [x] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

The following **additional** features are implemented:

- [ ] List anything else that you can get done to improve the app!

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:

![](https://i.imgur.com/OZR0btI.gif)


## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here.
I looked up parts in documentation-like resources like w3schools to see more examples of how some of the methods are used like getElementById and see other ways of using it. 

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
A challenge that I encountered was when I arrived at the end of the project, the game did not perform as expected. The game would start as intended but when I click the corresponding button, it would send the alert that I have failed the game. To solve this, I isolated this issue to the logic side of things since for some reason, it is evaluating my input as incorrect eventhough it is correct. Because of this, I went to script.js since that is the part that handles the logic. I then looked at the part specifically for the game and noticed that there was a comparison being done and for some reason, the evalulation of the statement is triggering an end of the game. I thought a potential cause of this could be an off by one error due to zero based indexing but I thought the best way to debug is just to output the two things being compared by using console-log. I saw that "btn" is always giving 1 even though I am clicking on the second one. Because of this, I went back to the original buttons and saw that I had forgotten to modify all the buttons accordingly which is what led to the problem.

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
One question I had while I was building the project is whether or not there were cleaner ways to organize style.css. HTML and JS seem like they could be organized in a pretty organized way since there are functions in JS and HTML is ordered like a tree. However, for CSS, it seems like it is everything in one file and there is really no structure. I am curious as to what happens when the project becomes much bigger and there are more elements and how precedence in styling would work. I am also interested to learn more about additional tools that would make web development more interact as the current websites in the market allow for a bunch more functions and features and I am curious how it is all possible. 

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
One feature I would add is to randomize the sequence since currently, the sequence is hard coded and I think a player would have more fun with the game if the challenge is new every time. I would also implement a score board of some kind to be able to track the top scores so far so that the user could continuously challenge themselves. I would also make the interface look a bit nicer perhaps adding additional styling. It would also be a cool idea to segment the difficulty level so that the user can choose how long the sequence is so depending on the skill level of the user, it could change. I would also explore the idea of making the sequence continue towards infinity so I would generate a random number each time and see if the user gets it correct. If it is correct, they would continue and the game would not terminate until an error is encountered.



## Interview Recording URL Link

https://youtu.be/4SXCsN8iTIk


## License

    Copyright Yihua Shen

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
