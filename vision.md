<div align="center">

<img src="https://www.sju.edu.in/assets/img/st-joseph-university-logo.png" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://www.erafoundationindia.org/images/logo.svg" height="80" style="background:white; padding:8px; margin:0 16px;" />
<img src="https://comedkares.org/wp-content/uploads/2023/04/Comedkares-Logo-EPS.png" height="80" style="background:white; padding:8px; margin:0 16px;" />

</div>

\---

# {{Project Title}}

\# VISION: AN IoT AND AI ENABLED SMART SOS PUBLIC SAFETY SYSTEM



<div align="center">

\*\*Navaneetha M\*\*, MCA, USN \&nbsp;·\&nbsp;

\*\*R Nataraj\*\*, MCA, USN \&nbsp;·\&nbsp;

\*\*Sowmya J\*\*, MSc BDA, USN \&nbsp;·\&nbsp;

\*\*V Kamala Kannan\*\*, MCA, USN \&nbsp;·\&nbsp;

\*\*Vijaya M\*\*, MSc BDA, USN

</div>---

## Abstract

Public safety systems frequently encounter issues with late responses to emergencies due to a lack of systems for alerting about real time emergencies as well as an intelligent awareness infrastructure.    Most SOS applications currently in use only send alerts to specific people or organizations, yet do nothing to proactively alert individuals in the immediate vicinity of the emergency or dynamically alter based on real-time information about unsafe areas. This work proposes VISION (Smart SOS Public Safety System), a whole new way for providing emergency response through a combination of IoT and AI technologies involving mobile apps, smart streetlights based on the ESP32 microcontroller, the internet, and machine learning analytics.



When an individual pushes the SOS button within the app, the GPS coordinates of that person will be sent at that moment to a centralized Firebase cloud data storage. Nearby IoT-enabled smart street lamps will be switched to red emergency mode, and an audible buzzer will go off to create public awareness at that very moment. Police will also be notified through the control dashboard via a real-time live emergency notification and the ability to watch and see the person’s location, allowing for quicker response to the emergency.



In addition, AI/ML-based unsafe-zone analytic functions using Kernel Density Estimation (KDE) heat maps and Random Forest-based risk assessments to identity repetitive SOS incidents or danger hours from historic emergency data has been implemented in order to predictively monitor the public safety risks of accidents, and to provide advanced visualisations of urban risk.



Through the combination of real time IoT communications, cloud-based monitoring, smart Infrastructure connectivity, and AI Analytics, a scalable public safety ecosystem, suitable for deployment in a smart city, has been created. The proposed architecture has been shown to reduce emergency notification response times substantially with the implementation of geographically distributed emergency notification and intelligent hotspot detection.

\---

## Keywords

Public Safety, Smart SOS System, Internet of Things (IoT), ESP32, Firebase, Smart Street Lights, Kernel Density Estimation (KDE), Random Forest, Emergency Alert System, Real-Time Monitoring, Smart City Infrastructure, Machine Learning, GPS Tracking, Police Dashboard, Unsafe-Zone Heatmaps.

\---

## 1\. Introduction

In today's world, many people are living in cities, but at the same time they are worried about how safe they will be when something happens. When there is an emergency (e.g., someone is being harassed, hurt or there is a medical emergency) you need to have a way to get help instantly. Most Emergency systems rely on people to report what is happening manually (call 911) or rely on isolated alerts sent from your mobile device to have an emergency responder dispatched to your location. Because of this, response times are much longer than what they could/should be and the nearby citizens and authorities do not have real time situational awareness.



