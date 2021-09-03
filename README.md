# Fruit-Ninja-AR-VR-game-
1. Idea:- 
The idea of the project was originated after watching a video on YouTube of an AR/VR game. The game 
was all controlled just by the gestures of the person and by any external hardware device. The source link 
of the video is- https://www.youtube.com/watch?v=J6e_YpwmLQc
2. Implementation:- 
Now for the implementation part, we went through the documentation of some python libraries and 
functions. Which are as follows
a) OpenCV 
OpenCV is the huge open-source library for the computer vision, machine learning, and image 
processing and now it plays a major role in real-time operation which is very important in today’s 
systems. By using it, one can process images and videos to identify objects, faces, or even handwriting 
of a human. When it integrated with various libraries, such as Numpy, python is capable of processing 
the OpenCV array structure for analysis.
a) pygame
pygame is a free and open-source cross-platform library for the development of multimedia 
applications like video games using Python. It uses the Simple DirectMedia Layer library and several 
other popular libraries to abstract the most common functions, making writing these programs a more 
intuitive task. 
Main Section 
1. Project Idea- To make Fruit Ninja AR (Augmented Reality) game with the help of NumPy library of python and then controlling the game with 
gestures using open cv library. 
2. Aim of the project:
In the game development, AR has the power to turn 3D models and videos into a reality. Virtual Reality determines the high-end 
user interface that involves real-time simulation and interactions. This makes the platform easy to connect with a virtual environment 
where users can feel the digitally created space. Therefore, they are instantly getting popular these days, and the expansion of AR 
and VR gadgets now offer a breakthrough technology that works as an extension to mobile capabilities. 
3. Gesture Mechanism
Voice and Gestures are the widely used ways of communication. We have voice-controlled gadgets like Alexa and Siri-enabled 
devices to control our homes using voice commands. We do have gesture-controlled TVs. Even the dashboards on top-of-thesegment luxury cars are gesture controlled. The video games are gesture-controlled. 
Main Project: Fruit Ninja game 
4.1. Introduction 
In Fruit Ninja, the player slices fruit with a blade controlled via the hand gesture by detecting the palm 
movement of the player. As the fruit is thrown onto the screen, the player swipes their palm in front of 
the screen and web cam to create a slicing motion, attempting to slice the fruit in half in a particular time 
duration. As soon as the time gets over it shows the score board of how much you have scored. 
Webcam window 
4.2. Contour Detection and Bounding Rectangle 
Since we were using color detection to track an object, this raised an issue that every new user will have to set colors for their 
choice of object which is a big headache. So, we came up with an idea of using palm of the user to control any movement in the 
game. We have to move our hand in order to move the blade. Just keep your hand in front of the webcam and adjust it in such 
a way that a blue square appears equipping your hand and detecting the position of your whole palm. 
 4.3. Check if/where object moves 
For this, we can define our own quadrants on a frame and locate the position of the centroid of the bounding rectangle in those 
quadrants. Based on the quadrant in which the point lies and can use the hand gesture in order to move the blade.
Game console window 
Scoreboard window 
4.4. Visual Representation of Game 
 After this you have to move your hand in order to move the blade to slice the fruits’ images and score 
accordingly. As much as the blades slice the fruit by your hand gesture, you’ll score a plus point for each 
cut. 
4.5. Challenges we faced: a. Installation issues: To run some of the functions we had to install some new libraries that we weren’t aware of. 
b. Color detection: While detecting the color we wanted to track, we had to struggle with the Hue and Saturation bars.
Resolved: Since we were using color detection to track an object, this raised an issue that every new user will have to set 
colors for their choice of object which is a big headache. So, we came up with an idea of using palm of the user to control any 
movement in the game.
c. Suddenly our code started throwing an error “module CV2 not found” which was finally resolved by 
uninstalling and installing some libraries back again. 
d. The foremost challenge was how to end the game as it was not a multiplayer game hence, we tried to deduce 
and limit the dropping of fruits but it led us to the more complex coding and installation of some more libraries which leads us 
to some errors. 
 
Resolved: That is why we introduced the timer of 60 seconds and after showing the score board the game and webcam window 
disappeared and after we click on close button the whole window exits. 
e. After switching from color detection to palm detection, we realized that our system is unable to 
detect the palm correctly and we had to struggle for the same. 
Resolved: So, we checked the cascade file and changed some threshold levels (which is basically the assignment of pixel 
intensities to 0’s and 1’s) for right and left palm detection in first.xml file and checked but it only worked 50 or 55 percent 
efficiently. 
 5. Final Project (after the changes and correction) 
After including the timer of the 60 seconds we were only facing the issue of palm detection as it was still not detecting the 
whole palm and the values of threshold levels was fluttering so, we decided to limit the contour region and moved to fist 
detection by using the cascade file for the same. 
