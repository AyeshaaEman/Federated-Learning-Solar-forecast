**Federated Deep Learning Techniques for Solar Power Forecasting**

This repository contains an implementation of federated learning for solar power forecasting using time-series data. Three clients train local LSTM models, and the models are aggregated using Federated Averaging (FedAvg). RandomForest, SVM, and XGBoost are included as baseline models.

**Project Overview**

This project implements federated deep learning for solar power forecasting with client-specific training and global model aggregation.

**Features**

Three client datasets with aligned timestamps.

Time-series preprocessing and feature scaling.

LSTM models for local forecasting.

Federated Averaging for global aggregation.

RandomForest, SVM, and XGBoost as baselines.

Evaluation with MAE, RMSE, MSE, and R².

**Workflow**

Load and align datasets

Synchronize and select numeric features

Split datasets into Train, Validation, and Test sets

Normalize features

Create time-series sequences

Train local LSTM models

Evaluate models

Aggregate with FedAvg

Train and compare baseline ML models
**Repository Structure**
fed-solar-forecast/
│── data/               # Datasets (not included)  
│── notebooks/          # Jupyter notebooks  
│── src/                # Scripts for preprocessing, training, and evaluation  
│── results/            # Plots and metrics  
│── requirements.txt    # Dependencies  
│── README.md           # Documentation  

**Installation**
git clone https://github.com/<your-username>/fed-solar-forecast.git
cd fed-solar-forecast
pip install -r requirements.txt

**Usage**
python src/train_local.py       # Train local LSTM models
python src/federated_avg.py     # Run FedAvg aggregation
python src/evaluate.py          # Evaluate models

**Results**

Local LSTM models trained per client.

FedAvg produced a global model.

RandomForest, SVM, and XGBoost used as baselines.

Results stored in the results/ folder.
