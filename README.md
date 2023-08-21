# Emotion_detection_with_CNN

![emotion_detection](https://github.com/datamagic2020/Emotion_detection_with_CNN/blob/main/emoition_detection.png)

This project aims to detect human emotions using Convolutional Neural Networks (CNN). The emotion detection model is trained on the FER2013 dataset and can recognize seven different emotions: Angry, Disgusted, Fearful, Happy, Neutral, Sad, and Surprised.

## Prerequisites

Make sure you have the following packages installed:

```bash
pip install numpy
pip install opencv-python
pip install keras
pip3 install --upgrade tensorflow
pip install pillow
```

## Dataset
Download the FER2013 dataset from the link below and place it in the data folder under your project directory:
- https://www.kaggle.com/msambare/fer2013

## Training the Emotion Detector
Train the emotion detector with all face expression images in the FER2013 Dataset using the following command:
```bash
python TrainEmotionDetector.py
```
Note: Training may take several hours depending on your processor. (On an i7 processor with 16 GB RAM, it may take around 4 hours.)

After training, the trained model structure and weights will be stored in your project directory as emotion_model.json and emotion_model.h5.

Copy these two files and create a model folder in your project directory, then paste them inside.

## Testing the Emotion Detector
Run your emotion detection test file using:

### run your emotion detection test file
```bash
python TestEmotionDetector.py
```
This script uses the trained model to perform emotion detection on test images, generating a confusion matrix and classification report.
