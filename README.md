# 🏎️ SmartDrive: 3D Autonomous Autopilot Driving Simulator

SmartDrive is an interactive WebGL-based autonomous driving car simulator. This application tests autopilot navigation algorithms on a procedural 3D road network, utilizing front-facing LiDAR raycasting sensors and real-time telemetry tracking. The system couples a Three.js and Vite client-side simulator with a Flask backend to perform shortest-path computations and generate post-drive performance charts.

---

## ⚡ Quick Start

### 1. Run the Python Backend
Activate a terminal in the project root and run:
```bash
# Set up virtual environment
python -m venv venv
# Activate (Windows PowerShell)
.\venv\Scripts\Activate.ps1
# Install dependencies
pip install -r requirements.txt
# Run server
python app.py
```
*The backend server will run on `http://127.0.0.1:5000`.*

### 2. Run the Vite Frontend
Activate a second terminal in the project root and run:
```bash
# Install Node modules
npm install
# Start developer server
npm run dev
```
*The client site will open automatically on `http://localhost:3000`.*

---

## 📖 Project Documentation

For deeper details regarding setup, controls, and architecture, explore the dedicated documentation guides:

*   🌐 **[Project Overview](file:/SMARTDRIVE/readme/overview.md)**: Explore the simulator's core feature set, environmental capabilities, and simulation modes.
*   🚀 **[Installation & Running Guide](file:/SMARTDRIVE/readme/setup.md)**: Step-by-step setup walkthrough for Python (venv) and Node.js environments.
*   📐 **[System Architecture](file:/SMARTDRIVE/readme/architecture.md)**: Breakdown of the client-side class structure (`Car`, `SelfDrivingCar`, `Sensor`, `RoadNetwork`, `TrafficManager`), API specifications, and the data sequence pipeline.
*   🎮 **[Controls & Settings Guide](file:/SMARTDRIVE/readme/controls.md)**: Details on manual driving keyboard binds, autopilot configuration, camera selection, and telemetry charts.
