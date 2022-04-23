# Pre-work - *Memory Game*

**Memory Game** is a Light & Sound Memory game to apply for CodePath's SITE Program. 

Submitted by: **Stephanie Ma**

Time spent: **5** hours spent in total

Link to project: https://glitch.com/edit/#!/glamorous-feline-airplane

## Required Functionality

The following **required** functionality is complete:

* [X] Game interface has a heading (h1 tag), a line of body text (p tag), and four buttons that match the demo app
* [X] "Start" button toggles between "Start" and "Stop" when clicked. 
* [X] Game buttons each light up and play a sound when clicked. 
* [X] Computer plays back sequence of clues including sound and visual cue for each button
* [X] Play progresses to the next turn (the user gets the next step in the pattern) after a correct guess. 
* [X] User wins the game after guessing a complete pattern
* [X] User loses the game after an incorrect guess

The following **optional** features are implemented:

* [ ] Any HTML page elements (including game buttons) has been styled differently than in the tutorial
* [X] Buttons use a pitch (frequency) other than the ones in the tutorial
* [X] More than 4 functional game buttons
* [X] Playback speeds up on each turn
* [X] Computer picks a different pattern each time the game is played
* [X] Player only loses after 3 mistakes (instead of on the first mistake)
* [ ] Game button appearance change goes beyond color (e.g. add an image)
* [ ] Game button sound is more complex than a single tone (e.g. an audio file, a chord, a sequence of multiple tones)
* [ ] User has a limited amount of time to enter their guess on each turn

No additional features implemented.

## Video Walkthrough (GIF)

If you recorded multiple GIFs for all the implemented features, you can add them here:
![ezgif com-gif-maker](https://user-images.githubusercontent.com/54160019/164862023-de3f4694-dc9e-4ba7-b451-791a6efbd07c.gif)

![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/54160019/164862324-baa488ea-3612-4534-aae9-eaf25bbe5d63.gif)

![](gif3-link-here)
![](gif4-link-here)

## Reflection Questions
1. If you used any outside resources to help complete your submission (websites, books, people, etc) list them here. 
https://www.w3schools.com/jsref/jsref_push.asp
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/random

2. What was a challenge you encountered in creating this submission (be specific)? How did you overcome it? (recommended 200 - 400 words) 
I encountered several challenges while implementing random pattern generation. After initializing my pattern variable to an empty array, I realized I did not know how to add items to an array in JavaScript. A Google search directed me to the first link above, where I learned that I should use the push() function to add an element to an array.
Then, when I tried to generate appropriate values to add to my pattern, I initially tried Math.random()*5, which caused an error because it produced floating point values. Next, I tried Math.floor(Math.random()*5)), which appeared to work initially before it also errored. By printing the resulting pattern to the console, I realized that this was because this expression had generated values between 0 and 4, and 0 is not a valid value for button number. Finally, I used Math.floor(Math.random()*5)+1, which worked. 

3. What questions about web development do you have after completing your submission? (recommended 100 - 300 words) 
The light, sound, and memory game created for this submission involves buttons that light up visually and sound effects that indicate the pattern to the player. How could this game be made more accessible to those who are visually impaired or hard of hearing? In general, how can we make websites more accessible to those with disabilities?
Services like Squarespace and Weebly abstract away the need for programming knowledge so that anyone can easily create a website, but at the cost of flexibility. Is there a way to make web development more accessible without sacrificing flexibility and creativity?

4. If you had a few more hours to work on this project, what would you spend them doing (for example: refactoring certain functions, adding additional features, etc). Be specific. (recommended 100 - 300 words) 
One feature that I would add if I had more time to work on this project is changing the page to replace the game buttons with a message when the game is over rather than having the win/lose message appear in a dialog box. There would then be a restart button that causes the game buttons to reappear if the player wants to play again.	
Another feature I would add is turning it into a multiplayer game where one player provides the pattern and the second player repeats the pattern. This could be accomplished by using the existing layout and having the buttons switch functions between setting and guessing the pattern. Alternatively the page could be designed so that it can be loaded in two separate windows, where the setter and guesser players play on different windows. The two sessions can be synchronized by using a randomly generated numerical code that both users enter. In this way, players who are not physically together could play against each other over the internet.


## Interview Recording URL Link

https://drive.google.com/file/d/1oAGQCPnrkvmk1ymTESWUU49ej2bdBUom/view?usp=sharing


## License

    Copyright Stephanie Ma

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
