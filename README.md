# Camera Calibration & Perspective Projection 🎥⚽

[![Python](https://img.shields.io/badge/Python-3.x-blue.svg)](https://www.python.org/)
[![OpenCV](https://img.shields.io/badge/OpenCV-4.x-green.svg)](https://opencv.org/)

## 📌 Project Overview
This project focuses on the implementation of **Perspective Projections** through advanced camera calibration algorithms. Designed as a technical exploration of **Computer Vision**, the system demonstrates how mathematical models can map 3D world coordinates onto a 2D image plane with high precision.

The core objective is to demonstrate how mathematical models can translate 2D image data into 3D spatial context—a technology widely used in modern sports broadcasting.

By accounting for lens characteristics and spatial orientation, this implementation bridges the gap between raw digital imagery and geometrically accurate environmental data. It serves as a foundational tool for applications requiring spatial awareness, such as sports analytics, augmented reality, and robotic navigation.

---

## ⚽ Applications: The VAR System
In modern football (soccer), the **Video Assistant Referee (VAR)** relies heavily on these algorithms to ensure fair play. By calibrating the cameras to the pitch, the system can draw mathematically accurate lines to determine player positions.

### 1. Offside Line Projection
Using homography, we can project a line that remains parallel to the goal line, even when the camera is at an angle.

<p align="center">
  <img src="./assets/offside_lined.jpg" width="450" title="Offside Line" alt="Offside Line Projection">
</p>

### 2. 3D Perspective Player Line
By accounting for 3D deformation, the system can project vertical lines to judge a player's body position (shoulders/head) relative to the ground.

<p align="center">
  <img src="./assets/3d_perpsective_line.jpg" width="450" title="3D Perspective" alt="3D Perspective Player Line">
</p>

---

## 🛠️ Technical Methodology
The project utilizes **OpenCV** to perform coordinate transformations. 



### Key Concepts:
* **Homography:** Mapping points from the camera view to a "top-down" pitch view.
* **Intrinsic Parameters:** Correcting for lens focal length and optical centers.
* **User Interaction:** The system allows for manual point selection to define the calibration plane dynamically.

---

## 🚀 Getting Started

### 📋 Prerequisites
The project was developed and tested using **Python 3**. Ensure you have `pip` installed to manage packages.

### 📥 Installation
1. **Clone the repository:**
   ```bash
   git clone [https://github.com/Andy9822/camera_calibration.git](https://github.com/Andy9822/camera_calibration.git)
   cd camera_calibration
   
2. **Install dependencies:** <br/>
   run `pip install -r -requirements.txt` <br />

3. **Run offside line drawer program:** <br/>
   run `python3 offside_line_projection.py` <br />
   
4. **Run 3D perspective line drawer program:** <br/>
   run `python3 offside_line_projection.py`<br />