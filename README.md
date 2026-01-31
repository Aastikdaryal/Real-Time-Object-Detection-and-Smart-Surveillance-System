AI Powered Smart CCTV Surveillance System

This project is a real-time AI based CCTV surveillance system that performs live object detection and demographic analysis using a smartphone camera.
A mobile phone (iPhone) is used as a live CCTV camera and the video feed is processed on a laptop to detect objects and classify people as Man, Woman or Kid in real time.

The system combines computer vision, deep learning models and an interactive dashboard to simulate a real-world smart surveillance setup.

---

Features

Real-time live video feed from smartphone camera
Object detection using deep learning (MobileNet SSD)
Person-aware face detection
Age and gender classification
Man / Woman / Kid categorization
Live demographic counts on dashboard
Interactive Streamlit based UI
FPS and performance monitoring
Smartphone used as CCTV camera instead of traditional IP camera

---

Tech Stack

Programming Language: Python
Computer Vision: OpenCV
Deep Learning Models: MobileNet SSD, Age and Gender Caffe Models
Dashboard: Streamlit
Camera Source: Smartphone (iPhone as virtual webcam using iVCam)
Platform: Windows

---

System Architecture

Smartphone Camera (iPhone)
Virtual Webcam Driver (iVCam)
Laptop running Python and OpenCV
AI Models for object detection and face analysis
Streamlit Dashboard for live monitoring

---

Project Structure

Realtime-face-detection-using-AI

app.py
Streamlit dashboard application

main.py
Core AI logic using OpenCV and deep learning models

test_camera.py
Utility script to detect available camera index

activity_log.txt
Logs of detected people with age and gender

models folder

MobileNetSSD_deploy.prototxt
MobileNetSSD_deploy.caffemodel
age_deploy.prototxt
age_net.caffemodel
gender_deploy.prototxt
gender_net.caffemodel

---

How It Works

The smartphone camera streams live video to the laptop using a virtual webcam driver.
Each frame is processed using MobileNet SSD to detect objects.
When a person is detected, face detection is performed inside the person region only.
The detected face is passed through age and gender models.
Based on the prediction, the person is classified as Man, Woman or Kid.
All results are displayed on a real-time Streamlit dashboard with live counts and FPS.

---

Installation and Setup

Clone the repository

git clone [https://github.com/Aastikdaryal/Realtime-face-detection-using-AI.git](https://github.com/Aastikdaryal/Realtime-face-detection-using-AI.git)
cd Realtime-face-detection-using-AI

Install required libraries

pip install opencv-python numpy streamlit

Setup smartphone as camera

Install iVCam Webcam app on iPhone
Install iVCam driver on Windows
Connect phone using USB cable
Run test_camera.py to identify camera index

Run the dashboard

streamlit run app.py

---

Use Cases

Smart indoor CCTV surveillance
Office and workplace monitoring
Mall and store footfall analysis
School and campus safety monitoring
AI based demographic analytics

---

Future Improvements

Intrusion detection alerts
Cloud deployment
Multi camera support
Historical analytics and graphs
CSV or database based logging

---

Resume and Interview Highlight

Built an end-to-end AI powered CCTV surveillance system using a smartphone camera, real-time object detection and demographic face analysis with an interactive dashboard.

---

Author

Aastik Daryal
MCA Student
AI and Computer Vision Enthusiast

GitHub Profile
[https://github.com/Aastikdaryal](https://github.com/Aastikdaryal)

---

If you like this project, feel free to star the repository.
