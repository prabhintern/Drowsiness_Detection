# Drowsiness_Detection
(Prototype Implementation) is for people who feel drowsy when driving which can lead to accidents.


Creating a drowsiness detection system using OpenCV, dlib, scipy.spatial, imutils, and pygame involves a series of detailed steps. The following outlines the methodology and implementation required to develop such a system effectively:

Overview
This system utilizes the in-built camera to monitor the user's eye movements and determine drowsiness by calculating the Euclidean distance between specific eye landmarks. If drowsiness is detected, an alert sound is played to wake the user.

Components and Workflow
Library Importation and Initialization:

Import the necessary libraries including OpenCV, dlib, pygame, scipy.spatial, and imutils.
Load dlib’s pre-trained facial landmark detector.
Initialize the video stream to capture live video from the in-built camera.
Facial Landmark Detection:

Detect faces within the video stream using dlib.
Extract the facial landmarks focusing particularly on the eyes.
Eye Aspect Ratio (EAR) Calculation:

Compute the Euclidean distances between vertical eye landmarks and horizontal eye landmarks.
The EAR is used to determine whether the eyes are closed or open.
Drowsiness Detection Algorithm:

If the EAR falls below a pre-defined threshold for a specified number of consecutive frames, the user is considered to be drowsy.
An alert sound is played using pygame to notify the user.
Real-time Video Processing:

Continuously process the video frames to monitor and detect drowsiness in real-time.


//Sample Photo//

![image](https://github.com/prabhintern/Drowsiness_Detection/assets/141141575/1d4a0efb-fb26-4ae4-84b5-bafc08b90905)


