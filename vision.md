<div align="center">

<img src="https://www.sju.edu.in/assets/img/st-joseph-university-logo.png" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://www.erafoundationindia.org/images/logo.svg" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://comedkares.org/wp-content/uploads/2023/04/Comedkares-Logo-EPS.png" height="80" style="background:white; padding:8px; margin:0 16px;" />

</div>


# VISION: AN IoT AND AI ENABLED SMART SOS PUBLIC SAFETY SYSTEM

### Authors

<div align="center">

Navaneetha M<sup>1</sup>,
R Nataraj<sup>1</sup>,
Sowmya J<sup>2</sup>,
V Kamala Kannan<sup>1</sup>,
Vijaya M<sup>2</sup>
<br><br>
<sup>1</sup> Master of Computer Applications (MCA)<br>
<sup>2</sup> MSc in Big Data Analytics (MSc BDA)

</div>

---

# Abstract

Public safety systems frequently encounter issues with delayed emergency responses due to a lack of real-time alerting mechanisms and intelligent awareness infrastructure. Most SOS applications currently in use only send alerts to specific people or organizations and do not proactively alert individuals in the immediate vicinity of an emergency or dynamically adapt based on real-time information about unsafe areas.

This work proposes VISION (Smart SOS Public Safety System), a comprehensive emergency response framework that combines IoT and AI technologies through mobile applications, ESP32-based smart streetlights, cloud connectivity, and machine learning analytics.

When a user presses the SOS button within the application, their GPS coordinates are immediately transmitted to a centralized Firebase cloud database. Nearby IoT-enabled smart streetlights switch to red emergency mode, and an audible buzzer is activated to increase public awareness. Simultaneously, police authorities receive real-time notifications through a monitoring dashboard that displays the user’s location, enabling faster emergency response.

Additionally, AI and Machine Learning based unsafe-zone analytics using Kernel Density Estimation (KDE) heatmaps and Random Forest risk assessment models identify recurring SOS incidents, dangerous time periods, and high-risk locations based on historical emergency data.

By integrating real-time IoT communication, cloud-based monitoring, smart infrastructure connectivity, and AI analytics, the proposed system creates a scalable public safety ecosystem suitable for smart city deployment. The architecture significantly reduces emergency notification response times through geographically distributed alerts and intelligent hotspot detection.

### Keywords

Public Safety, Smart SOS System, Internet of Things (IoT), ESP32, Firebase, Smart Street Lights, Kernel Density Estimation (KDE), Random Forest, Emergency Alert System, Real-Time Monitoring, Smart City Infrastructure, Machine Learning, GPS Tracking, Police Dashboard, Unsafe-Zone Heatmaps

# 1. Introduction

In today's urbanized world, public safety remains a significant concern. During emergencies such as harassment, accidents, theft, or medical incidents, individuals require immediate access to assistance. Traditional emergency systems often rely on manual reporting mechanisms or isolated notifications sent through mobile devices, resulting in delayed response times and limited situational awareness.

Advancements in IoT, cloud computing, mobile technology, and machine learning have enabled the development of smart public safety infrastructures capable of real-time monitoring and automated emergency communication. Existing safety applications primarily use GPS and GSM technologies for location tracking and emergency notifications. However, these systems generally lack intelligent analytics for identifying unsafe zones and predicting risks.

Recent smart city research has explored distributed IoT infrastructures, connected streetlight systems, centralized dashboards, and AI-driven hotspot detection methods. Machine learning techniques such as Kernel Density Estimation (KDE), clustering algorithms, and predictive analytics have proven effective in identifying high-risk locations and visualizing urban safety risks. Similarly, IoT-based emergency systems using ESP32 microcontrollers, GPS modules, cloud communication, and wireless alerts have demonstrated significant potential for real-time public safety applications.

This work presents VISION: Smart SOS Public Safety System, an integrated emergency response ecosystem comprising a mobile SOS application, ESP32-based smart streetlights, Firebase cloud communication, police monitoring dashboards, and AI-based unsafe-zone detection. Unlike conventional systems that only notify selected contacts, the proposed solution actively alerts nearby public infrastructure through smart streetlights and buzzer systems while simultaneously providing centralized police monitoring and intelligent hotspot analysis.

The primary objective is to bridge the gap between emergency reporting, public awareness, and intelligent urban safety infrastructure through real-time IoT communication and data-driven analytics.

# 2. Literature Review

