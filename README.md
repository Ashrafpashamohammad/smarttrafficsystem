# 🚦 Smart Traffic Management System – AI-Powered Traffic Control

An intelligent, ML-powered traffic control system that dynamically manages traffic signals based on lane density, detects emergency vehicles, identifies violations, and supports automated response — all from video footage.

-----

### 🚀 About The Project

The **Smart Traffic Management System** is built to improve urban traffic flow using real-time video analytics. Traditional static timers are inefficient for today’s dynamic traffic conditions. This project combines **YOLOv5 object detection**, **OpenCV**, and custom logic to detect vehicle density and automate traffic light durations accordingly.

Additional features include:
- Emergency vehicle detection (ambulance/fire engine)
- Automated challan generation for traffic violations
- Accident detection with automatic ambulance dispatch
- Crime vehicle detection (hit-and-run, chain snatching)

The system is ideal for smart cities aiming to reduce congestion, prioritize emergency response, and enforce road safety.

### ✨ Features

  * 📹 **Traffic Density Estimation** – Detects vehicle count from junction-side video feeds using YOLOv5.
  * 🚨 **Emergency Vehicle Detection** – Prioritizes ambulances/fire engines stuck in traffic with automatic green signals.
  * 📛 **Violation Detection** – Automatically flags red-light jumping or lane-crossing from CCTV footage.
  * ⚠️ **Accident Detection** – Triggers ambulance dispatch via alert logic upon impact detection.
  * 🚓 **Crime Vehicle Identification** – Detects vehicles involved in criminal activity via license plate verification.
  * 📈 **Smart Signal Timer** – Dynamically allocates green/red time per lane based on live traffic data.
  * 🌐 **Web UI** – Upload 4 video feeds from each direction and receive signal timing + detection results.

### 🛠️ Tech Stack

This project leverages both AI and web technologies:

  * **Python 3.8+**
  * **YOLOv5** – Vehicle and object detection
  * **OpenCV** – Video frame processing
  * **Flask** – Backend API + Web interface
  * **HTML/CSS/JS** – Web UI for video upload & output display
  * **NumPy / Pandas** – Data handling
  * **Matplotlib** – Optional visualization for stats

### ⚙️ Getting Started (Local Setup)

To get a local copy up and running, follow these steps.

#### Prerequisites

  * Python 3.8+ with pip
  * [Git](https://git-scm.com/) installed
  * System with a GPU (recommended for YOLOv5 performance)
  * Basic video files of junction traffic from 4 directions

#### Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/Ashrafpashamohammad/Smart_traffic_controller.git
    cd Smart_traffic_controller
    ```

2.  **Create a virtual environment:**

    ```bash
    python -m venv venv
    venv\Scripts\activate      # Windows
    source venv/bin/activate   # macOS/Linux
    ```

3.  **Install dependencies:**

    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the application:**

    ```bash
    python app.py
    ```

5.  **Access the UI:**

    Open your browser and go to: [http://localhost:5000](http://localhost:5000)

    Upload the four video feeds and receive the recommended signal timings based on traffic density.

### 📂 Project Structure

```bash
Smart_traffic_controller/
├── app.py
├── yolov5_model/        # Custom-trained YOLOv5 weights
├── static/
├── templates/
├── utils/
│   ├── traffic_detector.py
│   ├── violation_checker.py
│   └── emergency_handler.py
├── requirements.txt
└── README.md

🤝 Contact
GitHub – @Ashrafpashamohammad
Project Link – https://github.com/Ashrafpashamohammad/Smart_traffic_controller

⭐ Star this repository if you find the project valuable or innovative!
