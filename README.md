# Path Planning Project

## Abstract
This is a Udacity coursework project from Term 3 of the Self-driving Car Nanodegree program. The task is to make a path planner for the self-driving car to follow along while driving safely without breaking the law or causing any accident. You'll need the Udacity car simulator to run along with the code, which can be downloaded [here](https://github.com/udacity/self-driving-car-sim/releases/tag/T3_v1.2).

## Method
 In this project I use a simple finite state machine for the car to cope with several typical conditions where we normally would consider changing lanes, where two factors are put into account: how fast you're currently going, and is it safe to change lanes. I use a simple strategy that when the car is not going as fast as it could and it's safe to change lanes, then it'll change lanes. 

## Result
The car is able to change lanes safely while keeping a speed that's close to the speed limit whenever it can. The behavior of the car is rather simple considered that we're using a finite state machine here. So it is not optimal and definitely not nearly as smart as a human driver. This can be further improved using more complex cost functions to govern the car's behavior.

## How to use
1. Download the [simulator](https://github.com/udacity/self-driving-car-sim/releases/tag/T3_v1.2)
2. Clone this repo
3. Go to the `build` folder and build using `cmake .. && make`
4. Run the code with `./path_planning` 