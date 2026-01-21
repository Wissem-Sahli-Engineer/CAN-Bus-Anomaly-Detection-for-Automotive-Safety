# 🚗 CAN-Bus-Anomaly-Detection-for-Automotive-Safety
Real-time vehicle safety monitoring using CAN bus data with privacy-preserving federated learning

## 🎯 Project Overview
CANBusGuard is a federated learning system for detecting anomalous driving patterns using CAN bus data. Developed for Renault with partner Zouhour, this system enables privacy-preserving collaborative training across multiple vehicles.

- **Real-time anomaly detection** from CAN bus data  
- **Privacy-preserving federated learning** across multiple devices  
- **Multiple autoencoder architectures** (LSTM, GRU, Conv1D, Hybrid, Attention)  
- **TensorFlow Lite optimization** for edge deployment  
- **Comprehensive safety scoring system**  


## 📁 Project Structure
```
│
├──Copie de  pipeline.ipynb
├──Copie de device1_final_production.ipyn 
├──Copie de server_FL.ipynb
├── README.md
````
## 🚀 Workflow


- **Client Training**
Individual vehicles train LSTM autoencoders on local CAN bus data


- **Weight Extraction**
Trained models extract and compress weights to shared storage


- **Server Aggregation**
Central server performs federated averaging of all client weights


- **Global Model**
Aggregated global model generates safety scores for driving patterns


- **Edge Deployment**
Optimized TensorFlow Lite (TFLite) models are deployed back to vehicles


## 🛠️ Technical Implementation


- **Data**: Private Renault CAN bus database *(confidential)*
- **Models**: 3-layer LSTM autoencoder with federated averaging
- **Training**: 50 epochs per client, 20-timestep input sequences
- **Output**: Safety scores (0–1 scale) and anomaly detection reports

## Requiremetns 

```bash
pip install tensorflow numpy pandas matplotlib seaborn scikit-learn keras-tuner paho-mqtt
```
## 👥 Team 
### Zouhour - Wissem : Renault
