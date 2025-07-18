# Vehicle Detection and Counting System

![Project Status](https://img.shields.io/badge/status-Completed-brightgreen.svg)
![Platform](https://img.shields.io/badge/platform-PC--based-blue.svg)
![Language](https://img.shields.io/badge/language-Python-yellow.svg)
![Framework](https://img.shields.io/badge/framework-OpenCV%20%7C%20YOLOv4-red.svg)
![IDE](https://img.shields.io/badge/IDE-VS%20Code-blueviolet.svg)
![License](https://img.shields.io/badge/license-MIT-lightgrey.svg)

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/103e5c2b-0e59-4702-9802-44d87e662c03" />

## Introduction

The **Vehicle Detection and Counting System** is a real-time traffic monitoring solution built using **Python**, **OpenCV**, and **YOLOv4**. It is capable of identifying, tracking, and counting vehicles from a video feed or image sequence. It also features a voice interface using **pyttsx3** for audible alerts. This project addresses the growing need for intelligent traffic systems, helping to automate vehicle monitoring, enhance traffic flow analysis, and improve smart city infrastructure.

---

##  Problem Statement

Manual vehicle counting is time-consuming, error-prone, and not scalable for high-traffic areas. Our system aims to solve this by providing a fully automated, accurate, and scalable solution using computer vision and deep learning.

---

## Overview

This Python script is designed for real-time vehicle detection and counting using YOLOv4, OpenCV, pyttsx3, and a custom object detection module. The system identifies vehicles in a video stream, assigns unique IDs for tracking, and provides a voice-guided interface.

## Motivation

- Eliminate manual traffic counting.
- Provide real-time vehicle monitoring and alerts.
- Enable smart city infrastructure and intelligent traffic systems.
- Collect accurate traffic data for analytics and prediction.

---

## Scope

- Real-time vehicle detection in videos.
- Counting vehicles with unique IDs using tracking.
- Voice interaction for detected vehicle counts.
- Can be integrated with traffic lights, CCTV, or smart surveillance systems.

---

## Why Python?

Python is the preferred language for computer vision applications due to:

-  Easy syntax and rapid prototyping
-  Seamless integration with **OpenCV**
-  Support for deep learning frameworks like **YOLO**, **TensorFlow**, etc.
-  Libraries like `pyttsx3` make voice interaction easy

---

## Alogorthim:
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/b273058d-a35c-49e6-852e-4d78a22ff202" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/2d16ccdd-a035-438d-8a57-621ba6a13115" />

##  Libraries Used

| Library       | Purpose |
|---------------|---------|
| `cv2` (OpenCV) | Video capture, image processing, bounding boxes |
| `math`         | Distance calculations between object centers |
| `numpy`        | Frame matrix manipulation and array processing |
| `pyttsx3`      | Text-to-speech output for vehicle counts |
| `art`          | Generates ASCII art title screen for CLI |
| `textblob`     | Optional NLP tasks like text analysis |

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/9245f459-5dae-453e-8860-adfd99dcc396" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ccf03bbb-e74c-4a27-a727-ecdf2caada1d" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1194e042-c7a4-4cb9-a12f-048b505d9a19" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/943fef7e-5f3b-441d-92ce-dc3db2e433ce" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/f5a01232-bf8b-45e0-a859-7796cd11fea3" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/ae5c1ad8-7755-4922-b0bb-aeb8d5b7e435" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/dfe72a2a-058a-4e82-bbef-b14e53c3afce" />

## Flow Chart
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/c15f8264-cbc5-4038-921a-f6bb1044101b" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/4c708657-18ce-4fd4-93e8-e33ed0b47e49" />

## Installation

You have to download the latest version of python.

### Prerequisites

Make sure you have Python installed. You can download it from [python.org](https://www.python.org/downloads/).

### Install Required Libraries

Once python is installed then open the command window and run these commands.
```bash
pip install opencv-python
pip install numpy
pip install art
pip install pyttsx3
pip install textblob
pip install colorama
```

### Download YOLOv4 Weights

Download the YOLOv4 weights files and give the address of that files in object_detection.py.

Place the weights and cfg files in the object_detection directory .

## Usage

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/1e275917-ac67-4421-b299-0a3d6557548f" />
<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/238b70ec-e668-4a87-915b-23d1c4bcb269" />

1. Open the script in a code editor.

2. Customize the image/video file path according to your path:

   ```python
   video = cv2.VideoCapture("C:\\Users\\DELL\\OneDrive\\Desktop\\Project\\Highway.mp4")
   ```

3. Modify the YOLOv4 weights path:

   ```python
   od = ObjectDetection(weights_path="path/to/yolov4.weights")
   ```

4. Run the script:

   ```bash
   python vehicle_detection.py
   ```

## Working

## Image Processing:

Firstly you to download the libraries by using the above commands and then you have to save all the images and video files where your main.py file is located. 
When you will run the code then you have to answer some questions. When program ask for image processing then you have to put the name of that file only e.g 1
It depens on your image name and extension of image should be .png. For video processing repeat the same process and extension of video file should be .mp4

![1](https://github.com/Awais-Asghar/Vehicle-Detection-and-Counting-System-Using-Open-CV/assets/136043829/4e577579-220f-4c5d-a764-463ab9779ffb)

![2](https://github.com/Awais-Asghar/Vehicle-Detection-and-Counting-System-Using-Open-CV/assets/136043829/f269e931-241b-45a4-9dcb-0a06ee40e750)

It can detect cars in smog also.

![10](https://github.com/Awais-Asghar/Vehicle-Detection-and-Counting-System-Using-Open-CV/assets/136043829/944d7dbe-5420-4bd4-9fdf-e3cd0e5ce00d)

It can detect and count cars at night also.

![26354](https://github.com/Awais-Asghar/Vehicle-Detection-and-Counting-System-Using-Open-CV/assets/136043829/1e2dbe8b-2b34-4366-947b-8b252034e892)

## Video Processing:

![3](https://github.com/Awais-Asghar/Vehicle-Detection-and-Counting-System-Using-Open-CV/assets/136043829/f1a406c6-d371-4a94-bbdb-0c91c6d5aee9)

## Conclusion
The Vehicle Detection and Counting System provides a reliable, real-time solution for identifying and tracking vehicles using Python, OpenCV, and YOLOv4. It automates traffic monitoring with accurate detection and voice-based interaction, making it suitable for smart city and surveillance applications. This project lays the groundwork for future enhancements in intelligent transportation systems.

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/439dd0c6-4d62-4ad0-a437-274a331f4935" />
