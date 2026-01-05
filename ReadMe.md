# 🩺 LifeSavior: Vision-Based Fall Detection System  
*“ONE FALL MAKES A CALL.”*  

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-Prototype-blueviolet)
![Python](https://img.shields.io/badge/python-3.10%2B-brightgreen)
![Platform](https://img.shields.io/badge/platform-Computer%20Vision%20%26%20IoT-lightgrey)

---

## 📘 Overview  
The primary intent of **LifeSavior** is to develop a **noninvasive, autonomous device** capable of accurately detecting falls in seniors and immediately calling for help.  

According to the **CDC**, in the United States:  
- About **1 in 4 adults (28%) aged 65 and older** report falling each year.  
- That equates to roughly **36 million falls annually**.  
- By **2050**, projections indicate **52 million elderly falls** per year in the U.S.  

These alarming statistics highlight an urgent need for proactive fall detection systems. LifeSavior addresses this issue through **computer vision, object tracking, and pose detection** to recognize and respond to falls in real-time.

---

## 🎯 Project Goal  
Develop an **autonomous, vision-based fall detection system** that can identify falls, trigger alarms, and alert emergency contacts **without requiring user interaction**.

---

## 🧩 Core Features  

- **📷 Object & Pose Tracking:**  
  Uses real-time video analysis to monitor body posture and detect sudden changes indicating a fall.  

- **📱 SMS Alert System:**  
  Automatically sends customizable emergency messages via built-in SMS when a fall is detected.  

- **🔊 Dual Alert Mechanism:**  
  Activates an audible alarm and simultaneously notifies caretakers until assistance is confirmed.  

- **🧑‍⚕️ User Identification:**  
  Assigns a **unique ID** to each user, enabling accurate tracking and personalized alerts.  

- **🏥 Hospital Integration:**  
  Can be deployed in healthcare settings to monitor **high-risk patients**, reducing the workload for nurses and caretakers.  

---

## 🧪 Methodology  

### 1. Data Acquisition  
- Utilizes **camera-based tracking** to monitor user movement within a controlled environment.  
- Captures body keypoints using **pose estimation models** such as OpenPose or MediaPipe.  

### 2. Fall Detection Logic  
- Applies **temporal motion analysis** to identify sudden vertical-to-horizontal transitions.  
- Evaluates **pose angle, velocity, and duration** to confirm a fall event and reduce false positives.  

### 3. Alert System  
- Once a fall is detected:  
  - An **alarm** is triggered locally.  
  - An **SMS message** is sent continuously to emergency contacts:  
    ```
    Subject: IMPORTANT — User Has Fallen
    ```
  - Notifications persist until caregiver acknowledgment.  

---

## 💻 Tech Stack  

| Layer | Tools & Frameworks |
|-------|--------------------|
| **Computer Vision** | OpenCV, MediaPipe, TensorFlow |
| **Alert System** | Twilio API (SMS), Arduino Buzzer |
| **Backend** | Python, Flask |
| **Tracking & Detection** | YOLOv8, PoseNet |
| **Data Visualization** | Matplotlib, Seaborn |

---

## 🧰 Installation & Setup  

```bash
# Clone the repository
git clone https://github.com/rgna120/LifeSavior.git
cd LifeSavior

# Create a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Install dependencies
pip install -r requirements.txt

# Run the main program
python lifesavior.py
```

> ⚠️ *Note: Ensure the camera feed and Twilio API keys are configured before running.*

---

## 🚀 Expected Outcomes  

- **Real-time fall detection** with minimal false positives.  
- **Automatic emergency alerts** and immediate response.  
- **Reduced caregiver burden** in both home and hospital settings.  
- **Scalable design** adaptable for smart home or clinical monitoring systems.  

---

## 🌍 Broader Impact  
LifeSavior provides a **noninvasive, affordable, and autonomous** solution to one of the most pressing issues in elderly healthcare — accidental falls.  

By bridging **computer vision and healthcare**, LifeSavior helps:  
- Protect independent seniors living alone.  
- Support hospital staff managing multiple high-risk patients.  
- Enhance overall safety and response efficiency in elder care.  

---

## 📄 License  
This project is licensed under the [MIT License](LICENSE).

---

## 👤 Author  
**Nithilan Rengapragash**  
*Developer & Researcher — AI for Healthcare & Robotics*  
- 🔗 [LinkedIn](https://www.linkedin.com/in/nithilan-rengapragash/)
- ✉️ [Email](mailto:rg.nithilan@gmail.com)

---

> “ONE FALL MAKES A CALL.”  
> — *LifeSavior Vision Statement*