The new technologies that have come about from IoT, Cloud computing, mobile devices, and Machine Learning can be developed into new Smart Public Safety infrastructure that can provide real time surveillance of Public Safety issues and establish automated methods of communication with Local Public Safety agencies during an emergency. Presently available Women Safety Applications and IoT Alert Devices typically will utilize GPS and GSM technologies (i.e. locating the user's device through the use of Satellite Mapping or Cellular Network) for sending/outgoing emergency alerts and notifications. However, the present Woman Safety Applications and IoT Alert Devices do not have Intelligent Analytics that can identify unsafe zones for women because the current methods used provide for static vs. dynamic alert methods.



Research regarding smart cities increasingly investigates the use of distributed IoT infrastructures (for example: connected street light systems, centralized dashboards, \& AI-based analyses of urban “hot spots” for safety improvement).  In particular, machine learning (e.g.: kernel density estimation \[KDE], clustering algorithm, predictive analytic approaches) have produced positive results in identifying crime “hot spots” and visualizing spatial risk.  Likewise, IoT-driven emergency systems (i.e.: using ESP32 microcontrollers, GPS modules, cloud-based communications, \& wireless alert systems) have demonstrated the potential for developing real-time architectures for public safety.



This work presents VISION: Smart SOS Public Safety System, an integrated emergency response ecosystem that incorporates a mobile SOS application, ESP32-based smart street lights, Firebase for cloud-based communication, police monitoring dashboards, \& AI-based identification of dangerous locations.  Unlike traditional public safety applications that simply notify a select group of individuals, the proposed public safety system would be able to actively notify nearby public infrastructure (by activating smart street lights \& triggering buzzer alarms), while at the same time, providing centralized police monitoring \& machine learning-based detection of crime “hot spots”.



The goal of this system is to facilitate the relationship between the reporting of emergencies, awareness by the public, and intelligent urban systems (through the application of real-time IoT communications) while developing data-driven analytics concerning public safety.

\---

## 2\. Literature Review

The integration of Internet of Things (IoT) capability, machine learning techniques, and cloud communication technologies has led to recent advancements in public safety systems that improve emergency response times and enhance urban safety monitoring through smart city infrastructure. The VISION Smart SOS Public Safety System was developed based on the findings of five primary research studies that investigate crime hotspot analytics, IoT emergency systems, smart street light management, and real-time emergency communication.



Research described in the document "CHART: An Intelligent Crime Hotspot Detection and Real-Time Tracking Using Machine Learning" introduced the intelligent crime analytics framework. This framework uses Kernel Density Estimation (KDE) heatmaps and Random Forest models to identify crime hotspots based on historical data provided by police departments \[1]. The proposed system performs spatial crime within the framework; visualization of crime hotspots; and predictive monitoring of unsafe areas utilizing machine learning techniques. The use of KDE heatmaps effectively demonstrates how high-risk areas can be visually represented, while Random Forest models will assist in the analysis of crime patterns and the prediction of hotspots. These examples were significant influences on the AI analytics module of the proposed VISION system. The AI module of the VISION system will analyze SOS alert data to identify recurrent unsafe areas and dangerous times.



The paper "The Machine Learning-Based Evaluation of IoT-Supported Smart Safety Systems for Women and Children" developed a model of how IoT devices like GPS tracking and GSM communications can improve emergency response systems \[2]. The study also showed the possibility of sending emergency alerts in real time through IoT-enabled communication. The main purpose of this study was to enhance the safety of women and children by providing them with a means of automatically communicating an emergency situation, as well as locating them in real time. The results of this study provided the inspiration for the emergency alert workflow and IoT communication architecture upon which our proposed VISION Smart SOS Public Safety System is built.



The second supporting paper, "A Distributed Multi-Tier Emergency Notification System Utilizing Sensor-Based Detection of Emergency Events for Intelligent City Applications," \[3] presented a distributed emergency response architecture that includes IoT sensors, wireless communication systems, GPS modules, and centralized monitoring platforms for use in smart city environments. The findings of this study demonstrated how multiple IoT nodes can work together within a unified communication framework, allowing for efficient communication of emergency alerts and contributing to the management of emergencies in smart cities. The proposed distributed architecture of the proposed system will consist of a combination of mobile devices, Firebase cloud communication, ESP32-based smart street lights and police dashboards that will work together in real time.

\---

## 3\. Problem Statement

Though many improvements have been made in public safety technology, many existing emergency response systems have issues limiting their overall effectiveness.



**i.** Emergency Response is Being Delayed

Current SOS Systems use a lot of SMS or Mobile Notification systems to reach out to people in emergencies. However, unless an individual is already looking at their mobile device or watches the notifications, they do not initially see them and more importantly, they do not notice they have now been sent.



**ii.** Lack of Public Awareness + Public Infrastructure

The majority of safety applications that exist today are working to notify only particular contacts and are not actively working to alert other people by any visual public infrastructure (i.e., smart street lights) and audible emergency alarms.



**iii.** Real-Time Analysis of Unsafe Areas

Legacy systems are unable to provide any analysis of past emergency response data to identify continuous high-risk areas, risky times, or unsafe areas in urban areas using real time AI-Based Analytics methods.



**iv.** Real-Time Monitoring Is Limited

Some emergency management systems lack centralized dashboards that can actively track incidents geographically while also allowing for the rapid response of officers to incidents through live multimodal emergency alerts and other live monitoring options.



**v.** Safety Systems Are Disconnected from Smart Cities

For the most part, safety apps do not integrate and use available data gathered from the collection of IoT devices, cloud-based services, and advanced urban monitoring systems, all of which fall under the broad category of smart city infrastructure.



This research solves the previously mentioned issues by creating a “Smart SOS Public Safety System” that integrates Mobile Due Process, ESP32 Smart Street Lights, Firebase cloud based communications, Police Dashboards, and the use of AI-based hotspot analytics for the purpose of effectively monitoring safety in urban environments.



## 4\. Objectives

The primary goals of the proposed VISION Smart SOS Public Safety System include:



(i) Creation of a mobile SOS application for real-time transmissions of SOS messages, including emergency alerts and real-time GPS location data to a centralized cloud platform.



(ii) Design and build an IoT-enabled smart streetlight prototype using ESP32 microcontrollers, RGB LEDs and buzzer systems to create awareness of public safety emergencies.



(iii) Use Firebase Cloud messaging to distribute synchronizations between the mobile app, smart streetlights, and Police Monitoring dashboard.



(iv) Develop a centralized Police/Admin dashboard to provide Police and admin personnel the ability to view in real-time all emergency alerts, user locations, and streetlight operational status.



(v) Develop AI/ML-based unsafe-zone (analytical evaluation) of heat maps using Kernel Density Estimations (KDE) and Random Forest models for hotspot detection and risk assessment.



(vi) Analyze the historical data on SOS alerts to determine dangerous zones and times of the day based on identified patterns/risk metrics from an urbanization perspective.



(vii) Create a scalable smart city public safety ecosystem that combines IoT infrastructure, cloud-based communications, and intelligent emergency analytics for future urban safety implementations.



## 5\. Methodology

VISION Smart SOS Public Safety System operates using an integrated IoT and AI-based architecture. This new system incorporates five components: the mobile SOS App; the Firebase Cloud; the smart streetlight with integrated ESP32 technology; the central police dashboard; and machine learning (ML) for hotspot analytics to support hotspot monitoring.



The overall system workflow consists of five phases:



1\. Emergency detection, GPS/location acquisition, and SOS trigger.

2\. Cloud communication in real time.

3\. Smart streetlight alert activation.

4\. Police dashboard monitoring.

5\. AI-based unsafe zone analytics.



**5.1 Emergency Detection and SOS Triggering**



The system begins with the mobile application developed for public users. During emergency situations such as harassment, accidents, thefts, or medical emergencies, the user presses the SOS button available within the application.



When the SOS button is activated:

1.the application captures the live GPS coordinates of the user

2.timestamp and alert status are generated

3.emergency data is transmitted to the Firebase Realtime Database.



The transmitted data includes:

1.user ID

2.latitude

3.longitude

4.SOS status

5.time of alert

The mobile application acts as the primary interface between the user and the emergency response infrastructure.



**5.2 Communication with Firebase Cloud**

The Firebase Realtime Database is the primary means of communication for all system components.

It accomplishes the following tasks:

\- It stores SOS alerts

\- It updates emergency status in Real Time

\- It provides communication for the mobile app, the ESP32 Street Lights and Police Dashboard

\- It retains all historical emergency records for AI analysis.



Each time an SOS alert is generated:

Mobile App → Firebase → ESP32 \& Dashboard.

Firebase provides real-time updates to all connected devices without requiring manual refresh action.

Alerting a Smart Street Light through an SOS Alert.



**5.3 Smart Street Light Alert Activation**



The IoT Layer in the smart street light is formed of ESP32 Based Smart Street Light Prototypes using (RGB) Light Emitting Diode's (LEDs) and buzzer systems.

Every smart street light has:

1\.a unique device ID and

2\.geographic coordinates.

The ESP32 Microcontroller is continually checking Firebase for SOS Alerts.



When an SOS alert is received:

1\.the GPS coordinates of the user who submitted the SOS alert are compared to the GPS coordinates of the smart street lights registered in the Firebase Database

2\.the closest registered smart street light is determined,

3\.the nearest smart street light goes from being in non-emergency blue mode to being in emergency red alert mode,

4\.the buzzer or siren at the nearest smart street light will sound in order to attract public attention to assist the person who submitted the SOS alert.



This improves:

emergency visibility to the emergency responders

the public awareness of the emergency

the ability of nearby citizens to respond to the emergency.



&#x20;**Mode        	LED Status   	Buzzer** 

&#x20;Normal Mode 	Blue LED ON  	OFF    

&#x20;SOS Mode     	Red LED ON  	ON     



The ESP32 devices communicate using WiFi and Firebase cloud synchronization.





**5.4 Overview of Police vs. Admin Monitoring with a Dashboard**



The central monitoring of emergencies has been done through a developed Page that will show the most current emergency reports.



The following are some of the abilities that it will provide for each user on the dashboard:

1\.Live SOS Notifications

2\.Locate User via GPS

3\.Store Emergency Timestamp for Each SOS Alert

4\.Locate All Active Street Lights

5\.View Unsafe Areas via Heat Map

6\.Show Emergency History for User



When an SOS Alert is sent data goes from firebase to Police Dashboard

The dashboard will automatically apply any type of data needed to aid in responding to emergencies.



This Dashboard will allow for:

1\.Rapid Situational Awareness

2\.Monitoring Incidents

3\.Coordinating Emergency Response



**5.5 AI/ML Based Unsafe Zone Analysis**

AI portion of the system performed analysis of past SOS alert data to identify unsafe areas and repeating patterns of emergency incidents.



Historical data in Firebase contains:

\- Frequency of Alerts

\- GPS Coordinates

\- Time of Incidents

\- Repeated Hot Spot Area



Two analytical methods were used:



**5.5.1 Kernel Density Estimation (KDE)**



Kernel Density Estimation was used to create heat map representation of Unsafe Zones.



KDE process takes place through:

\- Collecting GPS location data from SOS incidents

\- Adding a density kernel around each incident point

\- Overlapping with other density kernels

\- Creating a heat map of Hot Spots.



Areas of concentration (high SOS incidence) can be identified as:

\- Red Zones (high risk)

\- Yellow Zones (moderate risk)

\- Green Zones (low risk).



KDE can be used:

\- To analyze emergency events spatially,

\- Identify Hot Spots,

\- Map visual representation of Unsafe Zones.



**5.5.2 Random Forest Methodology** 



The Random Forest methodology provides the following analyses for the fire service:

1\.recurring unsafe times

2\.repeated incidents of an emergency nature

3\.risk assessment.



The Random Forest methodology includes:

1\.historical records of alerts

2\.time sensitive incidents

3\.geographic information of incidents.



The outputs from the Random Forest methodology assist in identifying:

periods of high risk

patterns of repeated emergency responses

areas of potential unsafe conditions.



## 6\. Implementation

The implementation of the proposed VISION Smart SOS Public Safety System is divided into hardware implementation, software implementation, cloud integration, dashboard development, and AI analytics implementation.



**6.1 Hardware Implementation**

The hardware prototype consists of:



&#x20;**Component        Purpose**                 

&#x20;ESP32 / NodeMCU  Main IoT controller     

&#x20;RGB LED          Street light indication 

&#x20;Buzzer           Emergency siren         

&#x20;Breadboard       Circuit assembly        

&#x20;Jumper Wires     Connections             

&#x20;WiFi Network     Cloud communication   

&#x20; 

The ESP32 microcontroller is programmed using Arduino IDE and connected to Firebase through WiFi communication.



**6.1.1 Smart Street Light Prototype Description**

The smart street light prototype is made up of:

\* a blue indicator light, which indicates the light is functioning normally

\* a red indicator light, which indicates an SOS alert is currently active

\* a buzzer, which notifies users with sound when an emergency is happening.



The ESP32 continuously checks for SOS updates in Firebase.





**6.2 Software Implementation**

The software layer includes:

&#x20;**Software**                    **Purpose**           

&#x20;Blynk                       Prototype testing 

&#x20;Firebase                    Cloud database    

&#x20;Arduino IDE                 ESP32 programming 

&#x20;Flutter / MIT App Inventor  Mobile app        

&#x20;HTML/CSS/JS or Flutter      Police dashboard  

&#x20;Python                      AI analytics      





**6.2.1 Mobile Application**

The mobile application includes:

SOS button

GPS location access

emergency alert transmission

user authentication



**Workflow:**

User presses SOS

&#x20;      ↓

GPS location captured

&#x20;      ↓

Data sent to Firebase





**6.2.2 Blynk Integration**



Initially, Blynk IoT platform is used for:

testing LEDs

testing buzzer activation

verifying ESP32 cloud communication.



The Blynk button controls:

normal mode

SOS mode



**6.3 Firebase Integration**

Firebase Realtime Database acts as the communication backbone.

Stored data structure:



{

&#x20; "sos": 1,

&#x20; "latitude": 12.9716,

&#x20; "longitude": 77.5946,

&#x20; "time": "10:45 PM"

}



Firebase enables:

1\.live synchronization

2\.device communication

3\.dashboard updates

4\.historical data storage.



The selection of the nearest streetlight will consist of the following elements:

1\.Receive user GPS coordinates

2\.Compare these to the stored coordinates of all streetlights

3\.Calculate the distance from each streetlight to the user's GPS coordinates

4\.Activate the closest ESP32 device

This functionality reduces non-essential alerts and will provide a more accurate indication of an emergency for a specific location.



Police Dashboard Implementation.



The police dashboard will show:

1\.Active SOS alerts

2\.The location of user(s)

3\.The timestamp of the alert

4\.The current status of the emergency

5\.A heatmap showing unsafe areas

6\.Other features include:

7\.Real-time firebase updates

8\.Google Maps integration

9\.Emergency logs

10\.Heatmap showing hotspots.





**6.6 AI Analytics Implementation**

Historical SOS data is exported from Firebase and analyzed using Python.

&#x20;**Library       Purpose**              

&#x20;Pandas        Data processing      

&#x20;NumPy         Numerical operations 

&#x20;Scikit-learn  ML models            

&#x20;Folium        Heatmaps             

&#x20;Matplotlib    Visualization        





**6.6.1 KDE Heatmaps**

Kernel Density Estimation generates density-based unsafe-zone maps.



Input:

latitude

longitude

alert frequency.



Output:

risk heatmaps.

6.6.2 Random Forest Model



Random Forest processes:

incident timing

alert density

historical patterns.



Output:

risk predictions,

repeated hotspot analysis.





**6.7 Overall System Workflow**

Mobile App

&#x20;    ↓

Firebase Cloud

&#x20;    ↓

ESP32 Smart Street Lights

&#x20;    ↓

Police Dashboard

&#x20;    ↓

AI Analytics \& Heatmaps



The implementation demonstrates a scalable real-time public safety architecture integrating IoT communication, cloud synchronization, smart infrastructure, and machine learning-based analytics for emergency response enhancement.







## 7\. Results \& Analysis

\---









## 8\. Discussion

\---







## 9\. Conclusion

\---





## 10\. Future Scope

\---





## Acknowledgements







## References

\[1] CHART: Intelligent Crime Hotspot Detection and Real-Time Tracking Using Machine Learning, Computers, Materials and Continua, vol. 81, no. 3, pp. 4171–4194, 2024. DOI: 10.32604/cmc.2024.056971.



\[2] Evaluation of IoT Based Smart Safety Systems for Women and Children using Machine Learning Techniques, Scientific Reports, vol. 16, Article 87, 2026. DOI: 10.1038/s41598-025-29146-4.



\[3] A Distributed Multi-Tier Emergency Alerting System Exploiting Sensors-Based Event Detection to Support Smart City Applications, Sensors, vol. 20, no. 1, p. 170, 2020. DOI: 10.3390/s20010170.



\[4] “Design of Smart LED Streetlight System for Smart City with Web-Based Management System,” International Journal of Scientific \& Technology Research (IJSTR), Smart City and IoT-based Streetlight Management Research Paper.



\[5] “Developing Real-Time IoT-Based Public Safety Alert and Emergency Response Systems,” Journal/Conference Paper on IoT-based Emergency Communication and Public Safety Systems.

