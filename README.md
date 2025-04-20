A real-time Human Emotion Detection System using computer vision and deep learning. This project captures live video from a webcam, detects faces, classifies emotional states (e.g., Happy, Sad, Angry, etc.), and optionally allows users to capture images and retrain the model on-the-fly through a user-friendly GUI.
Features:-
Real-time face detection using OpenCV
Emotion classification using a trained CNN model
GUI-based interface for ease of use
Live emotion prediction and display
Option to capture images and save them by emotion label
Real-time training using newly captured data
Voice and sound feedback (optional)
Programming Language: Python
Libraries: OpenCV, TensorFlow/Keras, NumPy, Tkinter, PIL, sklearn, etc.
Model: Convolutional Neural Network (CNN)
Dataset: FER-2013 / Custom-labeled dataset
STRUCTURE:-
EmotionDetection/
│
├── dataset/                  # Stored emotion-labeled images
│   ├── Happy/
│   ├── Sad/
│   └── ...
│
├── model/                    # Trained model file
│   └── emotion_model.h5
│
├── gui/                      # GUI implementation
│   └── app.py
│
├── utils/                    # Utility scripts (e.g., preprocessing, face detection)
│   └── face_utils.py
│
├── training/                 # Scripts for model training
│   └── train_model.py
│
├── requirements.txt          # List of dependencies
├── README.md
└── main.py                   # Entry point for the application
Install dependencies:-
pip install -r requirements.txt
How to Use:-
Start Detection: Opens webcam and begins real-time emotion prediction.
Capture Image: Saves current face frame to selected emotion folder.
Train Model: Retrains model using current dataset (including new captures).
Stop Detection: Stops the webcam feed.
To retrain the model with newly captured data:-
python training/train_model.py
This will update emotion_model.h5 using all images in the dataset/ folder.
Sample Output:-
Real-time webcam feed
Detected face with bounding box
Predicted emotion label displayed on top of the box


Pull requests are welcome. Feel free to suggest new features, raise issues, or contribute code.
