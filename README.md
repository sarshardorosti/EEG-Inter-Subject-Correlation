# Neural Synchronization Response to Fractal Animations: An ISC Study

## Overview

This project investigates neural responses to fractal animations using Inter-Subject Correlation (ISC) within the curriculum of Bournemouth University's "Artificial Intelligence for Media" course. We analyze EEG data from fifteen healthy postgraduate male students to study how their brains react consistently to identical visual stimuli. The results offer insights into neural mechanisms and contribute to the design of neuropsychological tests and therapeutic interventions.

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

## Data Collection

Data collection involved recording EEG from subjects viewing fractal animations on a 42" monitor. EEG data were captured using a 32-electrode setup, synchronized with the presentation of the visual stimuli to ensure accuracy in temporal alignment.

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

## Evaluation Techniques

Robustness tests are conducted using:
- `shuffle_in_time`: Tests the dependency of EEG data analyses on temporal sequence.
- `phase_randomized`: Confirms genuine neural synchronizations and not artifacts.

## Conclusions

The study validates ISC as a robust method for examining neural responses, highlighting the critical roles of precise temporal and phase alignments in understanding collective neural dynamics.

## References and Appendices

The project includes extensive references and appendices that support the methodologies and results discussed.

## Project Resources

- **[Project Repository](https://github.com/sarshardorosti/EEG-Inter-Subject-Correlation.git)**
- **[EEG Dataset](https://drive.google.com/file/d/13C3jGhStqXbUsBjb5my_txzhr28zm5Cr/view?usp=sharing)**
- **[Video Visualization of Test Results](https://drive.google.com/file/d/1LDGlXA033PbD07uUoQRVTUeFBKS5L9n/view?usp=sharing)**

This README provides a professional overview of the project, facilitating understanding and exploration of the study, ensuring all necessary resources and references are accessible for users and researchers.
