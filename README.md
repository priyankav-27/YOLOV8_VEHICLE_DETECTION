# YOLOv8 Custom Object Detection Project

## Overview

This project uses a pre-trained YOLOv8 model to perform object detection on a video file, focusing on specific classes such as ambulances, cars, trucks, buses, and motorcycles. The model processes each frame of the video and counts the occurrences of these objects while also displaying bounding boxes around detected objects.

## Features

- Real-time object detection on video files
- Custom YOLOv8 model integration
- Object counting for specific classes
- Display of detected objects with bounding boxes and confidence scores

## Requirements

- Python 3.x
- [YOLOv8](https://github.com/ultralytics/ultralytics) by Ultralytics
- OpenCV for video processing
- NumPy for numerical operations

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/YOLOv8-custom-detection.git
   cd YOLOv8-custom-detection
2.**Install the required packages:**

  ```bash
  pip install ultralytics opencv-python numpy
  ```
3.**Download your custom YOLOv8 model:**

  - Replace custom_yolo_model.pt in the script with the path to your model file.
    
## Usage

1.**Prepare your video file:**

  - Place your video file in the project directory or provide the correct path to it in the script.
    
2.**Run the script:**

  ```bash
  python yolo_custom_detection.py
  ```
3.**Modify the detection classes (optional):**

  - If you need to detect different objects, update the object_counts dictionary in the script with your desired classes.
  
4.**View the results:**

  - The script will display frames with detected objects and print the final counts of each object at the end of the video.

## Example Output

- The model processes each frame of the video, detecting objects and drawing bounding boxes around them.
- A final count of detected objects (e.g., ambulances, cars, trucks) is printed to the console.
  
## Customization

- Classes: Modify the object_counts dictionary and update the model's class names to reflect the specific objects you want to detect.
- Model: You can replace the custom_yolo_model.pt with any other YOLO model trained on different datasets.
