# Installation & Setup Guide

This guide details how to install project dependencies and run both the Python Flask backend and the Vite frontend.

---

## 🛠️ Prerequisites
Make sure you have the following installed:
1. **Python 3.8+**: To run the backend logic and generate charts.
2. **Node.js (v18+ recommended)**: To package and serve the 3D application.
3. **pip** and **npm**: Package managers for Python and Node.js.

---

## 🐍 Backend Setup (Flask Server)

The Python backend manages A* pathfinding computations, tracks active telemetry, and generates analysis charts.

1. **Open a terminal** and navigate to the project root directory.
2. **Create a virtual environment** to isolate dependencies:
   ```bash
   # Windows
   python -m venv venv

   # macOS / Linux
   python3 -m venv venv
   ```
3. **Activate the virtual environment**:
   ```bash
   # Windows PowerShell
   .\venv\Scripts\Activate.ps1

   # Windows Command Prompt (CMD)
   .\venv\Scripts\activate.bat

   # macOS / Linux
   source venv/bin/activate
   ```
4. **Install Python dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
5. **Run the Flask server**:
   ```bash
   python app.py
   ```
   *The server runs locally at `http://127.0.0.1:5000`.*

---

## ⚡ Frontend Setup (Vite & Three.js)

The frontend hosts the 3D WebGL simulator canvas and the interactive telemetry interface.

1. **Open a second terminal window** and navigate to the project root directory.
2. **Install Node dependencies** specified in `package.json`:
   ```bash
   npm install
   ```
3. **Run the development server**:
   ```bash
   npm run dev
   ```
   *This starts the Vite server (typically at `http://localhost:3000`) and will automatically launch the simulator in your default browser.*

---

## 🔗 Verifying the Integration

Once both servers are running:
- Look at the top status bar of the application web interface.
- Under **BACKEND**, it should display a green **ONLINE** badge.
- If it displays a red **OFFLINE** badge, double-check that your Python Flask server is running at port `5000` and CORS is allowed (handled automatically by `flask_cors`).
