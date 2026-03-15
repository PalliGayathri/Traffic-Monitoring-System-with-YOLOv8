# Traffic Monitoring System with YOLOv8

A real-time intelligent traffic monitoring system that detects vehicles, estimates their speed, and counts traffic flow using the YOLOv8 deep learning model.

---

## Overview

This project implements a computer vision-based traffic monitoring solution capable of detecting multiple vehicle types, estimating their speeds, and counting vehicles entering and exiting a defined region of interest (ROI). Built with YOLOv8 (You Only Look Once), it delivers high-accuracy detection suitable for real-world traffic management applications.

**Use cases include:**
- Urban traffic congestion monitoring
- Highway traffic flow analysis
- Automated vehicle counting for smart cities
- Real-time surveillance and analytics

---

## Key Features

| Feature | Description |
|---|---|
| Real-Time Detection | Detects cars, trucks, motorcycles, and buses using YOLOv8 |
| Speed Estimation | Calculates vehicle speed based on frame timestamps and ROI crossing |
| Vehicle Counting | Tracks entry and exit counts within the region of interest |
| Customizable ROI | Define custom polygonal regions for precise monitoring |
| Video Support | Works with pre-recorded video files and live webcam feed |

---

## Tech Stack

- **Python** 3.10+
- **YOLOv8** — [Ultralytics](https://github.com/ultralytics/ultralytics)
- **OpenCV** — Video capture and frame processing
- **NumPy** — Numerical computations

---

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/PalliGayathri/Traffic-Monitoring-System-with-YOLO.git
cd Traffic-Monitoring-System-with-YOLO
```

### 2. Install Dependencies

```bash
pip install ultralytics opencv-python numpy
```

### 3. Run the System

```bash
python Traffic.py
```

> **Note:** The YOLOv8 model weights (`yolov8n.pt`) are included in the repository. A sample traffic video (`traffic_video.mp4`) is also provided for testing.

---

## Project Structure

```
Traffic-Monitoring-System-with-YOLO/
├── Traffic.py            # Main application script
├── yolov8n.pt            # YOLOv8 nano model weights
├── traffic_video.mp4     # Sample test video
├── LICENSE
└── README.md
```

---

## How It Works

1. **Frame Capture** — Video frames are captured from a file or webcam using OpenCV.
2. **Object Detection** — Each frame is passed through YOLOv8 to detect and classify vehicles.
3. **ROI Tracking** — Vehicles crossing the defined region boundaries trigger counting and speed calculations.
4. **Speed Estimation** — Speed is derived from the time elapsed between two ROI crossing events and known real-world distances.
5. **Output** — Results are overlaid on the video feed in real time, displaying vehicle count and speed.

---

## Author

**Palli Gayathri**

- GitHub: [github.com/PalliGayathri](https://github.com/PalliGayathri)
- LinkedIn: [linkedin.com/in/palli-gayathri-1a5105384](https://www.linkedin.com/in/palli-gayathri-1a5105384/)
- Email: [bapujipalli452@gmail.com](mailto:bapujipalli452@gmail.com)

---

## License

This project is licensed under the [MIT License](LICENSE).
