# Emotion-based music recommendation system

This Python-based web application leverages OpenCV to detect and analyze user emotions in real-time. The workflow is as follows:

Emotion Detection and Image Cropping:

The app captures a video frame using OpenCV and isolates the user's face by cropping the detected region of interest (ROI).
The cropped face image is passed to a pre-trained machine learning model for emotion prediction.
Rapid Iterative Predictions:

Over a period of 2-3 seconds, the app processes 30-40 frames, generating a list of predicted emotions.
Emotion Frequency Analysis:

The resulting emotion list is sorted by frequency.
Duplicates are removed to create a distinct, frequency-ranked emotion list.
Emotion-Based Content Recommendation:

Songs or other content are recommended sequentially based on the sorted emotion list, ensuring the user's most prominent emotions are prioritized.
This app seamlessly blends computer vision, machine learning, and real-time emotion analysis to deliver personalized, emotion-driven content recommendations.

## Installation & Run

Create a new project in Pycharm and add the above files. After that open the terminal and run the following command. This will install all the modules needed to run this app. 

```bash
  pip install -r requirements.txt
```

To run the app, type the following command in the terminal. 
```bash
  streamlit run app.py
```
