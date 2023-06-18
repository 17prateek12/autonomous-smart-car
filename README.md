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
block diagram

![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/b9d2f937-34fd-466a-ade6-cb69f267cfa0)
working model of car

![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/eac09cf7-045a-43e3-b5f8-cf84d8d52e62)
finaal circuit diagram

#########COMPARISON BETWEEN HOUGH TRANSFORM AND CNN##########
The results of both algorithms in the following cases have been shown in the given table. The result has been given by pass or fail, and accuracy has been found on the basis of the number of pass cases versus the total number of cases.
 
![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/f1f65d4e-a203-43eb-803c-60d54d73b7d2)
![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/ce54b431-a7b6-49f6-b374-ed02d16134fe)
![image](https://github.com/17prateek12/autonomous-smart-car/assets/88935432/ca272f1f-a989-4f22-8db5-8bba1e76fc9b)

Table 1: Comparative analysis between Hough transform and Convolutional neural network


########CONCLUSION########
As per the given data, we can see that CNN is working better in some situations due to the Hough transform. Both algorithms have failed on multiple cross-sectional roads. As per computing accuracy based on the number of pass-test cases. We can say that CNN has an accuracy of 77.77 percent, whereas Transform has an accuracy of 55.55 percent. But if we exclude the multiple-lane scenario where we tried all possible conditions but didn't get any success and focused only on single-lane scenarios, we found that CNN gave 100 percent accuracy whereas Hough Transform gave an accuracy of 71.42 percent as it was not able to detect two cases properly, one where lanes are broken in between and another where multiple lanes are running parallel to each other. Hence, we can say that CNN works better in single-lane scenario rather than through transform.
	 






