# Face Recognition Attendance System (Streamlit App)

This project is a face recognition–based attendance system built with Python and Streamlit. It uses a face recognition library to detect and recognize faces from images or a live webcam feed and records attendance automatically in a CSV file.

The goal of this project is to provide a simple, interactive way to manage attendance using face recognition with a clean web interface.



## Features

* Face detection and recognition
* Supports multiple faces in a single frame
* Real-time webcam tracking
* Image-based face recognition
* Attendance stored in a CSV file
* Simple and intuitive Streamlit UI
* Easy database management (add, update, delete users)



## Tech Stack & Requirements

* Python 3.9
* Streamlit 1.22.0
* face_recognition
* OpenCV
* NumPy

All required dependencies are listed in `requirements.txt`.



## Project Structure

```bash
├── dataset
│   ├── ID_Name.jpg
│   └── ...
├── pages
│   ├── 1_🔧_Updating.py
│   └── 2_💾_Database
├── Tracking.py
├── utils.py
├── config.yaml
├── requirements.txt
├── packages.txt
└── README.md
```



## Folder & File Overview

* **dataset**
  Contains images of people to be recognized.
  File naming format: `ID_Name.jpg`
  Example: `1_Elon_Musk.jpg`, `2_Jenna_Ortega.jpg`
  Supported formats: jpg, jpeg, png

* **pages**
  Contains individual Streamlit pages.
  New pages can be added using the format:
  `Order_Icon_PageName.py` or `Order_PageName.py`

* **Tracking.py**
  Main entry point of the application.
  Handles real-time webcam tracking and image-based recognition.

* **utils.py**
  Utility functions used across the application.

* **config.yaml**
  Application configuration such as dataset paths and messages.

* **requirements.txt**
  Python dependencies.

* **packages.txt**
  Packages required for deployment on Streamlit Cloud.



## Installation

1. Clone the repository

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the application

```bash
streamlit run Tracking.py
```



## How It Works

1. Load known faces from the dataset folder
2. Capture faces via webcam or upload an image
3. Match detected faces against the dataset
4. Automatically log attendance to a CSV file
5. Manage users through the update and database pages



## Use Cases

* Classroom attendance
* Office check-in systems
* Small-scale face recognition demos
* Learning project for computer vision + Streamlit


