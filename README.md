# Vehicle Lane Invasion Detection Based on Computer Vision Algorithms
## By Victor Enrique Gil Altamirano
## Supervised by Prof. Guo Ling, PhD.

# Summary
Transportation has become a major driver for society’s development, moving people and goods from one place to another plays a significant role in growth and welfare. The amount of time we spent in vehicles is increasing, and distances we drive are continuously furthering the limits. Naturally, conveyance necessities have led to a larger quantity of public and private vehicles. Unfortunately, the increase of vehicles warns a greater risk of accidents as well. Majority of car accidents are caused by driver’s misconducts, rather than vehicle’s malfunction, predominantly by lane-merging maneuvers. Advanced Driving Assistance Systems are designed to minimize fatalities and prevent safety issues.
This work proposes a driving assistance system capable of detecting when a neighboring vehicle maneuvers towards a forbidden lane with capabilities of executing in real-time. The system is composed by four main phases which are lane identification, vehicle detection, car plate recognition, and lane invasion detection.

The proposed method was tested using primary data using miniature vehicles running on a dedicated hardware consisting of a treadmill with a fixed video camera aiming at neighboring vehicles emulating driver’s field of view. Sample consisted on ten miniature vehicles of different size captured in ten respective footages at 30fps with a resolution of 1920x1080 pixels in 3-channels RGB frames. Lane markings alternated between solid and dashed where miniature vehicles were arbitrarily changing lane while running. On the software side, the system was written entirely in Python adapted to execute on the Robot Operating System (ROS) framework, given the modular ecosystem of ROS, each phase corresponds to a node. Additionally, in order to test the portability across devices, the system was tested in two different platforms, namely, a commercial Laptop computer running Linux in a virtual machine, and an OrangePi Single Board Computer running native Linux. 

Lane line identification phase isolates the specific region located in the near distance of the ego-driver with a trapezoidal shape. Results reported an average accuracy of 95.6% and 94.9% for the algorithm running on Laptop and OrangePi respectively. Lane identification phase executed at 28.22ms and 38.67ms respectively. Compared with related work, accuracy and processing time similarity were consistent. Similarly, Vehicle detection phase isolated the road region corresponding to neighboring vehicles shaped as trapezoid covering the complete road ahead of ego-driver. A first Haar Cascade filter examines the complete region of interest looking for a vehicle due to its high speed. To overcome the high false detection rate intrinsic in Haar Cascades, a second filter was implemented involving a Convolutional Neural Network which determined whether the Haar Cascade detected object was in fact a vehicle or not. Overall accuracy reported to average 85% on vehicle detection, whereas processing time was consistent with related works. Car plate recognition phase used a telescopic approach by first detecting a vehicle, and then locating the car plate pattern in the vehicle. Localization of car plate was achieved by using a Haar Cascade filter, whose region was isolated to perform optical character recognition. Successful car plate recognition for medium-sized vehicles reported an average accuracy of 68.5% above the mean compared with related works. It was reported that the ideal size for car plate recognition using Tesseract in Python was 200x100 pixels. This phase was reported to take the longest processing time, averaging 250.17ms and 407.77ms for Laptop and OrangePi respectively. Lastly, lane invasion detection phase uses a minimalist approach known as point-vs-rectangle, where the geometric center location of the bounded vehicle is compared with the lane equation computed for the lane line marking. Minimalist approach resulted with a 100% accuracy leaving room for further research such as lane invasion prediction before the maneuver is executed by computing the location points of the neighbor vehicle. 

The modular flexibility and cross-platform portability are just few of the many advantages ROS offers. The proposed system stablishes the foundation for a more elaborate project involving self-driving technology, as lane identification and vehicle detection are crucial for autonomous driving.

__*Keywords: Advanced Driving Assistant System, Computer Vision, Lane Invasion Detection, Robot Operating System.*__




# Under Construction...
Video coming soon...
