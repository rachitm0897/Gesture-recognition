# Gesture Recognition Using MediaPipe and Hand Landmarks Detection

This repository contains code for real-time gesture recognition using MediaPipe and basic hand landmarks detection. The approach relies on calculating distances between selected keypoints, which have been identified as a reliable subset of the landmarks provided by MediaPipe's hand detection model. These distances are then saved and normalized based on a specific distance between two chosen landmarks.

# Methodology
Landmark Detection: The code uses MediaPipe to detect hand landmarks in real-time video frames. The detected landmarks are represented as keypoints on the hand.

Distance Calculation: Distances between specific pairs of landmarks are calculated. The selection of these pairs is based on extensive testing to identify the most effective subset for gesture recognition.

Distance Normalization: To make the gesture recognition invariant to different hand sizes, the calculated distances are normalized using a reference distance between two landmarks.

Gesture Recognition: In the evaluation part, the code compares the calculated distances with predefined values for known gestures. The recognition process involves checking the differences between the known distances and the unknown distances calculated for the detected hand. This method results in real-time gesture recognition with minimal latency.

# Results
This approach to gesture recognition offers real-time performance with low latency. It has been optimized for accuracy and can be easily extended to recognize custom gestures or adapted for various applications such as sign language recognition or human-computer interaction.

# Acknowledgments
This code is made possible by the MediaPipe library developed by Google. Special thanks to the open-source community for contributions and resources.
