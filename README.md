
# Context Monitoring App

## Demo Video

Watch the demo video showcasing the features of the project: [YouTube (unlisted)](https://youtu.be/w-4QbcUBO5A).

## Introduction

This project involves developing a context-sensing application for real-time health monitoring, such as heart rate and respiratory rate collection. It integrates sensors, data storage, and feedback mechanisms to provide useful insights about the user’s health.

## Question 1: Specifications for Context Sensing Application
After reading the Health-Dev file, we need to have these specifications for the context sensing application.

### 1.1 Sensor Specifications

- **Node ID**: Provide unique IDs for each sensor in the Body Sensor Network (BSN).
- **Platform Type**: Specify the sensor platform for each type (e.g., Shimmer for ECG, TelosB for temperature and humidity).
- **Sensor Type**: Define what physiological signals each sensor captures (e.g., ECG for heart rate, accelerometer for respiratory rate).
- **Sampling Frequency**: Specify how often the data is collected by the sensors.
- **Computation Requirements**: Specify any data processing on the sensor side (e.g., peak detection for heart rate or correlation for temperature and humidity).
- **Communication Protocol**: Choose between Bluetooth or ZigBee for communication between the sensors and the smartphone.
- **Execution Sequence**: Define the order in which algorithms should be applied to sensor data (e.g., apply peak detection before heart rate calculation, then STD calculation for ECG).

### 1.2 Network Specifications

- **Network Topology**: Specify the routing table and network topology to define how data should be routed between sensors.
- **Energy Management**: Choose a radio duty cycle to balance energy consumption and performance.

### 1.3 Smartphone Specifications

#### 1.3.1 UI Components

- Buttons to start/stop heart and respiratory rate collection.
- TextViews to display heart rate and respiratory rate data.
- Graphs to visualize data over time.
- A spinner (dropdown) list of symptoms.

#### 1.3.2 Communication with Sensors

- Specify how the smartphone communicates with sensors, including commands for starting/stopping data collection, changing sampling frequencies, and receiving sensor data.
- Define how the smartphone processes sensor data (e.g., storing it locally after receiving it).
 ![image](https://github.com/user-attachments/assets/87478fde-905e-4e1e-85be-9b09f5d232a6)

---

## Question 2: Using the bHealthy Application Suite for Feedback
From the bHealthy application suite, we could use the feedback mechanism to monitor the Heart Rate and respiratory Rate, at the second page, we gonna collect the user's feeling of serveral symptons to give them feedback.Then collecting users' longterm data, so that we could provide the users' report when they need to obsersve their body health.

### 1. Heart Rate & Respiratory Rate Monitoring

- **Heart Rate Collection**: After collecting users' heart rates, continuously monitor the heart rate using physiological sensors (e.g., ECG) and feed this data into the bHealthy suite’s feedback loop.
- **Respiratory Rate Collection**: Track respiratory rate using an accelerometer sensor, then provide feedback based on the user’s state (e.g., relaxed, stressed).

### 2. Symptom Data Integration

- **Contextual Data**: Since we already store user symptoms in a local database, we can integrate this data with bHealthy’s assessment application. For example, symptoms like fatigue or anxiety can trigger feedback or suggestions like relaxation exercises.

### 3. Physiological State Assessment

- bHealthy analyzes physiological data to assess the user’s state (e.g., boredom, excitement, frustration). After collecting this data, a function could help generate wellness reports. The app could also suggest activities (e.g., relaxation or focus exercises) when abnormal heart rate or respiratory rate data is detected.

### 4. Modeling the User’s Well-being


- **Wellness Model**: The app could develop a personalized wellness model using user data. This model would adjust based on historical data and provide tracking graphs for the user to monitor their health. The app could also provide feedback based on the user's unique physiological profile.

---

## Question 3: Mobile Computing Beyond App Development

After completing Project 1 and reading both papers, I’ve realized that mobile computing involves much more than just app development. It encompasses:

- **Real-time Health Monitoring**: The system involves collecting and analyzing physiological data in real-time.
- **Context Awareness**: Mobile computing integrates data from sensors to provide context-aware interactions and feedback.
- **Data Integration**: It brings together hardware (sensors), software (applications), networks, and data processing for a seamless, smart user experience.

Mobile computing involves real-time data analysis, sensor integration, and user feedback mechanisms. It’s more than just building an app; it’s about creating a smart system that interacts with its environment and user to deliver personalized and useful experiences.

---




