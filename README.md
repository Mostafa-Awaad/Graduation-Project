<p align="center">
  <img src="https://upload.wikimedia.org/wikipedia/ar/a/a2/Nile_University_logo.png" alt="Nile University" width="200"/>
</p> 

# 🧠 BCI-based Upper Limb Exoskeleton Controlled by EEG Signals

<p align="center">
  <img src="https://www.gtec.at/wp-content/uploads/2023/09/unicorn-hybrid-black-bundle.jpg" alt="headset" width="300"/>
  <img src="https://github.com/user-attachments/assets/dd4721a9-e9e0-48ae-a6dd-ee068359c472" alt="headset" width="270"/>
</p>  


 

**Graduation Project — Nile University**  
📅 *Sep 2022 – Feb 2024*  
🎓 **Grade: A+**

---

## 📖 Introduction
This project presents a **Brain–Computer Interface (BCI) system** for controlling an **upper limb exoskeleton** using real-time **EEG signals**. The system integrates **EEG intent-classification pipelines**, advanced **machine learning models**, and a **robotic exoskeleton** to aid in **neurorehabilitation**.  

By decoding motor imagery tasks from EEG data, the exoskeleton responds to patient intent in near real-time, offering a practical solution for **stroke rehabilitation** and **motor recovery therapies**.

---

## 📑 Table of Contents
- [Introduction](#-introduction)  
- [Features](#-features)  
- [Tech Stack](#-tech-stack)  
- [Installation](#-installation)  
- [Usage](#-usage)  
- [System Architecture](#-system-architecture)  
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

## 🛠️ Tech Stack

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

## ⚙️ Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-repo/bci-exoskeleton.git
   cd bci-exoskeleton
