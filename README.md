# Face Recognition Attendance System (Streamlit App)

A face recognition–based attendance system built with **Python** and **Streamlit**.  
The application detects and recognizes faces from images or a live webcam feed and automatically records attendance in a CSV file.

The goal of this project is to provide a simple, interactive attendance system with a clean web interface.

---

## Features

- Face detection and recognition
- Supports multiple faces in a single frame
- Real-time webcam tracking
- Image-based face recognition
- Attendance stored in a CSV file
- Simple and intuitive Streamlit UI
- Easy database management (add, update, delete users)

---

## Tech Stack & Requirements

- Python 3.9
- Streamlit 1.22.0
- face_recognition
- OpenCV
- NumPy

All required dependencies are listed in `requirements.txt`.

---

## Project Structure

```bash
├── dataset
│   ├── ID_Name.jpg
│   └── ...
├── pages
│   ├── 1_Updating.py
│   └── 2_Database.py
├── assets
│   ├── adding.png
│   ├── tracking.png
│   └── webcam.gif
├── Tracking.py
├── utils.py
├── config.yaml
├── requirements.txt

```

## Folder & File Overview

### dataset
- Contains images of people to be recognized
- Naming format: `ID_Name.jpg`
- Example: `1_Elon_Musk.jpg`, `2_Jenna_Ortega.jpg`
- Supported formats: jpg, jpeg, png

### pages
- Contains individual Streamlit pages
- Used for navigation and app features
- Naming format:
  - `Order_PageName.py`
  - `Order_Icon_PageName.py`

### Tracking.py
- Main entry point of the application
- Handles:
  - Real-time webcam tracking
  - Image-based face recognition
  - Attendance logging

### utils.py
- Shared utility functions
- Handles reusable logic such as:
  - Face encoding
  - CSV operations
  - Helper methods

### config.yaml
- Central configuration file
- Stores:
  - Dataset paths
  - Application messages
  - App-level settings

### requirements.txt
- Lists all Python dependencies
- Used to install required libraries with pip

### packages.txt
- Lists system-level packages
- Required for deployment on Streamlit Cloud

├── packages.txt
└── README.md

## Installation

### 1. Clone the repository
```bash
git clone https://github.com/Abdul7410/face-check-in-app.git
```

### 2. Install dependencies
```bash
cd face-check-in-app
```

### 3. Run the application
```bash
pip install -r requirements.txt
```

## How It Works

1. Load known faces from the `dataset` folder.
2. Capture faces using a webcam or an uploaded image.
3. Detect and encode faces in real time.
4. Compare detected faces against stored face encodings.
5. Automatically log attendance into a CSV file.
6. Manage users through the update and database pages.

---

## Use Cases

- Classroom attendance tracking
- Office or workplace check-in systems
- Small-scale face recognition demonstrations
- Learning project for computer vision and Streamlit


