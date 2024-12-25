### README.md


# Face Recognition Attendance System

## Overview

This project implements a **Face Recognition Attendance System** using Python. It uses face recognition technology to mark attendance in real-time by detecting and identifying faces through a webcam. Attendance records are stored in a CSV file for future reference.

## Features

- **Real-Time Face Recognition**: Detects and recognizes faces in real time using the webcam.
- **Automated Attendance Tracking**: Marks attendance with a timestamp for identified faces.
- **Preloaded Known Faces**: Compares live webcam frames with preloaded images of known individuals.
- **Efficient Storage**: Avoids duplicate entries for the same person during a session.
- **User-Friendly Exit**: Easily terminate the system by pressing 'q' or closing the window.

## Directory Structure


project/
│
├── AttendanceImage/    
├── Attendance.csv     
├── main_script.py      

## Prerequisites

Ensure you have the following installed on your system:
- Python (>= 3.6)
- Webcam (for live video feed)

## Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/face-recognition-attendance-system.git
   cd face-recognition-attendance-system
   ```

2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Add images of known individuals to the `AttendanceImage` directory. Use recognizable filenames (e.g., `elon.jpg`).

4. Run the main script:
   ```bash
   python main_script.py
   ```

## How It Works

1. The script reads all images from the `AttendanceImage` directory.
2. Face encodings are generated for each image and stored.
3. The webcam captures frames, detects faces, and compares them to the stored encodings.
4. When a match is found, the system marks the person's name and the timestamp in the `Attendance.csv` file.

## Exit Instructions

- Press `q` to quit the program.
- Close the webcam window manually to exit.

## Contributing

Feel free to fork this repository and submit pull requests for:
- Adding new features
- Fixing bugs
- Improving performance
