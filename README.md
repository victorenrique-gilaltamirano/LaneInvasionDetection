# Vehicle Lane Invasion Detection Based on Computer Vision Algorithms
## By Victor Enrique Gil Altamirano
## Supervised by Prof. Guo Ling.

Last update: February 3rd, 2023

# Abstract
Transportation, moving people and goods from one place to another, has become a major driver of social development. Unfortunately, the increase of vehicles introduces a greater risk of accidents as well. Majority of car accidents are caused by driver’s misconducts, rather than vehicle’s malfunction, predominantly by improper lane-merging maneuvers. Therefore, the development of an advanced driver assistance system based on lane intrusion detection can regulate the driver's behavior, thereby preventing the occurrence of dangerous driving behavior.
To solve the above problem, a real-time lane intrusion detection system has been designed and implemented, and then tested in two different platforms, namely, a commercial Laptop computer running Linux in a virtual machine, and an OrangePi Single Board Computer running native Linux. The main contribution of the work is as follows:
(1)	The design of a real-time lane intrusion detection system has been carried out, which includes four key stages: lane identification, vehicle detection and car plate reading and intrusion detection. The software development is based on Python language on the ROS robot operating system under Linux;
(2)	The system has been designed and implemented with recognition algorithms based on computer vision, including: lane recognition based on edge detection and Hough transform, car detection based on Haar cascade filter and convolutional neural network, license plate detection based on optical character recognition, and lane intrusion detection with Kalman filter, and the algorithms are optimized to reduce computational expenses;
(3)	A prototype system, consisting of vehicles with plated, lanes and other necessary elements, has been constructed to debug and test the software implemented in this thesis;
(4)	Experimental results and analysis: The overall system performs a smooth execution at 30 fps, resulting in an acceptable real-time implementation. Minimalist approach for lane intrusion detection has 100% accuracy, which is in accordance to related literature. Similarly, lane identification results have reported an accuracy similar to related works with a processing time faster than the average of consulted literature. Vehicle detection stage consisting of a double-check of cascade filter followed by a convolutional neural network in an isolated region of interest reports a faster processing time than the average of related works with a similar accuracy. On the other hand, car plate reading reported a slower processing time but slightly higher accuracy than average of related works. 




# Video

Video can be found in the following [BiliBili LINK](https://www.bilibili.com/video/BV1C84y1V7Zn/?share_source=copy_web&vd_source=bbb17cb22d3114d9ff90ccd72154a868) and
[YouTube LINK](https://youtu.be/vqVZS-TxeTM).


