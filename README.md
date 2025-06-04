# weapon-detection

# Real-Time Weapon Detection using YOLOv3 and OpenCV

This project implements a real-time weapon detection system using the YOLOv3 deep learning model and OpenCV. It identifies the presence of weapons in video streams or files and plays an alarm when a weapon is detected.

## Project Overview

- Uses YOLOv3 for object detection
- Triggers an audio alert when a weapon is detected
- Supports webcam or video file input
- Fast and real-time processing with OpenCV DNN module

## Files

- `WEAP DET.py`: Python script for running weapon detection and alarm system
- `yolov3.cfg`, `yolov3_training_2000.weights`: YOLOv3 configuration and trained weights files
- `mixkit-alert-alarm-1005.wav`: Alarm sound file (make sure it's available at the specified path)

##  How It Works

1. Load the YOLOv3 model with trained weights and config
2. Accept input from webcam or a video file
3. Detect objects in each frame and classify them
4. If a "Weapon" class is detected, trigger an alarm sound

## Requirements

Install the following packages:

```bash
pip install opencv-python numpy playsound
```

##  How to Run

1. Make sure you have `yolov3.cfg`, `yolov3_training_2000.weights`, and the alarm `.wav` file in the correct paths
2. Run the script:

```bash
python "WEAP DET.py"
```

3. When prompted:
   - Press `Enter` to use webcam
   - Or enter a video file name (e.g., `video.mp4`) to use as input

4. Press `q` to exit the application

## Output

- Detected weapons are highlighted in real time
- An alert sound is played upon detection

## Note

- Update file paths (`.cfg`, `.weights`, `.wav`) according to your system setup
- Ensure the alarm file exists to avoid runtime errors

## License

This project is licensed under the MIT License.

