# Acoustic PUF for Aerospace SHM - Team Skyrim (Airbus Competition 2026) ✈️

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Ubuntu](https://img.shields.io/badge/OS-Ubuntu-E95420?logo=ubuntu&logoColor=white)]()
[![Python](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=white)]()
[![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?logo=pytorch&logoColor=white)]()
[![C++](https://img.shields.io/badge/C++-00599C?logo=c%2B%2B&logoColor=white)]()

> Team Skyrim’s edge-native Structural Health Monitoring (SHM) system extracts an Acoustic Physically Unclonable Function (PUF) from critical mechanical assemblies to detect physical tampering and degradation in real-time. By bridging the aerospace cyber-physical gap, this framework acts as a localized, Zero-Trust hardware authenticator for aircraft fleets without relying on heavy cloud bandwidth.

## ⚙️ Core Features
* **Multi-Class Fault Diagnosis AI:** A Grouped Convolutional Denoising Autoencoder (GCDAE) paired with a Support Vector Machine (SVM) locally classifies mechanical states (e.g., nominal vs. loosened structural fasteners) based on deep latent space feature extraction.
* **High-Frequency Edge DAQ:** Custom embedded architecture utilizes Direct Memory Access (DMA) on a heterogeneous edge node to capture 250kHz+ piezoelectric micro-vibration data synchronously with ambient MEMS microphones.
* **Cyber-Physical Security Layer:** Converts raw acoustic signatures into immutable "structural state tokens." This mitigates eavesdropping risks, isolates the IT network from remote spoofing, and seamlessly integrates with predictive maintenance ecosystems like Airbus Skywise.
* **Dynamic Thresholding:** Automatically recalibrates security baselines to account for natural operational signal drift and high-tempo environmental variations, virtually eliminating false positives.

## 🛠️ Tech Stack
* **Languages:** Python 3.10+, C/C++
* **Machine Learning:** PyTorch, Scikit-learn, SciPy, NumPy, Pandas
* **Embedded/Hardware:** STM32 HAL / ESP-IDF (Analog front-end data acquisition)
* **Modeling & Simulation:** ANSYS Workbench (Modal, Harmonic, Transient Analysis), Autodesk Fusion 360
* **Environment:** Ubuntu Linux

## 🚀 Quick Start

### Prerequisites
To run the AI anomaly detection pipeline and generate the diagnostic spectrograms locally, ensure you have the following installed on your Ubuntu environment:
* Python 3.10+
* `pip` package manager
* CUDA Toolkit (Optional, but highly recommended for hardware-accelerated PyTorch tensor operations)

## 👥 The Team (Skyrim)
* **Asraful Islam Hemel** -Team Lead & Systems Architect (Hardware, Embedded DAQ & AI Architecture)
* **Marufa Akter** - Mechanical Designer & ANSYS Simulation Specialist
* **Sayma Islam** - Structural Dynamics & ANSYS Simulation Specialist
* **Aresha Basir Spriha** - Machine Learning & AI Development 
* **Mubtasim Morshed Mugdha** - Hardware Integration & Experimental Testing
