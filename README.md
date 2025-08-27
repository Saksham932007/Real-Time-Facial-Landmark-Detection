# Real-Time Facial Landmark Detection

This project uses Python, OpenCV, and Google's MediaPipe library to perform high-fidelity facial landmark detection in real-time from a webcam feed.
Features

    Real-Time Performance: Smoothly processes webcam video to detect and track facial landmarks with minimal latency.

    478 Facial Landmarks: Utilizes the MediaPipe Face Mesh model to identify 478 distinct 3D landmarks on the face.

    High Precision: Accurately tracks detailed features like eyes, eyebrows, nose, mouth, and overall face contour.

    Lightweight and Efficient: Built with performance in mind, making it suitable for a wide range of applications.

    FPS Monitoring: Includes an on-screen FPS counter to monitor performance.

Getting Started

Follow these instructions to get a copy of the project up and running on your local machine.
Prerequisites

You will need to have Python 3 and a webcam installed on your system.

    Python 3.x: Download Python

    pip (Python package installer)

Installation

    Clone the repository:

    git clone https://github.com/your-username/your-repository-name.git
    cd your-repository-name

    Install the required Python libraries:
    All necessary packages are listed in the requirements.txt file. You can install them with a single command:

    pip install -r requirements.txt

    If a requirements.txt file is not available, you can install the packages manually:

    pip install opencv-python mediapipe numpy

Usage

To run the facial landmark detector, simply execute the main Python script from your terminal:

python facial_landmark_detection.py

A window will open displaying your webcam feed with the facial mesh and contours drawn on any detected faces.

    To quit the application, press the 'q' key.

How It Works

The script captures video from the default webcam using OpenCV. Each frame is then passed to the MediaPipe Face Mesh model, which is a powerful machine learning pipeline that predicts the location of 478 3D landmarks on the face.

The script performs the following key steps:

    Initializes the video capture and the MediaPipe Face Mesh model.

    Reads each frame from the webcam.

    Converts the image from BGR (OpenCV's default) to RGB, as required by MediaPipe.

    Processes the image to detect the facial landmarks.

    Draws the face mesh tessellation and contours onto the frame.

    Calculates and displays the real-time Frames Per Second (FPS).

    Displays the final processed frame in a window.

Acknowledgments

This project is built upon the incredible work done by the teams at Google with their MediaPipe framework.
