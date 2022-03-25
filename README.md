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
My algorithm performance: the mean absolute error at 90% availability is be less than 15 BPM on the test set. Put another way, the best 90% of my estimates--according to my own confidence output-- have a mean absolute error of less than 15 BPM.

</br>
</br>

<b> Dataset </b> </br>
I used the Troika dataset to build my algorithm. 

Zhilin Zhang, Zhouyue Pi, Benyuan Liu, ‘‘TROIKA: A General Framework for Heart Rate Monitoring Using Wrist-Type Photoplethysmographic Signals During Intensive Physical Exercise,’’IEEE Trans. on Biomedical Engineering, vol. 62, no. 2, pp. 522-531, February 2015

</br>


<b> Part 2: Clinical Application </b> </br>
After that I used my pulse rate algorithm to compute more clinically meaningful features and discover healthcare trends.

Specifically, I used 24 hours of heart rate data from 1500 samples to try to validate the well-known trend that average resting heart rate increases up until middle age and then decreases into old age. I also saw if resting heart rates are higher for women than men. 


<b> Dataset (CAST) </b> </br>
The data from this project comes from the Cardiac Arrhythmia Suppression Trial (CAST), which was sponsored by the National Heart, Lung, and Blood Institute (NHLBI). CAST collected 24 hours of heart rate data from ECGs from people who have had a myocardial infarction (MI) within the past two years.[1] This data has been smoothed and resampled to more closely resemble PPG-derived pulse rate data from a wrist wearable.[2]

[1] CAST RR Interval Sub-Study Database Citation - Stein PK, Domitrovich PP, Kleiger RE, Schechtman KB, Rottman JN. Clinical and demographic determinants of heart rate variability in patients post-myocardial infarction: insights from the Cardiac Arrhythmia Suppression Trial (CAST). Clin Cardiol 23(3):187-94; 2000 (Mar)

[2]Physionet Citation - Goldberger AL, Amaral LAN, Glass L, Hausdorff JM, Ivanov PCh, Mark RG, Mietus JE, Moody GB, Peng C-K, Stanley HE. PhysioBank, PhysioToolkit, and PhysioNet: Components of a New Research Resource for Complex Physiologic Signals (2003). Circulation. 101(23):e215-e220.


