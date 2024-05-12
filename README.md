# Neural Synchronization Response to Fractal Animations: An ISC Study

## Overview

This project investigates neural responses to fractal animations using Inter-Subject Correlation (ISC) within the curriculum of Bournemouth University's "Artificial Intelligence for Media" course. We analyze EEG data from fifteen healthy postgraduate male students to study how their brains react consistently to identical visual stimuli. The results offer insights into neural mechanisms and contribute to the design of neuropsychological tests and therapeutic interventions.


![Experiment paradigm](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/db5494dd-88ae-4514-a995-31650092fd98)


https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/9fa84d7e-2fbc-44db-8e8d-8a5cb2c3c383



## Table of Contents

- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Preprocessing](#preprocessing)
- [Analytical Techniques](#analytical-techniques)
- [Implementation](#implementation)
- [Visualization and Results Management](#visualization-and-results-management)
- [Evaluation Techniques](#evaluation-techniques)
- [Conclusions](#conclusions)
- [References and Appendices](#references-and-appendices)
- [Project Resources](#project-resources)

## Introduction

This study utilizes Inter-Subject Correlation (ISC) to examine the brain states triggered by fractal animations, assessing the reliability and consistency of neural responses to structured visual challenges across different subjects.
![Screenshot 2024-05-12 110134](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/7eec388f-9ac1-4a7a-9ec0-9d980f96413a)

## Data Collection

EEG data were collected using a 32-electrode setup from subjects as they viewed fractal animations on a 42" monitor. The data capture was synchronized with the visual stimuli presentation to ensure precise temporal alignment. Data collection involved 15 male postgraduate students, non-smokers with no history of mental disorders. Detailed preparation ensured accurate data by recording sessions between 9 to 11 AM in a controlled environment.

![Screenshot 2024-05-12 110005](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/fdf97f21-887d-4a0c-9f9c-1a6a7ceb0254)
![Screenshot 2024-05-12 110856](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/5b51c74d-f4fc-46fd-b87a-dfddfb7a985b)


To import data, the address of the first data must be given to raw2 to use the data structure for processing.
The extension of the data must be .set and also the entire data set must be located at the address data_dir = './data/'.


## Preprocessing

Raw EEG data were processed through several stages:
- Downsampling to 256 Hz and band-pass filtering between 1 and 40 Hz.
- Independent Component Analysis (ICA) for artifact removal, focusing on removing components associated with eye blinks and other common sources of noise.
- Meticulous inspection and removal of bad channels and noisy data, using techniques like Kurtosis to identify outliers.


## Analytical Techniques

Utilizing Correlated Component Analysis (CCA) for:
- Identifying spatial filters to enhance the correlation between brain signals across subjects under various experimental conditions.
- Calculating and adjusting covariance matrices, and extracting significant eigenvectors and eigenvalues.


## Implementation

Key functions in the project include:
- `train_cca`: Prepares and processes data using CCA for analysis.
- `apply_cca`: Applies CCA to examine relationships between multivariate datasets.
- `plot_isc`: Generates visualizations like bar charts and topographic maps to depict ISC values and their distributions.

## Visualization and Management

The project involves generating ISC values and distributions through visualizations like bar charts and topographic maps. Results are meticulously documented and managed in Excel for thorough analysis and accessibility.

![Screenshot 2024-05-12 113537](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/085bca9b-c49b-4c22-a0d4-61e555d5c2d2)


## Evaluation Techniques

Robustness tests are conducted using:
- **`shuffle_in_time`**: Confirms the dependency of EEG data analyses on the temporal sequence.
- **`phase_randomized`**: Validates genuine neural synchronizations, distinguishing them from artifacts.
- Detailed evaluations reveal the importance of precise temporal and phase alignments in interpreting neural synchronizations.

![Screenshot 2024-05-12 113638](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/22fc3de3-a322-4ac7-a1a7-e72933d84e24)
![Screenshot 2024-05-12 113601](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/b5ac3a4d-a8f0-4079-9cb3-3283817daa68)




## Conclusions

The study validates ISC as a robust method for examining neural responses, highlighting the critical roles of precise temporal and phase alignments in understanding collective neural dynamics.

![Screenshot 2024-05-12 110540](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/dc8713df-41de-4094-bd70-e43b8fe2821b)



## Project Resources
Only EEG data related to animation 4 is placed here. More data will be updated soon.

- **[Project Repository](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation.git)**
- **[EEG Dataset](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/tree/main/Data)**
- **[Video Visualization of Test Results](https://drive.google.com/file/d/1LDGlXA033PbD07u7UoQRVTUeFBKS5L9n/view?usp=sharing)**



## Reference list
- Dmochowski, J. P., et al. (2012). Correlated Components of Ongoing EEG Point to Emotionally Laden Attention – A Possible Marker of Engagement? *Frontiers in Human Neuroscience*, 6.
- DOROSTI, S., et al. (2022). ANALYSIS OF THE COMPLEXITY OF EEG SIGNALS IN RELATION TO THE COMPLEXITY OF FRACTAL ANIMATIONS. *Fractals*.
- Moreno Escobar, J. J., et al. (2020). Brain-Inspired Healthcare Smart System Based on Perception-Action Cycle. *Applied Sciences*, 10(10), 3532.
- Najafi, M., et al. (2017). Dynamics of Intersubject Brain Networks during Anxious Anticipation. *Frontiers in Human Neuroscience*, 11.