The integration of IoT, machine learning, and cloud communication technologies has led to significant advancements in public safety systems. The VISION Smart SOS Public Safety System is inspired by several research studies focused on crime hotspot analytics, IoT emergency communication, smart streetlight systems, and real-time emergency monitoring.

The study "CHART: An Intelligent Crime Hotspot Detection and Real-Time Tracking Using Machine Learning" introduced a framework utilizing Kernel Density Estimation (KDE) heatmaps and Random Forest models to identify crime hotspots using historical police data. The framework enabled crime hotspot visualization and predictive risk monitoring. These techniques directly influenced the AI analytics module of the VISION system.

The research "Machine Learning-Based Evaluation of IoT-Supported Smart Safety Systems for Women and Children" demonstrated how GPS tracking and GSM communication improve emergency response systems through real-time alert transmission and location tracking. The proposed VISION system adopts a similar emergency communication workflow.

Another relevant study, "A Distributed Multi-Tier Emergency Notification System Utilizing Sensor-Based Detection of Emergency Events for Intelligent City Applications," presented a distributed emergency response architecture using IoT sensors, GPS modules, wireless communication, and centralized monitoring systems. The findings influenced the distributed architecture of the VISION platform, integrating mobile devices, Firebase cloud services, ESP32-based smart streetlights, and police dashboards into a unified real-time communication framework.

# 3. Problem Statement

Despite advancements in public safety technology, several challenges remain:

### i. Delayed Emergency Response

Most SOS systems rely on SMS or mobile notifications that may go unnoticed if recipients are not actively monitoring their devices.

### ii. Lack of Public Awareness Infrastructure

Existing safety applications primarily notify selected contacts without utilizing public infrastructure such as smart streetlights or audible alarms to attract immediate attention.

### iii. Limited Analysis of Unsafe Areas

Traditional systems generally lack AI-based analytics capable of identifying recurring unsafe zones, high-risk locations, and dangerous time periods.

### iv. Insufficient Real-Time Monitoring

Many emergency management systems do not provide centralized dashboards capable of tracking incidents geographically and supporting rapid emergency response.

### v. Lack of Smart City Integration

Most safety applications operate independently and do not integrate with IoT infrastructure, cloud services, and intelligent urban monitoring systems.

To address these issues, this research proposes the VISION Smart SOS Public Safety System, integrating mobile applications, ESP32 smart streetlights, Firebase cloud communication, police dashboards, and AI-based hotspot analytics.

# 4. Objectives

1. Develop a mobile SOS application capable of transmitting emergency alerts and real-time GPS data.

2. Design and implement IoT-enabled smart streetlights using ESP32 microcontrollers, RGB LEDs, and buzzers.

3. Utilize Firebase cloud services for communication between mobile devices, streetlights, and dashboards.

4. Create a centralized police monitoring dashboard for real-time emergency tracking.

5. Implement AI and machine learning techniques such as KDE and Random Forest for unsafe-zone analysis.

6. Analyze historical SOS data to identify dangerous locations and time periods.

7. Develop a scalable smart city public safety ecosystem integrating IoT, cloud computing, and intelligent analytics.

# 5. Methodology

The VISION system consists of five major components:

* Mobile SOS Application
* Firebase Cloud Database
* ESP32 Smart Streetlights
* Police Monitoring Dashboard
* AI-Based Analytics Module

The workflow follows five phases:

1. Emergency Detection and SOS Triggering
2. Cloud Communication
3. Smart Streetlight Activation
4. Police Dashboard Monitoring
5. AI-Based Unsafe-Zone Analysis

## 5.1 Emergency Detection and SOS Triggering

When a user presses the SOS button:

* Live GPS coordinates are captured
* Alert timestamp is generated
* Emergency data is transmitted to Firebase

The transmitted information includes:

* User ID
* Latitude
* Longitude
* SOS Status
* Alert Time

## 5.2 Communication Through Firebase

Firebase Realtime Database serves as the communication backbone by:

* Storing SOS alerts
* Synchronizing updates in real time
* Enabling communication between all system components
* Maintaining historical records for AI analysis

Communication Flow:

Mobile App → Firebase → ESP32 Streetlights & Dashboard

## 5.3 Smart Streetlight Alert Activation

Each smart streetlight includes:

* ESP32 Microcontroller
* RGB LED
* Buzzer
* GPS Coordinates
* Device ID

When an SOS alert is detected:

1. User coordinates are compared with streetlight locations.
2. The nearest streetlight is identified.
3. Blue LED switches to Red Emergency Mode.
4. Buzzer activates to attract public attention.

