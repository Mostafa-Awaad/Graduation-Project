<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/ar/a/a2/Nile_University_logo.png" alt="Nile University" width="200"/>
</p> 

# 🧠 BCI-based Upper Limb Exoskeleton Controlled by EEG Signals

<p align="center">
  <img src="https://www.gtec.at/wp-content/uploads/2023/09/unicorn-hybrid-black-bundle.jpg" alt="headset" width="300"/>
  <img src="https://github.com/user-attachments/assets/dd4721a9-e9e0-48ae-a6dd-ee068359c472" alt="headset" width="270"/>
</p>  


 

**Graduation Project — Nile University**  
🎓 **Grade: A+**

---

## 📖 Introduction
This project presents a **Brain–Computer Interface (BCI) system** for controlling an **upper limb exoskeleton** using real-time **EEG signals**. The system integrates **EEG intent-classification pipelines**, advanced **machine learning models**, and a **robotic exoskeleton** to aid in **neurorehabilitation**.  

By decoding motor imagery tasks from EEG data, the exoskeleton responds to patient intent in near real-time, offering a practical solution for **stroke rehabilitation** and **motor recovery therapies**.

---

## 🎯 Aim & Motivation <a name="aim-&-motivation"></a>
- Our rehabilitation system comprises two subsystems – the mechanical and BCI systems – working in harmony to optimize the rehabilitation process.
- The mechanical and BCI systems operate together, fostering a cooperative approach that enhances targeted and adaptive rehabilitation for improved patient outcomes.
- Through progressive training, our system empowers patients to regain independence, leading a normal life and reducing reliance on external assistance.

---

## 📑 Table of Contents
- [Introduction](#-introduction)
- [Aim & Motivation](#aim-&-motivation) 
- [Features](#-features)  
- [Tech Stack](#tech-stack)   
- [Exoskeleton Arm Requirements](#exoskeleton-skeleton-requirements)
- [Hardware Components](#hardware-components)
- [Mechanical Design](#mechanical-design)
- [System Architecture](#system-architecture)  
- [Examples](#-examples)  
- [Troubleshooting](#-troubleshooting)  
- [Contributors](#-contributors)  
- [License](#-license)  

---

## 🚀 Features
- ⚡ **Real-time EEG intent-classification** for exoskeleton arm control.  
- 🤖 **Integration with UNICORN Hybrid Black EEG headset** via Lab Streaming Layer (LSL).  
- 🧩 **Multi-class EEG motor imagery detection** (feet, left hand, right hand, tongue).  
- 📊 Achieved **78% classification accuracy** *(Cohen’s κ = 0.71)*.  
- 🔬 **Signal preprocessing pipeline** with filtering, artifact removal, and feature extraction.  
- 🔗 **MATLAB Engine API integration** for enhanced computation and visualization.  
- 🏥 Application in **neurorehabilitation and assistive robotics**.  

---

## 🛠️ Tech Stack <a name="tech-stack"></a>

- **Programming & ML Frameworks** 

     ![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?logo=tensorflow&logoColor=white) ![Keras](https://img.shields.io/badge/Keras-D00000?logo=keras&logoColor=white)  

- **Data Visualization & Processing**

     ![Matplotlib](https://img.shields.io/badge/Matplotlib-005571?logo=plotly&logoColor=white) ![MNE](https://img.shields.io/badge/MNE-Purple?logo=brain&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-150458?logo=pandas&logoColor=white)  

- **Machine Learning & Statistics** 

     ![Scikit-learn](https://img.shields.io/badge/Scikit--learn-F7931E?logo=scikit-learn&logoColor=white) ![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?logo=scipy&logoColor=white)  

- **MATLAB Integration**  
![MATLAB](https://img.shields.io/badge/MATLAB-FF7400?logo=mathworks&logoColor=white)  

- **Real-time Streaming & Hardware**  
  - Lab Streaming Layer (LSL)  
  - UNICORN Hybrid Black EEG headset  
  - Exoskeleton Arm  

---

## 🤖 Exoskeleton Arm Requirements <a name ="exoskeleton-arm-requirements"></a>
| Requirement               | Features                                                                                                                                                                             |
|--------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| **Safety**               | - Aligning with natural arm movements <br> - Setting force limits <br> - Ensuring precise control for accurate and controlled movements                                               |
| **Comfort**              | - Prevent arm fatigue <br> - Focusing on well-transmitted forces <br> - Balanced torques around joints <br> - Secure attachment to avoid slipping                                     |
| **Easy Wearability**     | - Comfort and freedom of movement <br> - Avoiding need for specific starting poses <br> Minimizing bulkiness and be lightweight <br> - Providing Adjustment for different arm sizes   |

---

## 💻 Hardware Components <a name="hardware-components"></a>
| Component               | Features                                                                 |
|--------------------------|---------------------------------------------------------------------------|
| **Raspberry Pi**         | - Signal processing <br> - Machine Learning Integration                  |
| **Servo Motor (35.5 KG)**| - Relatively High Torque Capacity <br> - Movement of the Elbow            |
| **Servo Motor (MG995)**  | - Relatively Medium Torque Capacity <br> - Movement of the Wrist          |
| **Force Sensor**         | - Arm Weight Measuring                                                   |
| **MPU6050 Accelerometer**| - Motion Measurements <br> - Feedback for Control Algorithm               |

---

## ⚙ Mechanical Design <a name="mechanical-design"></a>
<table align="center">
  <tr>
    <td align="center">
      <img height="200" src="https://github.com/user-attachments/assets/59a827bf-1e15-4a04-b752-fbc573271f66" alt="Image 1"/><br>
      <b>Top View</b>
    </td>
    <td align="center">
      <img height="200" src="https://github.com/user-attachments/assets/0803555a-e1ab-408b-b6ce-f10fe8a0a174" alt="Image 2"/><br>
      <b>Isometric View</b>
    </td>
  </tr>
  <tr>
    <td align="center">
      <img height="200" src="https://github.com/user-attachments/assets/fb52e1ac-53a8-4acd-b019-fb2917d9202c" alt="Image 3"/><br>
      <b>Front View</b>
    </td>
    <td align="center">
      <img height="200" src="https://github.com/user-attachments/assets/7dc56933-64aa-49bb-86b4-bbc36ce006f2" alt="Image 4"/><br>
      <b>Side View</b>
    </td>
  </tr>
</table>







## 🛠️ System Architecture <a name="system-architecture"></a>

```mermaid
flowchart LR
    A["EEG Acquisition - UNICORN Headset"] --> B["Lab Streaming Layer - LSL"]
    B --> C["Signal Preprocessing - MNE, SciPy, Pandas"]
    C --> D["Feature Extraction & Classification - TensorFlow/Keras, Scikit-learn"]
    D --> E["Real-time Intent Detection"]
    E --> F["Exoskeleton Arm Control"]

    %% 🎨 Colors
    style A fill:#1E90FF,stroke:#000,stroke-width:2px,color:#fff
    style B fill:#00BFFF,stroke:#000,stroke-width:2px,color:#fff
    style C fill:#FFD700,stroke:#000,stroke-width:2px,color:#000
    style D fill:#FF7F50,stroke:#000,stroke-width:2px,color:#fff
    style E fill:#32CD32,stroke:#000,stroke-width:2px,color:#fff
    style F fill:#228B22,stroke:#000,stroke-width:2px,color:#fff


```

