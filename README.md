# autonomous-smart-car

In this project, I have made an automatic self-driving car that is capable of lane detection and obstacle avoidance.

Hardware component used in the project is followed as:
1. Raspberry pi
2. L298N moter module
3. pi cam
4. ultrasonic sensor
5. robot chassis

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

My project is capable of detecting lanes with the help of a Pi camera and OpenCV through the Hough Transform, sending a signal, and taking the turn according to the direction of the curve.


############OBSTACLE AVOIDANCE############

Also, with the help of an ultrasonic sensor, we are detecting objects coming in front of us and giving the command to stop the vehicles whenever a 15-cm-long object is detected by the sensor and the vehicles stop.


This is the first part of the project; I further plan to improve it to project more by:
1. Improving obstacle avoidance code
2. Integrating and gsp module to track the car and its safety.
3. Try to apply CNN for lane detection
4. traffic light responding
