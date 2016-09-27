# DT228/DT282 Object Oriented Programming 2016-2017

Resources
---------
* [Webcourses](http://dit.ie/webcourses) - Course code: CMPU2016
* [Slack](https://oop-2016-2017.slack.com)
* [Processing](http://processing.org)
* [The Processing language reference](http://processing.org/reference/)
* [Learning Processing: A Beginner's Guide to Programming Images, Animation, and Interaction (Morgan Kaufmann Series in Computer Graphics)](http://http://www.learningprocessing.com/)
* [The Nature of Code](http://natureofcode.com/)
* [Eclipse](http://eclipse.org)
* [The git manual - read the first three chapters](http://git-scm.com/documentation)
* [A video tutorial all about git/github](https://www.youtube.com/watch?v=p_PGUltnB6w)
* [The Java Tutorial from Oracle](http://docs.oracle.com/javase/tutorial/)
* [Games Fleadh](http://www.gamesfleadh.ie/)
* [The Imagine Cup](https://www.imaginecup.com/)

## Contact the lecturer
* Email: bryan.duggan@dit.ie
* Twitter: [@skooter500](http://twitter.com/skooter500)
* Slack: [oop-2016-2017.slack.com](https://oop-2016-2017.slack.com)

Some assignments from previous years:

[![YouTube](http://img.youtube.com/vi/sPjZSRCmt1U/0.jpg)](https://www.youtube.com/watch?v=sPjZSRCmt1U)

[![YouTube](http://img.youtube.com/vi/0hQt7BKxBcU/0.jpg)](https://www.youtube.com/watch?v=0hQt7BKxBcU)

[![YouTube](http://img.youtube.com/vi/S575a92AsuQ/0.jpg)](https://www.youtube.com/watch?v=S575a92AsuQ)

# Week 3
## Lecture
- [Trigonometry problem set](http://www.tippcityschools.com/cms/lib6/OH01000855/Centricity/Domain/111/Acc%20Geom%20eDay%201.pdf)
- [Simple Spirals sketch](processing/spiral)
- [Psychedelic Spirals sketch](https://github.com/skooter500/psychedelicSpirals)
- [Circles explained](https://www.khanacademy.org/math/trigonometry/unit-circle-trig-func/unit-circle-definition-of-trig-functions/v/unit-circle-definition-of-trig-functions-1)

Generative art:

[![YouTube](http://img.youtube.com/vi/LaarVR1AOvs/0.jpg)](https://www.youtube.com/watch?v=LaarVR1AOvs)

[![YouTube](http://img.youtube.com/vi/x0OK1GiI83s/0.jpg)](https://www.youtube.com/watch?v=x0OK1GiI83s)


In the lecture we learned how to make spiral shapes using a for loop with sin and cos. In the lab today you will make a sketch that draws star shapes with random numbers of points and random colours. Here is what the finished sketch could look like:

![Sketch](images/p5.png)

Here are some things you might need to read up on first:

- [random function in Processing](https://processing.org/reference/random_.html)
- [Using the modulus operator](http://www.cafeaulait.org/course/week2/15.html)

You can put all your code into the setup method as this sketch doesn't use any animation (unles you want to attempt the advanced part)

This is how I suggest you think about the problem.

- You will need a for loop that goes from 0 - TWO_PI. There will be twice as many steps as there are points on the star.
- You can use % (modulus) to decide whether the x and y values you calculate should be the tip of a point or base of the point (the pointy bit or the trough).
- Use line in your solution
- I strongly suggest you start the lab by just drawing a single star and then maybe move on to drawing multiple stars using a for loop.
- You could write a methdod to draw a single star with parameters

### Advanced
- Make a beautiful animated sketch with stars and spirals and share a picture/video/animated gif on the slack
- Use sin and cos to control colours

Do MCQ 2 and MCQ 3

# Week 2
## Lecture
- [Quadrants sketch](processing/quadrants) - How to use the if statement
- [Rectangle sketch](processing/rectangle) - Rectangle moves back and forth across the screen
- [Examples of using loops in Processing](processing/loops)
- [Solution to the BugZap lab](https://github.com/skooter500/BugZap)

# Lab
## Learning Outcomes
- Use what you learned in class to build a complete game system in Processing
- Practice drawing stuff and working out relative co-ordinates
- Practice using variables and compound if statements
- Gain experience thinking computationally
- Learn how to use random numbers
- Learn how to get input from the keyboard
- Learn how to import libraries into Processing

This is a video of a game called Bugzap that you can try and make in Processing today. There is a fair bit to it, so don't worry if you don't manage to complete everything.

[![YouTube](http://img.youtube.com/vi/s6PA8jtWneQ/0.jpg)](https://www.youtube.com/watch?v=s6PA8jtWneQ)

How you should do it:
- Get the main game working first and then if you have time, add fonts, sound, the splash screen and the game over screen.
- Write some code to draw the bug. You can write a method to do this if you like (but it's not essential). Here is [an article on using methods in processing](https://processing.org/examples/functions.html). Also make global variables for the bug position and size.
- Get the bug moving. The bug moves a random amount either to the left or the right and it also moves down the screen. Use the random method in Processing to generate random numbers. Also the bug can't move off the screen. You can use the % operator to make something happen on an interval. For example:

  ```Java
  if (frameCount % 60 == 0)
  {
    // Code in here will happen once per second
  }
  ```
- Write some code to draw the player. Use variables to control the player position and size. A method is good here too!
- Write code to move the player in response to a key presses. This is one way to do keyboard handling in Processing:

```Java
if (keyPressed)
{
  if (keyCode == LEFT)
  {
    // This will happen if the left key is pressed
  }
}
```
- Now add the player lazer. I used to UP key for this. I just drew a line for the lazer.
- Make a variable for score and check for collisions between the lazer and the bug. Add a variable for score. You can print stuff to the screen using the text method in Processing. In my version, I actually used [this processing library](http://www.foobarquarium.de/blog/processing/MovingLetters/) which makes wireframe text.
- Make some sound effects and add them to the game. I used [BFXR](http://www.bfxr.net/) to make the sounds and the Minim library to play them, but you might prefer to use the [built-in audio methods in Processing](https://processing.org/tutorials/sound/).
- Add the splash screen and game over screen

Upload pictures of your creations to the Slack and do this weeks MCQ.

# Week 1

## Lecture
* [Introduction slides](https://1drv.ms/p/s!Ak7y2552PWCrhONjAgskv4PATGqdpw)
* [The contract for this course](https://1drv.ms/w/s!Ak7y2552PWCrjPYXt8HlWl1T1cg5Og)

## Lab

### Learning Outcomes
- Sign up for the class Slack
- Enroll on Webcourses
- Become familiar with the syntax of Processing
- Become familiar with writing and running sketches in Processing

Firstly, go to https://oop-2016-2017.slack.com and sign up for the slack with your DIT email address. Make sure and click *Create an account* rather than try and enter your DIT credentials at the login screen, which wont work. When you are signed up, send a little greeting to everyone on the #general channel. If you have a smartphone, you might want to install the Slack app. It's free. Also if you install the app, you will probably want to disable certain notifications, otherwise your phone will be buzzing every time someone posts anything. [Here is an article that explains how to do this](https://slack.zendesk.com/hc/en-us/articles/201649323-Channel-and-group-notification-preferences).

Log onto Webcourses and enroll on the module CMPU2016.

Look up the following methods in the [Processing language reference](http://processing.org/reference/ ) to make sure you are clear about the syntax and parameters:

* noStroke
* noFill
* line
* ellipse
* rect
* background
* stroke
* fill
* size
* arc
* triangle

Write a processing sketch to draw the following shapes:

![Sketch](images/p1.png)

![Sketch](images/p1.1.png)

![Sketch](images/p1.2.png)

I prefer to draw the shapes on paper first before I try and work out the coordinates. Try experimenting with different colours

[Log onto webcourses](http://dit.ie/webcourses) and do this weeks MCQ.