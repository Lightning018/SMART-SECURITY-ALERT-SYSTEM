# 🚨 Intruder Alert System Using YOLO and Email Notifications 🔍

## 🔥 Overview
This project is a real-time intruder detection system using YOLO (You Only Look Once) object detection. It continuously monitors a video feed and alerts the user when a human is detected. The system sends an email notification 📧 with an image of the detected person and also provides real-time alerts using Notify 📲.

## ⚡ Features
- 🎥 Real-time object detection using YOLOv3
- 🕵️‍♂️ Detects humans and triggers alerts
- 📩 Sends email notifications with the captured image
- 🛠️ GUI for setting confidence and threshold levels
- 🖥️ Uses PySimpleGUI for a simple user interface

## 📌 Requirements
Make sure you have Python installed on your system. Then, install all required dependencies listed in `requirements.txt` using:
```bash
pip install -r requirements.txt
```

## 🚀 Setup and Running the Project
1. **Clone the Repository** 📥
   ```bash
   git clone https://github.com/your-username/intruder-alert-system.git
   cd intruder-alert-system
   ```

2. **Install Dependencies** ⚙️
   ```bash
   pip install -r requirements.txt
   ```

3. **Download YOLO Model Files** 📂
   - Place the YOLO model files (`yolov3.weights`, `yolov3.cfg`, and `coco.names`) inside the `yolo-coco` directory.

4. **Enable Less Secure Apps for Gmail** 🔑
   - If using a Gmail account for email alerts, you must allow less secure apps or create an **App Password** for authentication.
   - Visit [Google Less Secure Apps](https://myaccount.google.com/security) and enable the setting or generate an app-specific password.

5. **Run the Detection Script** 🎯
   ```bash
   python intruder_alert.py
   ```

6. **Adjust Settings (Optional) 🔧**
   - The GUI allows you to change the confidence and threshold levels in real time.
   - You can modify the email sender and receiver in the `send_email` function inside the script.

## 🛠️ How It Works
1. The system initializes the webcam and loads the YOLO model.
2. It processes video frames and detects objects.
3. If a human is detected, it sends a notification and captures an image.
4. The captured image is sent via email as an alert.

## 🔮 Future Improvements
- ☁️ Implement a cloud-based notification system
- 📹 Add support for multiple camera sources
- ⚡ Optimize model inference for faster processing



