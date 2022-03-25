# Motion Compensated Pulse Rate Estimation

This project has 2 main parts.

1. Develop a Pulse Rate Algorithm on the given training data.
2. Apply the Pulse Rate Algorithm on a Clinical Application and compute more clinically meaningful features and discover healthcare trends.

<b> Introduction </b> </br>
A core feature that many users expect from their wearable devices is pulse rate estimation. Continuous pulse rate estimation can be informative for many aspects of a wearer's health. Pulse rate during exercise can be a measure of workout intensity and resting heart rate is sometimes used as an overall measure of cardiovascular fitness. In this project I created a pulse rate estimation algorithm for a wrist-wearable device. 


<b> Part 1: Pulse Rate Algorithm Project Overview </b> </br>
My algorithm:
<li> estimates pulse rate from the PPG signal and a 3-axis accelerometer </li>
<li> produces an estimation confidence </li>
<li> produces an output every 2 seconds </li>
</br>
My algorithm performance success criteria are as follows: the mean absolute error at 90% availability is be less than 15 BPM on the test set. Put another way, the best 90% of my estimates--according to my own confidence output-- have a mean absolute error of less than 15 BPM.
