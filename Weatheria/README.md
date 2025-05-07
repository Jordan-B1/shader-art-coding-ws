Absolutely! Here's the updated version of the `README.md` with that information included:

---

# 🛰️ IoT Project — Sensor Driver Development & Real-Time Monitoring

## 📌 Project Overview

This project aims to build a complete IoT infrastructure with the following goals:

* Develop **custom drivers for sensors** (light, temperature, humidity, etc.).
* Run these drivers on **Raspberry Pi** devices to collect sensor data in real-time.
* Send the collected data to an **InfluxDB time-series database**.
* Monitor the data live using **Grafana dashboards**.

The project emphasizes real-time data flow, modular development, and system robustness.

> 💡 The subject is written using the **official Epitech project format**, but the **content and concept are entirely my own creation**.

---

## 🧭 Workshop Structure

The workshop is **divided into multiple sessions**, each covering a specific stage of the project:

* Sensor driver development
* Backend & data pipeline setup
* Live monitoring with Grafana
* Optional advanced features (e.g., authentication, automation)

Each session has its own dedicated PDF file, which can be found in the `subjects/` folder.

```
subjects/
├── session1_driver_dev.pdf
├── session2_influx_grafana.pdf
├── session3_auth_iot_security.pdf
└── session4_optional_extensions.pdf
```

---

## ⚙️ Technical Architecture

```
[ Sensor ] ---> [ Driver on RPi ] ---> [ InfluxDB ] ---> [ Grafana ]
```

* Drivers interact directly with the sensors over the I2C bus.
* Raspberry Pis run the drivers continuously and forward data as it is read.
* InfluxDB stores the measurements using an efficient time-series model.
* Grafana is configured to display dynamic, customizable dashboards.

---

## 🔧 Technologies Used

* 🐍 Python (for driver development)
* 📦 `smbus2` (I2C communication)
* 🍓 Raspberry Pi OS
* 🗃️ InfluxDB (time-series database)
* 📊 Grafana (data visualization)
* 🐳 Docker & Docker Compose (service deployment)

---

## 🚀 Learning Objectives

* Understand low-level sensor communication (via datasheets and protocols).
* Design robust and modular sensor drivers.
* Work with time-series data storage and querying.
* Deploy a full-stack IoT monitoring solution.

---

## 🧪 Example Sensor

* **TSL2561** (Light sensor)

  * Communication: I2C
  * Students are expected to read and interpret the **sensor datasheet** to determine registers, addresses, and configuration modes.

---

## 📁 Project Structure

```
iot-project/
├── drivers/
│   └── tsl2561_driver.py
├── docker/
│   ├── docker-compose.yml
│   ├── influxdb/
│   └── grafana/
├── docs/
│   ├── session1_driver_dev.pdf
│   ├── session2_influx_grafana.pdf
│   ├── session3_auth_iot_security.pdf
│   └── session4_optional_extensions.pdf
├── scripts/
│   └── setup_pi.sh
└── README.md
```

## 👨‍🏫 Context

This project is designed for  students with a strong programming foundation, aiming to deepen their skills in:

* Embedded systems
* Hardware-level communication protocols
* IoT data pipelines
* Real-time data visualization
