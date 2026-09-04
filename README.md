# Disaster Risk Monitoring Using Satellite Imagery

**Author:** Shubham Sharma[cite: 1]

## Project Overview
This repository contains the independent research and technical thesis detailing an automated flood detection system[cite: 1]. It utilizes advanced Computer Vision techniques and Sentinel-1 Synthetic Aperture Radar (SAR) satellite imagery to rapidly assess infrastructure damage due to flood events[cite: 1]. The primary objective is to generate high-fidelity flood maps to provide immediate, actionable intelligence for response teams in environments where human access is impossible or unsafe[cite: 1].

## Technical Pipeline
This solution follows an industry-standard, GPU-accelerated Deep Learning workflow[cite: 1]:

* **Data Ingestion & Preprocessing:** Utilizes the NVIDIA Data Loading Library (DALI) to create GPU-accelerated data pipelines for high-throughput data loading and on-the-fly augmentations[cite: 1].
* **Model Training:** Employs the NVIDIA TAO Toolkit to fine-tune a pre-trained ResNet-18 model adapted for a U-Net Semantic Segmentation architecture[cite: 1].
* **Deployment & Inference:** The trained model is compiled into an optimized TensorRT engine and deployed via the NVIDIA Triton Inference Server to balance low latency with high throughput for real-time inference[cite: 1].

## Dataset & Case Study
* The model was developed using Sentinel-1 SAR data (GeoTIFF format)[cite: 1].
* Practical utility was validated against the Nepal June 2021 Flood Event, monitored by UNOSAT[cite: 1].
* The AI-generated flood extent was cross-referenced with baseline demographic data (like WorldPop) to estimate the exposed population and support disaster risk management[cite: 1].

## Acknowledgements
This project acts as a permanent portfolio record of the skills gained from specialized training provided by the NVIDIA Deep Learning Institute (DLI) in partnership with UNITAR and UNOSAT[cite: 1].
