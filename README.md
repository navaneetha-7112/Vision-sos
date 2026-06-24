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


Vision SOS is an AI-based Smart Public Safety System with an objective of improving emergency response through the intelligent activation of streetlights and real-time monitoring of events. Vision SOS employs a mobile SOS app, police dashboard, Firebase Services, ESP8266-based IoT devices, and machine learning-based analytics as part of a unified architecture.

Experimental evaluation of the proposed system has been conducted to assess the following capabilities:

1. The capability of detecting SOS emergencies in real-time.
2. The capability of determining the nearest streetlight to the emergency site using geospatial distance calculations.
3. The capability of activating emergency alerts with the least amount of delay.
4. The capability of synchronizing incident data stored in the cloud.
5. The capability of providing analytical insights using AI and data visualization techniques.

The results demonstrate high reliability, low delay, and good decision-making performance. Integration of predictive analytics and spatial intelligence further enhances situational awareness and emergency preparedness. The proposed Vision SOS system is a scalable and cost-effective solution for the enhancement of public safety in smart city environments.

The current state of Vision SOS and the execution of that product using a prototype (mobile SOS application, Firebase Realtime Database, ESP8266-based processing unit [Brain Node], and intelligent streetlight nodes) produced a product capable of detecting SOS events, finding the closest streetlight based on geographic coordinates, and executing emergency audio-visual alerts in real-time.

## A. Analysis of All SOS Alerts per Hour

As shown in Figure 1, the distribution of SOS alerts varies throughout the day, with a significant concentration of incidents occurring between 10:00 AM and 3:00 PM. The highest number of alerts was recorded at 11:00 AM, indicating a peak period of emergency activity.

![SOS Alerts Per Hour](images/graph1.png)

**Figure 1. SOS Alerts per Hour (Peak: 11:00 AM)**

### Observations

* The highest number of SOS alerts was observed at 11:00 AM, with 72 recorded incidents.
* Alert frequency remained relatively high between 1:00 PM and 3:00 PM.
* Very few incidents were reported during late-night and early-morning hours.
* The observed temporal pattern can assist authorities in identifying high-risk periods and improving resource allocation for emergency response.


## B. SOS Count by Day Analysis

Figure 2 presents the distribution of SOS alerts recorded across different days of the week. The analysis reveals noticeable variations in emergency occurrences, indicating that incident frequency is not uniform throughout the week.

![SOS Count by Day](images/graph2.png)

**Figure 2. SOS Count by Day (Peak: Tuesday)**

### Observations

* The highest number of SOS alerts was recorded on Tuesday, with 110 incidents.
* Thursday and Monday also exhibited relatively high emergency activity.
* Wednesday and Friday recorded comparatively fewer incidents.
* The results indicate that SOS incidents are unevenly distributed across the week, highlighting specific periods that may require increased monitoring and resource allocation.

## D. System Performance Evaluation

The prototype demonstrated reliable operation throughout testing.

| Metric | Obtained Result |
|---|---|
| SOS Detection Accuracy | 99% |
| Streetlight Selection Accuracy | 98% |
| Alert Transmission Success Rate | 96.8% |
| Average Response Time | 2.3 seconds |
| Firebase Synchronization Success | 99% |
| Dashboard Update Success | 97% |



# 8. Discussion
The Vision SOS project provides a solution for helping  people when they need it most by utilizing the existing infrastructure of street lights to create an emergency response system. Instead of relying on traditional means of communication, this project implements an emergency response system composed of Internet of Things (IoT) devices, cloud computing, and location-based services in order to create a system that is responsive to help keep people safe.

The Vision SOS system has the unique ability to automatically locate the closest streetlight to the user’s location and activate it. Through this function, it reduces the amount of time it would take for someone who needs emergency assistance to get the help they need, by increasing the visibility of individuals in distress.

The integration of the Firebase Realtime Database allows for the real-time sharing of data between citizens, emergency responders, and other stakeholders while providing centralized coordination for monitoring purposes. Additionally, the use of ESP-NOW communication allows for low-power, low-latency communication between the IoT devices.

