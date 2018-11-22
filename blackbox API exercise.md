# BlackBox API
*Basics:* Explore black box puzzles with an automated tool over an api.

*Source:* an existing workshop, new puzzles.

*Aim:* Tiny tools to run many tests. 

## Requirements
At a minimum, you’l need something with a browser (ie your phone).

Better: something easy to type on, something which runs your weapon of choice, something you can generate data with (ie your laptop).

Tools you could use: the URL in your browser – it’s just a GET. Postman. Paw. cURL.


## Logistics
Note that these APIs validate your input and tell you what they expect, and (roughly) what’s wrong.

Puzzle29 [Bare API](http://handsonlab.workroomprds.com:8001/puzzle29 ), [working example](http://handsonlab.workroomprds.com:8001/puzzle29?button1=up&button2=up&button3=up&button4=up), [Puzzle29 GUI](http://blackboxpuzzles.workroomprds.com/patreons/PP01/)

Puzzle31 [Bare API](http://handsonlab.workroomprds.com:8001/puzzle31), [working example](http://handsonlab.workroomprds.com:8001/puzzle31?buttonA1=down&buttonA2=down&buttonA3=down&buttonB1=down&buttonB2=down&buttonB3=down&buttonC1=down&buttonC2=down&buttonC3=down), [Puzzle31 GUI](http://blackboxpuzzles.workroomprds.com/puzzle31/)

Docs via [Postman](https://documenter.getpostman.com/view/169247/RzZ4o1MA)


## Process
The system under test is the thing that lies behind the UI, and also behind the API. One piece of code.
(As usual) What it does can be described in a tweet. If you can describe it, you’ve solved it.

Where do you start testing? What does having two interfaces do to your test approach? 

Once we’ve tested, we’ll consider:
* What qualities does the API have, and what does that tell you about the puzzle?
* What information does the API require, and what does it return?
* What are some differences in your approach?
* What is simpler – and what is more difficultt?
* How do you identify what’s in the system under test, and what’s not for your attention? Can you keep focus?
