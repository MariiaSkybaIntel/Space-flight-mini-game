<b>THIRD PERSON SPACE FLIGHT MINI-GAME</b>

The code for this game is written in Processing language (Java Mode);

<b>Important</b>

Copy the code into a new Processing sketch and save it in a folder with the same name;

Create a new folder called "Data" inside the main sketch folder;

Download and store all the attached files into "Data" folder for the game to work correctly;

DKThievery.vlw font must be installed;

Minim library must be installed in Processing to play audio files;

<b>GAME LOGIC</b>

Control the spaceship with the right and left keys.

You've got three lives. The goal is to reach maximum possible speed.

Avoid collisions with asteroids. The faster you travel the faster they appear.


Your record will be displayed on screen after no more lives are left.

<img src= "https://github.com/cmulation/Space-flight-mini-game/blob/master/Capture1.JPG" width="300" height="300"/>
<img src= "https://github.com/cmulation/Space-flight-mini-game/blob/master/Capture2.JPG" />

<b>Additional info</b>

Four different trajectories have been created for the asteroids to move along using vectors.

A variable “float fside=random(0,4);” generates a random number from 0 to 3

and then passes the value to “side”: “side=int(fside);”. This tells the asteroid

which trajectory to use. Each trajectory uses three vectors, so the corners of an image

can be guided along these lines. Asteroid sprite increases in size as it moves along a trajectory.
This was achieved by guiding the four points of the asteroid image along the trajectory lines,
which spread out near the edges of the screen. This helped create the illusion of depth.

<img src= "https://github.com/cmulation/Space-flight-mini-game/blob/master/vectors.png" width="300" height="300"/>
-----------------------------------------------------------------------------------------

Spaceship movement is calculated by using trigonometric functions:
spaceship_x = 220 * sin(angle) + OriginX;
spaceship_y = 240 * cos(angle) + OriginY;
It moves in a semi-circle to help create perspective. Left and right keys control
spaceship’s movement.

![movement](https://github.com/cmulation/Space-flight-mini-game/blob/master/movement.png)

<b>CREDITS AND USED RESOURCES:</b>

Credit to Frederik Rogalski (openprocessing) https://www.openprocessing.org/sketch/445916

Credit to Alex Samuel (openprocessing) http://www.openprocessing.org/sketch/66950

General queries and information: https://processing.org; https://forum.processing.org/two/

Impact sound effect: http://soundbible.com/346-Metal-Impact-Hollow.html

Mouse click sound effect: http: http://noisefx.ru/skachat-zvuki-klika-myshi.html

Spaceship sound effect: https://www.soundjay.com/propeller-plane-sound-effect.html

Main music theme: Tales - Endless Spaces

All images used in this game created by Mariia Skyba
