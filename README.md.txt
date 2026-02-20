# 🩺 Nadi Smartwatch: IoT Monitoring Sandbox

A full-stack IoT development environment designed to monitor real-time health data. This project utilizes a **NodeMCU (ESP8266)** to publish simulated heart rate data to a containerized **Mosquitto MQTT** broker, which is then processed and visualized using **Node-RED**.

## 🚀 Features
* **Containerized Infrastructure**: The backend (Broker & Node-RED) runs in Docker for portability.
* **Real-time Dashboard**: Live gauge and chart visualizations of "Nadi" heart rate data.
* **Automated Alerts**: Threshold logic triggers notifications and audio alarms when heart rate exceeds 100 BPM.
* **Data Persistence**: Uses Docker volumes to ensure flows are saved during restarts.

## 🛠️ Technical Stack
* **Hardware**: NodeMCU 1.0 (ESP8266).
* **Middleware**: Eclipse Mosquitto (MQTT Broker).
* **Orchestration**: Docker Compose.
* **Logic Engine**: Node-RED.

## 🔧 Setup
1. Ensure Docker Desktop is running.
2. Run `docker compose up -d` in the project folder.
3. Flash the provided `.ino` code to your NodeMCU.
4. Access the UI at `http://localhost:1880/ui`.