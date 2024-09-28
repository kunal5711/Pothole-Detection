# Pothole Detection using YOLOv8

This project uses a YOLOv8 model to detect potholes in video frames. The model is trained on a custom-labeled dataset and predicts potholes in real-time, drawing bounding boxes around the detections and displaying confidence scores.

## Project Overview

- **Data Labeling**: The video frames were labeled using Roboflow, and the dataset was exported in YOLO format.
- **Model Training**: The YOLOv8 model was trained on the labeled dataset using Google Colab, with the final model saved as `best.pt`.
- **Real-Time Detection**: The trained model is used to process video frames, detect potholes, and display the results with bounding boxes and confidence scores.

## Requirements

To run the project, you'll need the following Python packages:

```bash
opencv-python
matplotlib
ipython
ultralytics
```

You can install them using:
```
pip install -r requirements.txt
```

## How to Run the Project
1. Clone the repository:
   ```
   git clone https://github.com/yourusername/pothole-detection.git
   cd pothole-detection
   ```

2. Download the trained model (best.pt) and place it in the appropriate folder.
3. Make sure to update the paths for the model and video file in the script:
  ```
  model = YOLO(r"your_path_to_best.pt")
  cap = cv2.VideoCapture(r"your_path_to_video.mp4")
  ```