| Mode        | LED Status | Buzzer |
| ----------- | ---------- | ------ |
| Normal Mode | Blue ON    | OFF    |
| SOS Mode    | Red ON     | ON     |

## 5.4 Police Dashboard Monitoring

The dashboard provides:

* Live SOS Notifications
* User Location Tracking
* Emergency Timestamps
* Streetlight Monitoring
* Heatmap Visualization
* Emergency History Logs

Benefits include:

* Rapid Situational Awareness
* Incident Monitoring
* Emergency Response Coordination

## 5.5 AI-Based Unsafe Zone Analysis

Historical Firebase data includes:

* Alert Frequency
* GPS Coordinates
* Incident Time
* Repeated Hotspots

### Kernel Density Estimation (KDE)

KDE is used to generate heatmaps by:

* Collecting SOS locations
* Applying density kernels
* Combining overlapping densities
* Visualizing hotspot concentrations

Risk Levels:

* Red Zone – High Risk
* Yellow Zone – Moderate Risk
* Green Zone – Low Risk

### Random Forest Analysis

Random Forest is used to identify:

* Recurring unsafe times
* Repeated incidents
* Risk assessment patterns
* Potential danger zones

# 6. Implementation

## 6.1 Hardware Implementation

| Component       | Purpose               |
| --------------- | --------------------- |
| ESP32 / NodeMCU | Main IoT Controller   |
| RGB LED         | Streetlight Indicator |
| Buzzer          | Emergency Alarm       |
| Breadboard      | Circuit Assembly      |
| Jumper Wires    | Connections           |
| WiFi Network    | Cloud Communication   |

## 6.2 Software Implementation

| Software                   | Purpose            |
| -------------------------- | ------------------ |
| Blynk                      | Prototype Testing  |
| Firebase                   | Cloud Database     |
| Arduino IDE                | ESP32 Programming  |
| Flutter / MIT App Inventor | Mobile Application |
| HTML, CSS, JavaScript      | Police Dashboard   |
| Python                     | AI Analytics       |

## 6.3 Firebase Integration

Sample Data Structure:

```json
{
  "sos": 1,
  "latitude": 12.9716,
  "longitude": 77.5946,
  "time": "10:45 PM"
}
```

Firebase enables:

* Live synchronization
* Device communication
* Dashboard updates
* Historical data storage

## 6.4 Police Dashboard Features

* Active SOS Alerts
* User Location Tracking
* Alert Timestamps
* Emergency Status Monitoring
* Unsafe-Zone Heatmaps
* Emergency Logs
* Google Maps Integration

## 6.5 AI Analytics

Libraries Used:

| Library      | Purpose              |
| ------------ | -------------------- |
| Pandas       | Data Processing      |
| NumPy        | Numerical Operations |
| Scikit-learn | Machine Learning     |
| Folium       | Heatmap Generation   |
| Matplotlib   | Visualization        |

### KDE Heatmaps

Input:

* Latitude
* Longitude
* Alert Frequency

Output:

* Risk Heatmaps

### Random Forest Model

Input:

* Incident Timing
* Alert Density
* Historical Patterns

Output:

* Risk Predictions
* Hotspot Analysis

## 6.6 Overall System Workflow

Mobile App
↓
Firebase Cloud
↓
ESP32 Smart Streetlights
↓
Police Dashboard
↓
AI Analytics & Heatmaps

# 7. Results and Analysis

(To be completed after implementation and testing)

# 8. Discussion

(To be completed)

# 9. Conclusion

(To be completed)

# 10. Future Scope

(To be completed)

# Acknowledgements

(To be completed)

# References

[1] CHART: Intelligent Crime Hotspot Detection and Real-Time Tracking Using Machine Learning. Computers, Materials and Continua, Vol. 81, No. 3, 2024. DOI: 10.32604/cmc.2024.056971

[2] Evaluation of IoT-Based Smart Safety Systems for Women and Children Using Machine Learning Techniques. Scientific Reports, Vol. 16, Article 87, 2026. DOI: 10.1038/s41598-025-29146-4

[3] A Distributed Multi-Tier Emergency Alerting System Exploiting Sensor-Based Event Detection to Support Smart City Applications. Sensors, Vol. 20, No. 1, 2020. DOI: 10.3390/s20010170

[4] Design of Smart LED Streetlight System for Smart City with Web-Based Management System. International Journal of Scientific & Technology Research (IJSTR).

[5] Developing Real-Time IoT-Based Public Safety Alert and Emergency Response Systems. Journal/Conference Paper on IoT-Based Emergency Communication and Public Safety Systems.
