# Vigil Drive OpenCV Project

## Overview
The Vigil Drive OpenCV Project is designed to enhance vehicle safety through real-time monitoring and detection using computer vision techniques. This project utilizes OpenCV to implement various safety features, ensuring a safer driving experience.

## Features
- **Real-Time Monitoring**: Monitors the driving environment in real time.
- **Object Detection**: Identifies and classifies various objects around the vehicle.
- **Alert System**: Notifies drivers of potential hazards and unsafe conditions.

## Functionality

**Live Camera Detection**:
- Click "Live Cam Detection" to access the live camera feed.
- Press 'q' to exit.

**Video Input**:
- Select a video file using the "Video Input" button.
- Press 'q' to stop playback.
  
**Image Input**: 
- Use "Image Input" to select an image file.
- Note: This feature is partially implemented; complete the code in the `image_input` function.

**Model Loading**: 
- Load your pre-trained PyTorch model with:
  
  ```python
  model = torch.load(r"your_model_path.pt")
  model.eval()
  ```

## Requirements
This is the requirements for the tkinter application
- Python 3.x
- OpenCV
- PyTorch

install the required libraries using the following command

```bash
pip install opencv-python torch
```


## Installation

To run this project, you must install the required packages and dependencies. Follow the below steps :

1. Start by cloning the repository ans installing required packages:
   
   ```bash
   git clone https://github.com/lakshanika/Vigil-Drive-OpenCV-project.git
   cd Vigil-Drive-OpenCV-project
   pip install -r requirements.txt
   ```

2. Install Python packages, YOLOv8
   ```bash
   !pip install IPython
   !pip install ultralytics==8.0.100
    ```

3. Install roboflow
   ```bash
   !pip install roboflow
   ```
   
4. Set up roboflow to access the dataset:
   ```bash
   from roboflow import Roboflow
   rf = Roboflow(api_key="mfT0nNfmxVjhUNyuOOqF")
   project = rf.workspace("shiv-nadar-university-kkpwx").project("mobile-seatbelt-drowsy")
   dataset = project.version(1).download("yolov8")
   ```
       

## Note

Ensure the required libraries are installed before running the script. Update the model file path to your trained PyTorch model. Note that image input functionality is incomplete; you'll need to add the code in the `image_input` function. Feel free to replace the placeholders and modify any sections to better fit your project!

