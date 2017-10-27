# HW5_Sigeay

Student: Ostanin Mike.
 
Variant D: Balancing a la segway with straight movement.

## Task description
Create a Lego Robot and find thr best coefficients for pid controller of lego robot

## Description of the work process:

I used official LEGO® MINDSTORMS® EV3 Software for programming my robot.

For estimation the error I used angle value from Giro sensor.
I send a sum of current and previous error to integrate.
I used rotation rate from Giro sensor as the differentiator.
Before starting the main loop of the program Gyro sensor is reset.

#### PID turig steps

1. Find the angle of vertical position. It is needed for calculating the error.
2. Find Kp.
3. Decrease oscillation by changing Kd.
4. Add Ki for decrease static error.
5. Optimization parameters.

## Results
The PID controller coefficients are folow: Kp=30, Kd=1, Ki=0.1.

Video: https://drive.google.com/file/d/0B6twz1PXaR8ISlM1bVJlaTNEclU/view?usp=sharing 

Lego Gyro sensor has some defects. First, discretization is a 1 degree, it is so big. Second, after some period of Gyro sensor add angle value by itself.

