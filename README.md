# FitLife: MATLAB-Powered Fitness Tracker
**Developed by:** BESTME
**Powered by:** MATLAB

---

## 📌 Project Objective
The primary goal of this project is to evaluate the effectiveness of a workout and provide detailed information regarding user activity. By analyzing sensor data, the application identifies physical behaviors and calculates key performance metrics.

## 🛠 Key Features
* **Activity Classification**: Automatically detects if a user is **Sitting**, **Walking**, or **Running** using a trained model. 
* **Metric Tracking**: Calculates the total **Number of Steps** and **Calories Burned**. 
* **Visual Mapping**: Generates an **Exercise Route** using GPS data plotted on geographic axes. 
* **Performance Analysis**: Provides velocity (speed) and acceleration over time graphs.

## 📊 Data Collection & Sensors
The system utilizes two primary sensors to gather data: 
* **GPS**: Records Latitude and Longitude to track the exercise route and assist in step counting. 
* **Accelerometer**: Measures 3-axis acceleration ($X, Y, Z$ in $m/s^2$) at a frequency of 10 Hz to identify movement patterns.

## 🤖 Machine Learning Implementation
The project employs a supervised learning approach to classify activities.
* **Model Selection**: Various models were tested, including **Fine Tree**, **Weighted KNN**, and **Efficient Logistic Regression**. 
* **Training Performance**: The **Fine Tree (Model 2.1)** achieved a validation accuracy of **99.9%** using 6 features.
* **Data Visualization**: Includes scatter plots of raw acceleration and absolute acceleration to show class separation.

## 🧮 Calculations
### Calories Burned Formula
Calories are estimated using the following MET-based (Metabolic Equivalent of Task) equation:

$$Calories\ Burned = Time \times (MET \times 3.5) \times \frac{Weight\ [kg]}{200}$$

**MET Values Used:**
* **Sitting**: 1.0
* **Walking**: 3.5
* **Running**: 10.0

### Distance & Steps
* **Total Distance**: Calculated in meters based on GPS coordinates. 
* **Estimated Steps**: Derived from sensor input (e.g., 354 steps for a 265m run).

## 🚀 Future Developments
* Familiarize the system with the specific activity habits of an individual user.
* Implement idle or inactivity alerts.
* Incorporate a wider variety of supported workouts. 

---
*Generated for the FitLife Project - © 2025 BESTME*
