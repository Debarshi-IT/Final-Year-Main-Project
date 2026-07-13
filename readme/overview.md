# Project Overview: 3D Self-Driving Car Simulator

Welcome to the **SmartDrive Autopilot Simulator**, a high-fidelity 3D interactive self-driving car testbed. This project integrates a WebGL frontend (built with Three.js and Vite) and a Python Flask backend to simulate, control, and analyze autonomous driving telemetry in real-time.

---

## 🌟 Core Features

### 1. 3D WebGL Physics & Environment
- **Interactive Three.js Scene**: Features lighting, custom shadows, and fog configurations.
- **Procedural Road Network**: Generates 4-way intersections, 3-way junctions, parking bays, road lanes, traffic lights, and street markings dynamically.
- **Pedestrian Simulation**: Simulates walking pedestrians crossing roads, which the car's sensors must detect and avoid.

### 2. Multi-Directional LiDAR Raycasting
- Uses Three.js raycasting to simulate a physical LiDAR system.
- Projects multiple laser beams in a forward-facing arc from the car.
- Dynamically highlights intersections with obstacles (traffic, pedestrians) and feeds real-time proximity metrics to the autopilot and dashboard.

### 3. A* Pathfinding Navigation
- Employs a backend-calculated **A* Search Algorithm** across nodes and weighted road edges to discover optimal paths.
- Provides dynamic, highlighted path waypoints for the vehicle to trace during autonomous mode.

### 4. Smart Autopilot & Cruise Control
- Automatically handles acceleration, braking, and steering using path-following geometry.
- Slows down or halts for obstacles and red lights, maintaining lane alignment automatically.
- **Instant Manual Override**: Seamlessly hands back steering/acceleration controls to the user upon any manual keystroke (arrow keys, spacebar).

### 5. Telemetry & Ride Comfort Analytics
- Streams real-time speed, acceleration (G-forces), cumulative distance, and collision metrics.
- Processes logged data on the backend to render professional analytics charts using Matplotlib:
  - **Speed Profile**: Interactive velocity charts.
  - **Safety Index**: Autopilot caution tracking and Lidar warnings.
  - **Ride Comfort (G-G diagram)**: Longitudinal acceleration scatter plotting to assess deceleration comfort.
