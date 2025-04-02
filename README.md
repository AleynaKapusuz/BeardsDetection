# BeardsDetection

![Image](https://github.com/user-attachments/assets/2fa1a6f9-6c5f-4143-97d6-99a8c2d3b053)


📝 Project Description:
This project uses YOLOv8 (You Only Look Once) for real-time whisker detection in videos. The model was trained on a custom dataset and is used to track and visualize whiskers in video frames.

🛠️ Key Features:
Whisker Detection with YOLOv8:
The project leverages YOLOv8, a state-of-the-art object detection model, to detect and track whiskers in video footage. It is optimized for fast and accurate detection, making it suitable for real-time applications.

Model Training:
The model was trained using a custom dataset for whisker detection, and the weights are stored in best.pt.

Real-Time Video Processing:
The code captures frames from a given video and applies YOLOv8 to detect whiskers in each frame. Annotations (bounding boxes) are drawn around detected whiskers for visualization.

Video Output:
After processing the video, the detected whiskers are visualized in each frame with bounding boxes and class labels. You can easily use this framework for other object detection tasks by swapping the model and dataset.

🚀 How It Works:
Model Loading:
The YOLOv8 model is loaded from the specified weights file (best.pt).

Video Capture:
The video is read frame by frame using OpenCV (cv2.VideoCapture). For each frame, YOLOv8 processes the image to detect whiskers.

Tracking & Annotation:
YOLOv8 tracks objects across frames and annotates the detected whiskers with bounding boxes and confidence scores.

Real-Time Display:
The processed frames are displayed in real-time, showing the detected whiskers.

Quit Functionality:
Press the "q" key to exit the video display.

📥 Prerequisites:
To run this project, Install the necessary libraries using:
```
pip install opencv-python ultralytics
```

⚙️ Usage:
To use the script, update the paths to your trained model and video file:

```
model = YOLO("models/best.pt")
cap = cv2.VideoCapture("path_to_your_video.mp4")
```

Run the script, and the video will be processed with whisker detection.

You can download the model from:

`models/best.pt`


## Beard detection code output: 

![Image](https://github.com/user-attachments/assets/612a1274-e43d-4841-99f8-9be154b0c56a)

and video : 

[https://github.com/user-attachments/assets/f749b386-b871-45df-8873-078bc51dd9ae](https://github.com/user-attachments/assets/411de064-957f-47db-aeb8-4280554fc871)
