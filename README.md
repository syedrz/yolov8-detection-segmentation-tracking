# Real-time Object Detection and Tracking with YOLOv8 and Streamlit

This repository is a comprehensive open-source project that demonstrates the integration of object detection and tracking using the YOLOv8 object detection algorithm and Streamlit, a popular Python web application framework for building interactive web applications. This project provides a user-friendly and customizable interface that can detect and track objects in real-time video streams.

## Tracking With Object Detection Demo

<https://user-images.githubusercontent.com/104087274/234874398-75248e8c-6965-4c91-9176-622509f0ad86.mov>

## Demo Pics

### Home page

<img src="https://github.com/syedrz/yolov8-detection-segmentation-tracking/blob/master/assets/pic1.png" >

### Page after uploading an image and object detection

<img src="https://github.com/syedrz/yolov8-detection-segmentation-tracking/blob/master/assets/pic3.png" >

### Segmentation task on image

<img src="https://github.com/syedrz/yolov8-detection-segmentation-tracking/blob/master/assets/segmentation.png" >

## Requirements

Python 3.6+
YOLOv8
Streamlit

```bash
pip install ultralytics streamlit pafy
```

## Installation

- Clone the repository: git clone <https://github.com/syedrz/yolov8-detection-segmentation-tracking.git>
- Change to the repository directory: `cd yolov8-detection-segmentation-tracking`
- Create `weights`, `videos`, and `images` directories inside the project.
- Download the pre-trained YOLOv8 weights from (<https://github.com/ultralytics/assets/releases/download/v0.0.0/yolov8n.pt>) and save them to the `weights` directory in the same project.

## Usage

- Run the app with the following command: `streamlit run app.py`
- The app should open in a new browser window.

### ML Model Config

- Select task (Detection, Segmentation)
- Select model confidence
- Use the slider to adjust the confidence threshold (25-100) for the model.

One the model config is done, select a source.

### Detection on images

- The default image with its objects-detected image is displayed on the main page.
- Select a source. (radio button selection `Image`).
- Upload an image by clicking on the "Browse files" button.
- Click the "Detect Objects" button to run the object detection algorithm on the uploaded image with the selected confidence threshold.
- The resulting image with objects detected will be displayed on the page. Click the "Download Image" button to download the image.("If save image to download" is selected)

## Detection in Videos

- Drag and drop video file
- Click on `Detect Video Objects` button and the selected task (detection/segmentation) will start on the selected video.

### Detection on RTSP

- Select the RTSP stream button
- Enter the rtsp url inside the textbox and hit `Detect Objects` button

### Detection on YouTube Video URL

- Select the source as YouTube
- Copy paste the url inside the text box.
- The detection/segmentation task will start on the YouTube video url

<https://user-images.githubusercontent.com/104087274/226178296-684ad72a-fe5f-4589-b668-95c835cd8d8a.mov>

## Acknowledgements

This app is based on the YOLOv8(<https://github.com/ultralytics/ultralytics>) object detection algorithm. The app uses the Streamlit(<https://github.com/streamlit/streamlit>) library for the user interface.

### Disclaimer

Please note that this project is intended for educational purposes only and should not be used in production environments.

**Hit star ⭐ if you like this repo!!!**
