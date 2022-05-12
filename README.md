# COLLABDRAW ( Make Art Here!) 
![Landing Page](https://eric-asare.github.io/ConnectionsLab/projectTwo/design/doc-images/landingPage2.png)

## Description:
A collaborative drawing application built using Node, Express, and socket.io.

Link to working app: 

“CollabDraw” is a collaborative drawing application where two users come together to make art under a time condition. This is for you to draw a unique Art together with your friends in real-time over the internet in your browser. Take turns, complete each others drawing, be in sync and foster stronger relationships. Afterall, when it comes to art, we don’t make mistakes, just happy little accidents. Joy is even greater when it comes from the unexpected. Unleash your creativity and boost teamwork<br/><br/>


<p align="center">
  <img 
    width="450"
    height="300"
    src="placekitten.com/450/300"
  >
</p>

## Inspiration:
I enjoy drawing on a sheet of paper with no idea of what I want to end up with. I experiment strokes and at the end I am always shock what I come up with. I then turn to my friends and the person next to me, look what I have done. 

---

> I made this app for you and me if you ever had the joy of drawing or sharing a drawing with a friend. Let's Draw.
> -- Eric (CTO)
---
<br/><br/>

<p align="center">
  <img 
    width="200"
    height="200"
    src="placekitten.com/200/200"
  >
</p>

## Production

 _The Plan_
I will be building MemoICE in two phases. The first phase will be purely functional with less aesthetics for user testing whilst the second phase will be an upgrade on the UI based primarily on the results of the user testing. 

_The WireFrame_

I started off with a simple sketch of the game flow to inform the phase 1 coding. I didn't make a lot of sketches in project two because I focussed more on the communication between client and server (game flow) which is listed below. The user interface became really clear as a result of the user testing. 

![Layout Sketch](https://eric-asare.github.io/ConnectionsLab/week10/memoICE/design/collabDrawWireframe.png)

_The Game Flow Steps_  
* Two users join the same room. Room is full when two people join. When a third User Join, he or she is prompted to join another room

* (NEW) Change Background base on Room (Famous Art from there)

* Only one of the users has to select the Drawing mode (Free Drawing or Challenge Mode), the clients sends a signal to the server to load the data (timer and logic) for the drawing mode. Both modes of drawing are pretty similar, the difference is that in the challenge mode, the users will be shown a prompt like "draw a castle" before the timer starts. 
   
*  Client upon receiving this drawing logic data displays to the users ("continue each others drawing to create the unexpected" , "collab to draw a flower") and starts the drawing timer. 

* The 10/20 countdown timer starts for the first user, he or she gets to draw while the other user can't (waits his or her turn). Each user continue each others drawing inturns until the whole experience timer is over(~3mins). 

* The logic for the turns is that whenever a client's timer is over, the client sends to the server and the server emits who's turn. 
   
*  Once the timer is done, the clients sends to server drawing time is over, the server sends to the client to view the final product, explore the gallery ( what others have drawn, exit or draw another
  


## Workflow:

_Hellooo (MamaMia):_


## Features:

## User Testing Feedback:
_What I change_

_What I did not change_


## Key Challenges / Things I Learnt:
1.Timer : I tried different ways
* a timer loop with another timer loop inside, hard, how do I send info in and out and not disrupt the timer

* changes were not reflecting for both users
-  io.to(socket.roomName). came to the rescue


* was doing this : starts the timer, send info to the server to start logic, the server sends the turn to the client, was not working so I turned it around. 


* loading canvas

* preventing another user from drawing

* Learnt a lot about p5 js
- adjusting audio volume
https://www.youtube.com/watch?v=Pn1g1wjxl_0

## Next Steps / More Ideas:
*


## References:

* Create shearable room link : https://stackoverflow.com/questions/71037062/create-a-sharable-url-for-a-room-nodejs-socketio

* https://stackoverflow.com/questions/31373455/socket-io-rooms-based-on-link

* Drawing Ideas : 
No More Blank Pages: 60 Easy Drawing Ideas - CreativeLivehttps://www.creativelive.com › Home › Posts

* Get random : https://stackoverflow.com/questions/4550505/getting-a-random-value-from-a-javascript-array

* Meee : 
* Hello : 
* You: 

* to load p5 only when you are ready: https://stackoverflow.com/questions/56639804/is-there-a-way-to-only-run-p5-js-once-an-event-happens


https://github.com/processing/p5.js/wiki/Global-and-instance-mode

* animations : https://animista.net/play/attention


*p5 reference : https://p5js.org/reference/#/p5/draw


* draw an element outside draw box: https://stackoverflow.com/questions/50770189/p5-js-drawing-an-element-outside-draw

* Save canvas data to file : https://stackoverflow.com/questions/5867534/how-to-save-canvas-data-to-file


* pencil thickness (https://editor.p5js.org/Zoe/sketches/HJdsXS1BZ)


* https://stackoverflow.com/questions/24779288/sending-a-canvas-image-over-socket-io


* learnt that use and get are different things an dI have to do something like

    fetch("http://localhost:4000/drawingsApi")


* needed to use namespace


## Presentation
* Slide 1 - Project Name
* Slide 2 - Tech Stack
* Slide 3 - Here is the link and this is how to play
* Slide 4 - Next STEPs (neDB - add image)
* Slide 5 - The Biggest Challenge