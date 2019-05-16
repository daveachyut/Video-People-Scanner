# Video-People-ScannerAI based Surveillance Counter

Abstract—Most of the research done in the extent of counting a large number of people has inadvertently underlined the fact that the task, to detect and count people, still continues to be painstaking. This project presents a solution wherein getting a headcount of crowd will no longer need people to strain their vision; requires two steps: Detection and Tracking.

I. INTRODUCTION

Artificial Intelligence has emerged as a great futuristic domain,whose many chapters are yet to be disclosed. One of the intriguing chapter is Face Detection and Face Tracking. Keeping the exact count of people at any given time within any large premise is ideally very difficult to do. Monitoring, detection, tracking and Counting of people with the help of the same CCTV footage can be an added advantage to the already existing technology.

The aim of this project is to design an application, the main purpose of which is to count the number of people entering and leaving any
premises, involving cutting edge technologies such as Artificial Intelligence and Deep Learning, thereby getting increased efficiency in the desired results. The faces are tracked across simultaneous frames and the count of people is displayed in a specific amount of time.

II. LITERATURE REVIEW

For many businesses, one of the most important basic metrics is traffic; how many people came through the door.

The people-counting system can be widely used for tasks such as video surveillance, security, statistical analysis of people accessing an area, and other value added services.

1. 1st generation: Infrared beam counters (2002)

This is a single, horizontal infrared beam across an entrance. Since a person normally enters and leaves by the same door, dividing the count by two gives a measure of people. Even though it has many disadvantages infrared counters are still widely used due to being cheap and simple.

2. 2nd generation: Thermal counters (2005)

Thermal Counters use array sensors that detect heat sources. Thermal people counters are a popular choice in some situations due to following reason:

● Patterns on flooring that may disrupt optical sensors do not affect thermal sensors.

Various limitations of thermal counters:

● Thermal counters cannot be mounted on a high ceiling without using a narrow-angle lens.

● Accuracy is reduced in places with variations in thermal conditions.

3. 3rd generation: Video and WiFi counting (2012)

● Wifi counting functionality collects WiFi probe request signals from shoppers' smartphones, including outside the store.

III. PROPOSED SYSTEM

Firstly, using the existing security system for traffic counting eliminates the need for additional hardware on the back end. Second, traffic count data is captured in the security system control panel and can be accessed using the existing interfaces or applications. 

The counter requires two steps: detection and tracking. Finally, the system updates the counters based on the direction of the trajectories.

Further problematic situations, such as occlusions, people grouped in different ways, scene luminance changes, etc., were used by Jorge, et al. to validate the performance of the system.

The software application makes use of Python 3.6 programming and OpenCV 3.1 library to process the live CCTV footage. The reasons for using Python are its compatibility with Artificial Intelligence systems and features such as object oriented programming and large comprehensive standard library. The algorithm used for face detection is Haar Cascade Algorithm and the detection itself is unsupervised.

Input to the program are test images, which are then converted into their respective grayscale images by color image processing.

Increased accuracy in face detection can be provided by the Haar Cascade algorithm due to its features such as high robustness and the fact that the algorithm is adept in distinguishing faces from non-faces. Face tracking requires the location and size of human faces in an image. Face tracking often uses machine learning (ML) algorithms to keep track of human faces after face detection is already performed in previous frame of the video.

The rectangular box is labeled Person X, where X is the tracker ID assigned to every face, which changes, after performing the most difficult part, that is, comparison of consecutive frames of video in real time.

The centre point of tracker must lie in the region of face detected.

Deciding the frame rate for the input frames which indeed will depend on the type and model of CCTV whose frame per seconds differ.

The face detection uses the Haar Cascade Classifiers for accurate face detection. These may obviously vary from person to person but the outline of every feature remains the same. Now if a face gets out of a corresponding frame then a new tracker gets assigned to the face, in this way the number of people coming into the frame and going out of the frame can be monitored. There is constant updation of the tracker which ignores the earlier one and ascribe the new coordinates to the new face. The output device can be a LCD display linked to
the CCTV or just a machine which is protected and used by the officials only.

IV. RESULT AND ANALYSIS

The system is trained to operate with various ambiguities like person wearing a cap or spectacles. The system was tested under various lighting conditions and it was found that adequate amount of lighting is required for successful detection of faces.

Advantages
1. High Detection Accuracy- 90-95%.
2. Low false positive rate- Detection of a non-face is very less.

Disadvantages
1. Computationally complex and slow- Processing time increases with more number of faces.
2. Limitation in difficult lighting conditions.

V .CONCLUSION

This project presents a customized approach for face detection for real time video capture and processing using Haar Cascade algorithm. The proposed system was designed to be implemented in apartments, offices, museums, colleges, theatres. The system can be enhanced to perform recognition and associated application such as Biometric recognition system, voter verification and access control.

VI. REFERENCES

1. “Python OpenCV: Face detection and counting” [Online]. Available: https://techtutorialsx.com/2017/05/02/pythonopencv-face-detection-and-counting/amp/
2. “An Introduction to Python” [Online]. Available: http://www.tulane.edu/~howard/NLP/python.html
3. “Face detection using OpenCv and Python.”[Online]. Available: https://www.superdatascience.com/opencvface-detection/
