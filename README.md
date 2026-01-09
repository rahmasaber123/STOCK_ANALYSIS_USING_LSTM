# 📈 LSTM Time Series Prediction Model

## Overview
This project implements a **Long Short-Term Memory (LSTM)** neural network to perform **time-series forecasting** on a univariate dataset. The model learns temporal dependencies from historical data and predicts future values based on sliding time windows.

The pipeline covers data preprocessing, scaling, sequence generation, model training, evaluation, and visualization.

---

## Project Objectives
- Build an end-to-end LSTM-based time-series prediction model  
- Capture temporal patterns and trends in sequential data  
- Evaluate model performance using statistical metrics and visual analysis  

---

## Technologies Used
- Python  
- NumPy  
- Pandas  
- Matplotlib  
- Scikit-learn  
- TensorFlow / Keras  

---

## Data Preprocessing

### Train–Test Split
The dataset is divided into training and testing subsets while preserving temporal order.

### Normalization
Data is scaled to the range **[0, 1]** using `MinMaxScaler` to improve training stability.

### Sliding Window Technique
A fixed window length is used to transform the time series into supervised learning samples:
- **Input:** previous `n` time steps  
- **Output:** next time step  

### Reshaping for LSTM
 - **Data** is reshaped into the format:
   (samples, timesteps, features)

---

## Model Architecture
The model is built using a stacked LSTM architecture:
- 4 LSTM layers (50 units each)  
- Dropout layers (0.2) for regularization  
- Dense output layer for final prediction  

**Architecture Flow:**
```bash
Input → LSTM → Dropout → LSTM → Dropout → LSTM → Dropout → LSTM → Dense
```
## How to Run
1. Clone the repository  
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
## Conclusion

### This project demonstrates a complete and well-structured approach to time-series forecasting using LSTM networks. 
### It provides reliable trend predictions with good generalization and serves as a solid foundation for further experimentation and optimization.
**Author:**
## ENG RAHMA SABER ABBAS
Data is reshaped into the format:

