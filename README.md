# HW5_Sigeay

Student: Ostanin Mike.
 
Variant D: Balancing a la segway with straight movement.

##Task description
Create Lego Robot and PID controller.

##Description of the work process:

I use oficial LEGO® MINDSTORMS® EV3 Software for program my robot.

For estimation the error I used angle value from Giro sensor.
I send a sum of current and previos error to integrater.
I used rotation rate from Giro sensor as differention.
Befor statirting the main loop of the program Gyro sensor is reseted.

### PID turig steps

1. Find the angle of vertical posotion. It is needed for calculation the error.
2. Find Kp.
3. Decrease osclation by changing Kd.
4. Add Ki for illumanation static error.
5. Optimization parameters.

## Results
The PID controller coefficients are folow: Kp=30, Kd=1, Ki=0.1.

Video: https://drive.google.com/file/d/0B6twz1PXaR8ISlM1bVJlaTNEclU/view?usp=sharing 

Lego Gyro sensor has some defects. First, descritization is a 1 degree, it is so big. Second, after some period of Gyro senser add angle value by it-self.

