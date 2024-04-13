# Head Pose Estimation
### <br>Supervised Machine Learning Regression Model</br>
The main objective of this model is to find the relative orientation (and position) of the human’s head using 2d face landmarks extracted using mediapipe library. In particular, in the head pose estimation task, it is common to predict relative orientation with Euler angles – yaw, pitch and roll. They define the object’s rotation in a 3D environment.
<p align="center">
    <img width="700" src="https://user-images.githubusercontent.com/97121850/221661146-b65ead74-749b-4ac0-8262-e3b55b0dc400.jpg">
</p>

# Demo
https://user-images.githubusercontent.com/97121850/221677815-bdb167f6-761a-4e0c-ad2c-c1e01a6aacfb.mp4

# Dataset
For this project, the dataset used is AFLW2000 Dataset, which consists of 2000 face images, with some information about them like the facial landmarks and the pitch, yaw, and roll values for each picture.

# Solution
1. Used the MediaPipe library to extract the face landmark, consisting of 468 points representing 2D landmarks .
2. Performed preprocessing step to make the model independent of the face position or scale.
3. Trained a regression model using the facial landmarks to estimate the values of the pitch, yaw, and roll.
4. Used rotation, translation, and projection of the axes on the image to visualize the direction the person is looking at.
5. Used the values of pitch, yaw, and roll to define the direction.

# Libraries used
1. MediaPipe
2. Numpy
3. OpenCV
4. Scikit-Learn
