# AirWatcher: Air Quality Monitoring Application

## Overview
AirWatcher is a software application developed for a government agency to monitor and analyze air quality data across a large territory. This project was completed as part of a Software Engineering Lab series at INSA Lyon.

The application processes data collected from sensors distributed across the region to help identify malfunctioning sensors, calculate air quality statistics, and track the impact of industrial air cleaners. It also includes functionality for ranking sensors based on air quality similarity and detecting unreliable data from privately owned sensors.

## Key Features
- **Sensor Health Monitoring:** Analyze sensor data to detect malfunctions and reliability issues.
- **Air Quality Statistics:** Calculate mean air quality in a user-specified area or time period.
- **Sensor Similarity Ranking:** Rank sensors based on air quality similarity during a specified time period.
- **Impact Analysis of Air Cleaners:** Monitor the influence of industrial air cleaners on air quality.
- **Geographic Estimation:** Provide air quality estimates for precise locations, even without a sensor present.
- **Private Sensor Participation:** Manage sensors installed by private individuals, rewarding data contribution while identifying potential malicious activity.

## Data Sources
- **Sensors:** Defined in `sensors.csv`, including SensorID, latitude, and longitude.
- **Measurements:** Data from sensors are in `measurements.csv`, with timestamp, SensorID, AttributeID (e.g., O3, PM2.5), and values.
- **Attributes:** The types of measurements (e.g., Ozone, PM2.5) are detailed in `attributes.csv`.
- **Air Cleaners:** Industrial air cleaners and their operation periods are stored in `cleaners.csv`.
- **Providers and Users:** Air cleaner providers and individual sensor users are stored in `providers.csv` and `users.csv`.

## Algorithms
The application includes efficient algorithms for:
- Sensor malfunction detection
- Air quality aggregation and statistics
- Sensor similarity computation
- Classification of unreliable sensors

The performance of these algorithms is measured in terms of execution time to ensure efficiency.

## User Interface
AirWatcher offers a console-based user interface tailored for different roles within the government agency and private individuals. The application is run locally on the agency's server, and remote access is not supported.

## Project Structure
- **Source Code:** Includes all functionalities with guides to build the executable.
- **Tests:** Unit tests for core functionalities, with test data and non-regression procedures.
- **Documentation:** Includes detailed specifications, design diagrams, and user manuals.

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/Samsam19191/AirWatcher.git
2. Navigate to the project directory and run the application using make:

cd AirWatcher
make

This will compile and run the application based on the Makefile provided.

3. Interact with the application through the console, using the commands described in the user manual.
