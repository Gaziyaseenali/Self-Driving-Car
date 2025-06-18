                             Vision-Based Self-Driving Car Simulation
A deep learning-based self-driving car prototype developed in a simulated environment using behavioral cloning and convolutional neural networks (CNNs). The project focuses on lane navigation and obstacle avoidance using visual inputs from the vehicle's front-facing camera.

Project Overview:
This project demonstrates a vision-based autonomous driving system built and tested in Udacity and CARLA simulators. It utilizes end-to-end learning through a CNN model trained on human driving behavior to predict steering commands in real time.

Objectives:
Develop an autonomous vehicle that navigates lanes using camera input.
Implement behavioral cloning using a CNN-based architecture.
Achieve real-time inference performance suitable for deployment in simulation.
Test and evaluate the model under diverse driving scenarios and conditions.

Model Architecture:
The model is inspired by NVIDIA’s end-to-end architecture and includes:
5 Convolutional layers
Flattening and fully connected dense layers

Output: single continuous steering angle prediction

Input:
200x66 RGB images (preprocessed and normalized)

Output:
Predicted steering angle

Data Collection & Augmentation:
Driving data recorded using the Udacity simulator (steering angle, throttle, brake, speed, and images).
Augmentation techniques:
Random brightness
Horizontal flipping
Shadow overlay
Normalization

Performance:
Lane deviation: ±0.25 meters
Route completion: 92% without intervention
Real-time inference: 25 FPS
Evaluation based on lane accuracy, collision count, and completion rate.

Tech Stack:
Python
TensorFlow / Keras
OpenCV
NumPy
Udacity Simulator
