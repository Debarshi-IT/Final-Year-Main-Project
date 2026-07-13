# User Controls & Interface Guide

This guide explains how to drive the vehicle, navigate using autopilot, configure simulation parameters, and interpret telemetry analytics.

---

## ⌨️ Manual Keyboard Controls

Manual input overrides autopilot instantly.

| Key | Action | Details |
| :--- | :--- | :--- |
| **`▲` (Up Arrow)** | **Accelerate** | Increases forward speed |
| **`▼` (Down Arrow)** | **Brake / Reverse** | Decelerates or reverses the vehicle |
| **`◀` (Left Arrow)** | **Steer Left** | Rotates front wheels left |
| **`▶` (Right Arrow)** | **Steer Right** | Rotates front wheels right |
| **`SPACEBAR`** | **Handbrake** | Sudden lock of speed for emergency stops |

---

## 🧭 Autopilot Navigation Mode

Autopilot steers the vehicle autonomously using paths calculated by the backend server.

1. **Configure Nodes**:
   - Go to the **Self-Pathing Navigation** panel on the right sidebar.
   - Choose a **Start Junction** (where the car will start or teleport to) and a **Destination Junction**.
2. **Engage**:
   - Click **ENGAGE AUTOPILOT**. The car will teleport to the starting node and begin navigating to the target using dynamic steering and speed adjustments.
3. **Disengage / Override**:
   - Click **DISENGAGE AUTOPILOT** at any time.
   - Alternatively, **press any manual keyboard control key** (e.g., Up/Down/Left/Right/Space) to instantly take control of the vehicle.

---
