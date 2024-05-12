# Neural Synchronization Response to Fractal Animations: An ISC Study

## Overview

This project investigates neural responses to fractal animations using Inter-Subject Correlation (ISC) within the curriculum of Bournemouth University's "Artificial Intelligence for Media" course. We analyze EEG data from fifteen healthy postgraduate male students to study how their brains react consistently to identical visual stimuli. The results offer insights into neural mechanisms and contribute to the design of neuropsychological tests and therapeutic interventions.
![Experiment paradigm](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/db5494dd-88ae-4514-a995-31650092fd98)

## Table of Contents

- [Introduction](#introduction)
- [Data Collection](#data-collection)
- [Preprocessing](#preprocessing)
- [Analytical Techniques](#analytical-techniques)
- [Implementation](#implementation)
- [Visualization and Management](#visualization-and-management)
- [Evaluation Techniques](#evaluation-techniques)
- [Conclusions](#conclusions)
- [References and Appendices](#references-and-appendices)

## Introduction

This study utilizes Inter-Subject Correlation (ISC) to examine the brain states triggered by fractal animations, assessing the reliability and consistency of neural responses to structured visual challenges across different subjects.
![Screenshot 2024-05-12 110134](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/7eec388f-9ac1-4a7a-9ec0-9d980f96413a)

## Data Collection

Data collection involved recording EEG from subjects viewing fractal animations on a 42" monitor. EEG data were captured using a 32-electrode setup, synchronized with the presentation of the visual stimuli to ensure accuracy in temporal alignment.

![Screenshot 2024-05-12 110005](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/fdf97f21-887d-4a0c-9f9c-1a6a7ceb0254)
![Screenshot 2024-05-12 110856](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/5b51c74d-f4fc-46fd-b87a-dfddfb7a985b)


## Preprocessing

Raw EEG data were processed through several stages:
- Downsampling and band-pass filtering
- Artifact removal using Independent Component Analysis (ICA)
- Preparation of data for further analysis through meticulous preprocessing protocols

## Analytical Techniques

Correlated Component Analysis (CCA) was the primary technique used, focusing on:
- Identifying spatial filters that enhance correlations between brain signals
- Computing covariance matrices and extracting informative eigenvectors and eigenvalues

## Implementation

Key functions in the project include:
- `train_cca`: Prepares and processes data using CCA for analysis.
- `apply_cca`: Applies CCA to examine relationships between multivariate datasets.
- `plot_isc`: Generates visualizations like bar charts and topographic maps to depict ISC values and their distributions.

## Visualization and Management

The project involves creating visualizations to display ISC results comprehensively. Functions manage the creation of bar charts, topographic maps, and the documentation of results in Excel for accessibility and further analysis.

![Untitled-1](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/3991da54-5f06-4896-9e0c-9f1272bd5746)

## Evaluation Techniques

Robustness tests are conducted using:
- `shuffle_in_time`: Tests the dependency of EEG data analyses on temporal sequence.
- `phase_randomized`: Confirms genuine neural synchronizations and not artifacts.
![ISC_Bar_Chart_shuffled copy](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/189c2b82-889a-46d3-831f-4c611d124b35)
![Screenshot 2024-05-12 110221](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/61a9b240-7289-48db-9974-9193f7e822c9)

## Conclusions

The study validates ISC as a robust method for examining neural responses, highlighting the critical roles of precise temporal and phase alignments in understanding collective neural dynamics.

![Screenshot 2024-05-12 110540](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation/assets/50841748/dc8713df-41de-4094-bd70-e43b8fe2821b)

## References and Appendices

The project includes extensive references and appendices that support the methodologies and results discussed.

## Project Resources

- **[Project Repository](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation.git)**
- **[EEG Dataset](https://drive.google.com/file/d)**
- **[Video Visualization of Test Results](https://drive.google.com/file/d/1LDGlXA033PbD07uUoQRVTUeFBKS5L9n/view?usp=sharing)**



## Reference list
Dmochowski, J. P., Sajda, P., Dias, J. and Parra, L. C., 2012. Correlated Components of Ongoing EEG Point to Emotionally Laden Attention – A Possible Marker of Engagement? Frontiers in Human Neuroscience, 6.
DOROSTI, S., NAMAZI, H. and KHOSROWABADI, R., 2022. ANALYSIS OF THE COMPLEXITY OF EEG SIGNALS IN RELATION TO THE COMPLEXITY OF FRACTAL ANIMATIONS. Fractals.
Moreno Escobar, J. J., Morales Matamoros, O., Tejeida Padilla, R., Lina Reyes, I., Chanona Hernández, L. and Ramírez Gutiérrez, A. G., 2020. Brain-Inspired Healthcare Smart System Based on Perception-Action Cycle. Applied Sciences, 10 (10), 3532.
Najafi, M., Kinnison, J. and Pessoa, L., 2017. Dynamics of Intersubject Brain Networks during Anxious Anticipation. Frontiers in Human Neuroscience, 11.


