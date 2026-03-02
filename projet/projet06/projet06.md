# EMG-Driven Musculoskeletal Modeling using OpenSim
**Institution:** École Supérieure Privée d’Ingénierie et de Technologie Appliquée (ESPITA)  
**Category:** Biomechanics / Biomedical Engineering / EMG Signal Processing  
**Status:** Research & Simulation Study  

## Project Overview
This project focuses on the development of a musculoskeletal model integrating EMG signals to estimate muscle forces and activations using OpenSim.

The objective was to investigate muscle force control through EMG-informed simulations and compare computational estimations with experimental data.

The study explores how electromyographic (EMG) signals can enhance the personalization and accuracy of musculoskeletal simulations.

---

## Images / captures
![Image du projet](../assets/images/projet1.png)

## Lien / Vidéo
[Voir le projet](https://lien-vers-le-projet-ou-video)

---

## Scientific Background

Musculoskeletal modeling aims to estimate:
- Muscle forces
- Joint moments
- Internal biomechanical loads

Integrating EMG signals allows:
- Subject-specific personalization
- More realistic neuromuscular simulation
- Improved validation of computational models

---

## Dataset

The project used the **Ninapro DB5 dataset (Subject 4)** for upper-limb EMG signals.

Dataset characteristics:
- Sampling frequency: 2000 Hz
- 16 EMG channels (8 per Myo armband)
- Segmented and labeled repetitions
- Synchronized glove data (22 sensors)
- Integrated accelerometer data

---

## Methodology

### 1. EMG Signal Processing
- Signal filtering and normalization
- Data segmentation
- Conversion into `.mot` file format compatible with OpenSim

### 2. OpenSim Workflow
- Loading `.osim` musculoskeletal model
- Importing `.mot` motion file
- Performing static optimization

### 3. Simulation Outputs
OpenSim generated:

- `.xml` file → control configuration  
- `.sto` file (activation) → estimated muscle activation levels (0–1 range)  
- `.sto` file (force) → estimated muscle forces (in Newtons)  

These outputs allow:
- Comparison between estimated activation and real EMG
- Muscle-by-muscle force analysis
- Peak force identification
- Movement-induced muscle demand estimation

---

## Theoretical Framework

The model assumes equilibrium between:
- Muscle force (Fm)
- Tendon force (Ft)

The dynamic equations incorporate:
- Force-length relationship
- Force-velocity relationship
- Passive elastic components
- Tendon stiffness properties

The computational approach follows methodologies described in:

OpenSim: A musculoskeletal modeling and simulation framework for in silico investigation  
PMID: 25893160  

---

## Tools & Technologies
- OpenSim
- EMG Signal Processing
- Ninapro DB5 Dataset
- Musculoskeletal Modeling
- Biomechanical Simulation

---

## Challenges

Due to muscle naming inconsistencies between the Ninapro dataset and OpenSim models, full subject-specific simulation alignment was not completed.

However, simulations using open-source OpenSim models were conducted to understand workflow mechanics and force estimation behavior.

---

## Outcomes

The project demonstrated:
- The feasibility of EMG-informed modeling
- The ability to estimate muscle activation and force
- The importance of model calibration and anatomical consistency

---

## Conclusion

EMG integration into musculoskeletal modeling represents a powerful tool for improving biomechanical simulations and understanding neuromuscular dynamics.

This approach has strong potential applications in:
- Rehabilitation engineering
- Prosthetics design
- Movement analysis
- Personalized medicine
