# autonomous-smart-car

In this project, I have made an automatic self-driving car that is capable of lane detection and obstacle avoidance.

Hardware component used in the project is followed as:
1. Raspberry pi
2. L298N moter module
3. pi cam
4. ultrasonic sensor
5. robot chassis
6. Neo 6m gps module

Software and Libraries used in the project is followed as:
1. Open Cv
2. Python 3
3. Raspbian OS

############REMOTE CONTROL############

With help from Python, we will be able to control our vehicle with the help of the keyboard.

In this module, I have basically created a remote control setup for the model. It contains a motor module, a keyboard module, and a final drive.

1# Motor module has set of command which define the direction for cars to take turn, and  speed for motors control.

2# In this keyboard module, I can give input from a keyboard and send it to our car. I have made the keyboard code modular, which means it will be a separate file that will send signals to our main robot code.

3# Final test drive, this module in integration of keyboard module and motor module, which will controlled the movement of car.


############LANE DETECTION############

My project is capable of detecting lanes with the help of a Pi camera and OpenCV through the Hough Transform, CNN, sending a signal, and taking the turn according to the direction of the curve. This part is basically a comparison between hough transform and CNN accuracy. 


############OBSTACLE AVOIDANCE############

Also, with the help of an ultrasonic sensor, we are detecting objects coming in front of us and giving the command to stop the vehicles whenever a 15-cm-long object is detected by the sensor and the vehicles stop and take turn accordingly.

############GPS############
Use neo 6m gps module with raspberry pi to track the live location of car.
![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/b58ff676-1171-4f76-b2fd-c463c4fecd4c)



