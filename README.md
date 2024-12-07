# Network Slicing in Weather Forcasting System
## Team Members

- **Nishant Dev**  
  - Branch: Computer Science Engineering  
  - ID: 202151100@iiitvadodara.ac.in

- **Sankalp Sagar**  
  - Branch: Information Technology   
  - ID: 202152337@iiitvadodara.ac.in

- **Siddhant Kumar Chaudhary**  
  - Branch: Computer Science Engineering  
  - ID: 202151155@iiitvadodara.ac.in

- **Sourabh Totod**  
  - Branch: Computer Science Engineering  
  - ID: 202151173@iiitvadodara.ac.in

- **Tanmay Meshram**  
  - Branch: Information Technology  
  - ID: 202152341@iiitvadodara.ac.in
 
## Continuation of Edge Computing Project

This repository continues the work from the [Weather Forecasting AI Project](https://github.com/sid142003/weather-foreasting-AI).

## Overview

This README provides information on how to use the single-prediction script designed to load a pre-trained weather and QoS (Quality of Service) model, preprocess input data, make a single prediction, and print the steps involved in the process.

## Video Link

This link contains the video demonstration [Network Slicing in Weather Forcasting System](https://drive.google.com/file/d/11t74k2zX4ug39dKNRJuVb35oT-ysExQR/view?usp=sharing).

## Key Features

1. **Single Model Loading**: Instead of loading all models, this script focuses on loading only one model for a chosen time slice and QoS level or feature.
2. **Preprocessing**: The script preprocesses the last `n_steps` of historical weather data to predict future values.
3. **Single Prediction**: Generates one prediction and prints the intermediate steps, making the process transparent.
4. **Inverse Scaling**: The predicted values are inverse-transformed to the original scale for interpretability.

## File Structure

- `predict_weather.py`: The main script containing all functions and logic to load models, preprocess data, and make a single prediction.
- `README.md`: This file, describing how to use the script.
- `models_path`: Directory containing:
  - Trained `.keras` models (e.g., `morning_high_accuracy_model.keras`)
  - `scaler.pkl`: A fitted scaler for data normalization.
- `data_path`: Path to the CSV file (e.g., `filtered_data.csv`) containing historical weather data.

## Requirements

- Python 3.7+
- TensorFlow (for `tensorflow.keras`)
- Pandas
- NumPy
- scikit-learn

Install any missing dependencies:
```bash
pip install tensorflow pandas numpy scikit-learn
