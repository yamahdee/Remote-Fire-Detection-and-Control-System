# Remote-Fire-Detection-and-Control-System 


**Overview**

This project is a remote fire detection and control system designed for early detection and response to fire hazards. It integrates IoT technology to provide real-time monitoring and remote control functionalities via a mobile app and SMS commands.

**Features**

-Monitors environmental conditions for fire risks using:

-DHT11: Temperature and humidity sensor.

-MQ135: Gas detection sensor.

-MQ2: Smoke detection sensor.

-Flame Sensor: Detects visible flames.

-Sends alerts and sensor data to a Firebase Realtime Database.

-Controls sprinklers via SMS commands using a SIM800L module.

-Provides a user-friendly interface via a Flutter mobile app for real-time monitoring.


**System Components**

-ESP32 Microcontroller: For sensor integration and IoT communication.

**Sensors:**

-DHT11: Reads temperature and humidity levels.
-MQ135: Detects gas leakage.
-MQ2: Detects smoke.
-Flame Sensor: Monitors for flames.

**Communication Modules:**

-SIM800L: Handles SMS alerts and remote control.
-Wi-Fi: Used by ESP32 to send data to Firebase.
-Mobile App: Built with Flutter, displays sensor readings and alerts users in real time.

**How It Works**

-Sensors collect environmental data and send it to the ESP32 microcontroller.
-The ESP32 updates the Firebase Realtime Database with sensor readings.
-If thresholds are exceeded, the system:
-Sends an SMS alert via the SIM800L module.
-Activates sprinklers when commanded remotely via SMS.
-Users can monitor the system and send control commands using the Flutter app.

**#Technologies Used**

-Hardware: ESP32, DHT11, MQ135, MQ2, Flame Sensor, SIM800L.

**#Software:**

-Firebase Realtime Database for IoT backend.
-Flutter framework for mobile app development.
-Arduino IDE for programming the ESP32.
