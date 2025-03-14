# Detecting Moving Objects in DAS Recordings

## Project Overview
This project focuses on developing an algorithm to detect and track moving objects in acoustic data collected from a Distributed Acoustic Sensing (DAS) system. The DAS system is attached to a fiber optic cable along Jana Pawla II Street, capturing vibrations caused by passing vehicles such as trams, trucks, and cars. The project was carried out during Computer Vision course on AI Vth sem on PUT.

## Methodology
1. **Load Data**: Process 2D numpy matrix representing strain rate measurements along the fiber optic cable.
2. **Noise Filtering**: Apply appropriate signal processing techniques to remove background noise.
3. **Object Detection**: Identify moving objects by isolating slanted lines in the data matrix.
4. **Velocity Calculation**: Compute the velocity of detected objects using given spatial and temporal metadata.

## Input Data
- **Format**: 2D numpy array (strain rate data)
- **Dimensions**: 
  - First axis: Time
  - Second axis: Space
- **Metadata**:
  - `dx = 5.1065 m` (spatial resolution)
  - `dt = 0.0016 s` (time resolution)
  - File duration: `10s`
  - Time samples per file: `6250`
  - File naming format: `HHMMSS`
  - Data date: `2024-05-07`

## Technologies Used
- Python
- NumPy
- Signal Processing Libraries (e.g., SciPy, OpenCV)
- Machine Learning (optional for advanced object tracking)

## Usage
1. Load the dataset using NumPy.
2. Apply noise filtering techniques.
3. Detect slanted lines representing moving objects.
4. Calculate and visualize object velocities.

## References
Distributed Acoustic Sensing (DAS) is a technology that converts optical fiber cables into highly sensitive vibration sensors by analyzing backscattered laser signals to detect strain variations.

---
**Authors**: Piotr Balewski 156037, Kuba Czech 156035
**Date**: December 2024
