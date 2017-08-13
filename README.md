# CubeWorldAR

CubeWorldAR is an augmented reality game made with Unity and Vuforia. The game is placed inside a cube and the basic idea is that the user can look inside the cube only through one side at a time. The user can move the game character only to the left or to the right on the axis parallel to side of the cube through which the user is currently looking into the cube.

## Game Idea

The game takes place inside a cube sitting on top of an image tracker. The AR library tracks the position of this image tracker and places the game world (the cube) onto the tracker and therefore into the real world. The user can only look into the cube through one side of the cube at one time. The sides of the cubes are not transparent by default, but get transparent if the camera (the mobile device) is pointed at it.

The player controls the game character by moving it on the horizontal and vertical axis (viewed from above) and letting it jump. The character can only move along one of the axis at a time, and only parallel the axis. The axis the character can move along is also determined by the camera (the mobile device). The character can only move along the axis that is most parallel to the camera view. 

<img src="/img/Screenshot_1.jpg" width="60%">

The image shows the game cube with the first level inside. The light blue cylinder is the character, the light green sphere is the finish and the other objects are obstacles. The camera facing side of the cube is transparent. The character can only move along the axis parallel to the camera (A), and not along the other Axis (B) or diagonal.

The goal of the game is to reach the destination/finish of each level. All objects inside the game world with exception of the goal indicator (the sphere) are affected by gravity. The yellow obstacles can be moved by the character.


## Implementation
Untiy (https://unity3d.com/) is used as game engine to create the game. Vuforia (https://www.vuforia.com/) is used as tracking library. The library recognizes and tracks a defined image in the real world and uses it to place the coordinate origin of the game world into the real world.


<img src="/img/Screenshot_2.jpg" width="60%">
