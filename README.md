## Facial_Emotion_Recognition
This project implements a real-time emotion recognition system using computer vision and deep learning techniques. It leverages OpenCV for video capture and face detection, along with the DeepFace library for emotion analysis. The system identifies and classifies emotions expressed by individuals captured through a webcam.This project focuses on real-time facial emotion detection utilizing the DeepFace library in conjunction with OpenCV. It captures live video from the webcam, identifies faces, and predicts the emotions displayed on each face. The detected emotions are overlaid on the video frames in real time, creating an interactive experience for monitoring emotional expressions. This implementation stands out as a streamlined solution for emotion recognition in real-time scenarios, showcasing my skills in computer vision and deep learning.


Created with PK SANGAMESWAR

Dependencies
DeepFace: A powerful deep learning library designed for facial analysis, offering pre-trained models for emotion detection and relying on TensorFlow for computational tasks.
OpenCV: A robust open-source library for computer vision, widely used for image and video processing tasks.

## USAGE
# Initial Steps

Git clone this repository Run: git clone https://github.com/SANGU1010/Facial_Emotion_Recognition.git
Run: cd Facial-Emotion-Recognition-using-OpenCV-and-Deepface
Install the required dependencies:

You can use pip install -r requirements.txt
Or you can install dependencies individually:
*pip install deepface*
*pip install tf_keras*
*pip install opencv-python*
Download the Haar cascade XML file for face detection
Run the code.
Execute the Python script.
The webcam will open, and real-time facial emotion detection will start.
Emotion labels will be displayed on the frames around detected faces.


## Approach
Import the necessary libraries: cv2 for video capture and image processing, and deepface for the emotion detection model.

Load the Haar cascade classifier XML file for face detection using cv2.CascadeClassifier().

Start capturing video from the default webcam using cv2.VideoCapture().

Enter a continuous loop to process each frame of the captured video.

Convert each frame to grayscale using cv2.cvtColor().

Detect faces in the grayscale frame using face_cascade.detectMultiScale().

For each detected face, extract the face ROI (Region of Interest).

Preprocess the face image for emotion detection using the deepface library's built-in preprocessing function.

Make predictions for the emotions using the pre-trained emotion detection model provided by the deepface library.

Retrieve the index of the predicted emotion and map it to the corresponding emotion label.

Draw a rectangle around the detected face and label it with the predicted emotion using cv2.rectangle() and cv2.putText().

Display the resulting frame with the labeled emotion using cv2.imshow().

If the 'q' key is pressed, exit the loop.

Release the video capture and close all windows using cap.release() and cv2.destroyAllWindows().
