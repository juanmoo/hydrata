# Hydrata

Hydrata is a plant-care automation platform designed to provide quantitative insights into plant health through easy-to-access visualizations. The project is modular and extensible, allowing for future expansion.

## Tech Stack

- **Sensors:** ESP32 microcontrollers connected to [capacitive soil moisture sensors](https://www.elecrow.com/crowtail-capacitive-soil-moisture-sensor.html). Sensors are configured to take readings every 5 seconds and transmit data wirelessly.
- **API:** Python [FastAPI](https://fastapi.tiangolo.com/) backend for ingesting sensor data, managing devices, and exposing endpoints for data retrieval.
- **Database:** [PostgreSQL](https://www.postgresql.org/) for persistent storage of sensor readings and metadata.
- **Visualization:** [Grafana](https://grafana.com/) dashboards for real-time and historical visualization of sensor data.

## Features

- **Automated Data Collection:** ESP32-based sensors continuously monitor soil moisture and send readings to the backend.
- **RESTful API:** FastAPI provides endpoints for data ingestion, device management, and data access.
- **Persistent Storage:** All sensor data is stored in a PostgreSQL database for reliability and scalability.
- **Visual Dashboards:** Grafana dashboards allow users to monitor current and historical moisture levels for each sensor.

## Getting Started

1. **Set up Sensors:** Flash ESP32 devices with the provided firmware and connect capacitive moisture sensors.
2. **Deploy API:** Run the FastAPI backend to receive and process sensor data.
3. **Configure Database:** Set up a PostgreSQL instance and apply the required schema.
4. **Visualize Data:** Connect Grafana to the PostgreSQL database and import the provided dashboards.

## Roadmap

- Add support for additional sensor types and modules.
- Implement user authentication and device management.
- Integrate AI-driven plant care recommendations.

For detailed setup instructions, please refer to the [docs/SETUP.md](docs/SETUP.md).
