# CarND-Controls-PID
Self-Driving Car Engineer Nanodegree Program

---

## Overview

Goal of the project is to builds a PID Controller which runs in Udacity [Simulator](https://github.com/udacity/self-driving-car-sim/releases).

## Prerequisites 

* cmake >= 3.5
 * All OSes: [click here for installation instructions](https://cmake.org/install/)
* make >= 4.1(mac, linux), 3.81(Windows)
  * Linux: make is installed by default on most Linux distros
  * Mac: [install Xcode command line tools to get make](https://developer.apple.com/xcode/features/)
  * Windows: [Click here for installation instructions](http://gnuwin32.sourceforge.net/packages/make.htm)
* gcc/g++ >= 5.4
  * Linux: gcc / g++ is installed by default on most Linux distros
  * Mac: same deal as make - [install Xcode command line tools]((https://developer.apple.com/xcode/features/)
  * Windows: recommend using [MinGW](http://www.mingw.org/)
* [uWebSockets](https://github.com/uWebSockets/uWebSockets)
  * Run either `./install-mac.sh` or `./install-ubuntu.sh`.
  * If you install from source, checkout to commit `e94b6e1`, i.e.
    ```
    git clone https://github.com/uWebSockets/uWebSockets 
    cd uWebSockets
    git checkout e94b6e1
    ```
    Some function signatures have changed in v0.14.x. See [this PR](https://github.com/udacity/CarND-MPC-Project/pull/3) for more details.
* Simulator. You can download these from the [project intro page](https://github.com/udacity/self-driving-car-sim/releases) in the classroom.



## Basic Build Instructions

1. Clone this repo.
2. Make a build directory: `mkdir build && cd build`
3. Compile: `cmake .. && make`
4. Run it: `./pid`. 

Tips for setting up your environment can be found [here](https://classroom.udacity.com/nanodegrees/nd013/parts/40f38239-66b6-46ec-ae68-03afd8a601c8/modules/0949fca6-b379-42af-a919-ee50aa304e6a/lessons/f758c44c-5e40-4e01-93b5-1a82aa4e044f/concepts/23d376c7-0195-4276-bdf0-e02f1f3c665d)




## PID Parameter 

The parameter were choosen manually by trail and error . the behaviour of the car for each of the parameter were analysed 

P parameter 

with only P parameter set the car started driving in the lane but oscillated highly [P_BehaviourVideo](./Video/P_set_PIDController.mp4)


I Parameter

Car started rotating when the I parameter is set alone [I_BehaviourVideo](./Video/I_set_PIDController.mp4)

D Parameter

Car started going straight with D parameter set  [D_BehaviourVideo](./Video/D_set_PIDController.mp4)

with the above behaviour the values were changed and a final value of P = 0.35, I =0.00001 , D = 4 was choosen