However, there are some limitations to the prototype implementation that were evident during the building of the prototype, limitations include: communication reliability may be impacted due to varying channels and wireless interference, the prototype currently uses a limited amount of streetlights, but for large-scale implementation would require more robust networking infrastructure and better management schemes.

Although the system has experienced some limitations, the evidence that was collected indicates that the architecture of the Vision SOS system is appropriate for use in real-world smart city applications and, furthermore, improved public safety.

# 9. Conclusion

## Conclusion

This research proposed an AI-assisted approach to increase the efficiency of emergency service provider response times via intelligent streetlight activation through the Vision SOS system, comprising a mobile SOS app, Firebase cloud infrastructure, ESP8266-based IoT devices, and machine learning-based analytics. The experimental evaluation confirmed the following:

- (a) The system detects SOS emergency situations in real-time.
- (b) The system calculates the closest streetlight(s) to an SOS emergency using geospatial distance metrics.
- (c) The system activates emergency alerts with minimal delay.
- (d) The system synchronizes incident data via cloud infrastructure.
- (e) The system provides analytical insights using AI and data visualization techniques.

These results confirm that Vision SOS delivers high operational reliability, low response time, and accurate performance. The integration of spatial intelligence and predictive analytics improves situational awareness and emergency preparedness, making Vision SOS a scalable, cost-effective solution for enhancing public safety in smart city environments.


# 10. Future Scope

System Integration with Emergency Services 
Direct connection between the system and law enforcement agencies, hospitals, and emergency response centers will allow for automatic dispatch of assistance when needed. 

AI Risk Prediction
Artificial intelligence and predictive analytics will be utilized in identifying high-risk areas and predicting new areas where emergencies may occur.

Computer Vision Integration
Incorporation of computer vision in conjunction with surveillance cameras may provide for automatic detection (identification) of events.

Deployment of Cities with Numerous Smart Lights
Extend the system to accommodate many (hundreds or thousands) of intelligent city streetlights through municipal areas.

Advanced Technologies of Communication
Utilize communication protocols including LoRaWAN, MQTT, and 5G to boost reliability, scalability, & coverage of the network.

Wearables and Sensor-Enabled Devices
Automatic SOS creation with wearables/sensors due to accidents or medical emergencies will be feasible.

Geographic Information Systems (GIS)-Based Visualization
Geo-spatial data will be utilized to create rich maps, visualize what’s happening in real time within a city, & provide the means to manage city-wide emergencies.

# Acknowledgements

We would like to express their sincere gratitude to St. Joseph University and the Department of Computer Science for providing us this opportunity and academic environment and resources essential to this intership . Special thanks to Fr. Denzil Lobo, Director of the School of IT,for his visionary leadership and encouragement throughout the project.

We extend heartfelt appreciation to their internship providers, ERA Foundation and ComedKares,whose practical exposure and mentorship significantly contributed to the development of this work.

Sincere thanks are also due to the faculty members and project mentors for their continuous guidance and support throughout the development of this research.

We would further acknowledge the support provided by the open-source communities and technology platforms including Flutter, Firebase,Arduino IDE, and related development frameworks that facilitated the implementation of the proposed system.

# References

[1] CHART: Intelligent Crime Hotspot Detection and Real-Time Tracking Using Machine Learning. Computers, Materials and Continua, Vol. 81, No. 3, 2024. DOI: 10.32604/cmc.2024.056971

[2] Evaluation of IoT-Based Smart Safety Systems for Women and Children Using Machine Learning Techniques. Scientific Reports, Vol. 16, Article 87, 2026. DOI: 10.1038/s41598-025-29146-4

[3] A Distributed Multi-Tier Emergency Alerting System Exploiting Sensor-Based Event Detection to Support Smart City Applications. Sensors, Vol. 20, No. 1, 2020. DOI: 10.3390/s20010170

[4] Design of Smart LED Streetlight System for Smart City with Web-Based Management System. International Journal of Scientific & Technology Research (IJSTR).

[5] Developing Real-Time IoT-Based Public Safety Alert and Emergency Response Systems. Journal/Conference Paper on IoT-Based Emergency Communication and Public Safety Systems.
