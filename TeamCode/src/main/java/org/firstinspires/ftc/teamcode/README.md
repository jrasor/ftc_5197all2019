## Welcome!

This GitHub repository contains the source code that is used to build 
robot vision code for FTC Team 5197 "the GearHeads".
It is based on the FTC Software Development Kit (SDK), available at the
[FTC SDK repository](https://github.com/ftctechnh/ftc_app/releases).
        
Open it in Android Studio.

### Get This Project
To get our code, download or clone from 
[our repository](https://github.com/jrasor/2018vision).

This also was developed in Android Studio.

If you are new to the FIRST Tech Challenge software and control system, 
look at the [FTC SDK Wiki](https://github.com/ftctechnh/ftc_app/wiki).

Check back there from time to time, as it contains the most current 
information about the FIRST Tech Challenge software and control system.
### About This Project
Robot vision is very useful in FTC competition. Many recent games have included
recognition of images as part of some point scoring methods. These methods are
detailed in Game Manual Part 2. For the 2018 game "Rover Ruckus", that
was released at Kickoff on Sept. 8, 2018. This repository contains our
experience with vision methods beyond simple color sensors.

Robot vision methods we've used in the past:
- Vuforia
- OpenCV

Now we add
- TensorFlow lite

#### The Robot
The robot used by the GearHeads to test robot vision is the "Lookeebot", a
simplified version of the Pitsco-TETRIX Rangerbot. Its configuration and robot
class are based on the Pushbot class in the FtcRobotController external
samples. It has a drive train and a Robot Controller phone, but no servos
or sensors other than the phone camera. It's basically designed to run
around and look at stuff.

Much of the vision code in here can also run on other robots, like the
Trainerbots. The robot class Trainerbot is kept for that reason. Much of this
code can also run on a "nullbot", an empty configuration. In that scenario, 
hold the Robot Controller phone in your hand, put the Driver Station
phone on a table, and point the Robot Controller's camera at the things
you want the vision software to look at and process.

#### The Software
The software is this project. It is built up from sample opmodes taken from
the FtcRobotController samples that come with the SDK, and also with this
project. Software to support Vuforia and OpenCV has been added. Later versions
may add other robotic vision systems.