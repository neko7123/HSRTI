# High Speed Railtrack Inspection System

![WhatsApp Image 2025-02-02 at 20 54 20_704b5dad](https://github.com/user-attachments/assets/6026823e-01f1-49e7-8650-94fb45061bd4)


# Overview

The High Speed RailTrack Inspection System is a cutting-edge solution designed to inspect railway tracks at operational speeds between 15 km/h to 120 km/h without requiring the train to slow down.
The system uses a combination of ultrasonic and acoustic sensors to detect both surface-level and internal faults.
An integrated GPS module provides exact fault locations, and a trained machine learning model predicts upcoming failures in advance, enabling preventive maintenance.

# Key Features

1. Real-Time Rail Monitoring:
2. 
Captures rail track condition data dynamically even at high speeds.

3. High-Precision Sampling:

Equipped with 5 MHz ultrasonic sensors capable of collecting a sample every 0.2 microseconds.

The system collects approximately 7500 samples every 1.5 milliseconds, ensuring fine-grained defect detection.


3. Predictive Fault Detection:

Uses a machine learning model trained on real-world data to predict upcoming faults and critical issues.

4. Exact Location Tracking:
   
Integrated GPS records the precise position of anomalies for targeted maintenance actions.

5. User Mobile Application:

A Flutter-based mobile app helps maintenance personnel navigate directly to the predicted or existing fault locations, making interventions faster and more efficient.

6. Cloud Integration:

Sensor data is streamed live to a ThingSpeak server for storage and monitoring.
Critical fault alerts are automatically pushed to a Firebase server for immediate mobile notification.

# System Architecture

1. Hardware:

Arduino D1 Wi-Fi (ESP8266-based) microcontroller for real-time data processing

5 MHz Ultrasonic Sensors and Acoustic Sensors

GPS Module for geolocation tagging


2. Software:

Arduino IDE for firmware development

Flutter for mobile application development

ThingSpeak server for IoT data storage and visualization

Firebase server for push alerts


3. Machine Learning:

Model trained using 15,000+ samples collected from real-world track conditions at Virar Railway Car Shed.

Deployed and tested using Google Colab, achieving 90% model accuracy.

# Data Collection

Collected over 15,000 entries by field-testing on actual railway tracks.

Documented and classified track faults including:

Split Heads

Faulty Welds

Joint Gaps

Internal Cracks


Sensor readings along with defect photographs were recorded to build a reliable dataset.

# Project Impact

1. Faster Rail Inspections:
No need to slow down or halt trains for track inspection.

2  Enhanced Safety:
Early fault detection prevents derailments and major accidents.

3. Operational Efficiency:
Targeted maintenance saves cost, time, and manpower.

4. Higher Accuracy:
Ultra-high-speed sampling enables detection of even minor defects.

5. Smart Maintenance Planning:
Predictive alerts help maintenance teams act proactively.

# How It Works

1. High-frequency ultrasonic and acoustic sensors collect continuous data while in motion.


2. Data is sent to the ThingSpeak cloud server every second.


3. A machine learning model analyzes incoming data to detect patterns indicating potential faults.


4. If a fault is predicted to occur within one week, a critical alert is generated.


5. Alert and GPS location are transmitted to the Firebase server.


6. Maintenance personnel receive notifications via the Flutter mobile app, which guides them to the fault location.
