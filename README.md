# 🚀 Elevator Fault Detection and Prediction System

This project simulates a smart elevator fault detection system inspired by **KONE's intelligent urban mobility solutions**. It uses real-time sensor-like inputs and a trained machine learning model to predict possible faults in elevators.

## 🎯 Objective

Predict elevator faults based on features such as:
- Motor Temperature
- Door Status
- Floor Requests
- Time-based data (Hour, Minute, Day of Week)
- Rolling average and historical inputs

## 🔍 Key Features

✅ **Simulated sensor data**  
⚙️ **Feature engineering**: Time, moving averages, lag variables  
🧠 **ML Model**: Random Forest Classifier with GridSearchCV  
💻 **Gradio App**: Clean UI for live predictions  
📈 **High Accuracy**: ~95% with perfect recall on fault cases  

## ⚙️ Technologies Used

- Python
- Pandas, NumPy
- Scikit-learn (Random Forest, LabelEncoder, GridSearchCV)
- Gradio (Interactive UI)

## 🧪 Sample Inputs

| Motor Temp (°C) | Door Status | Floor Req | Hour | Minute | Day | MA Temp | Prev Temp | Prev Req |
|------------------|-------------|------------|------|--------|-----|----------|------------|-----------|
| 105              | Closed      | 6          | 14   | 30     | 1   | 101      | 100        | 5         |

→ **Output**: ⚠️ Fault Detected in Elevator!

## 🔗 Live Demo

👉 **Try it here**: [Gradio App Live Link](https://huggingface.co/spaces/THARUNIKA28/elevator-fault-detector)  


## 📁 Dataset

- Generated using Python to simulate realistic elevator logs and sensor readings.
- Can be replaced with real IoT-based datasets in production.

## 📊 Model Metrics

- ✅ **Accuracy**: ~95%
- 🎯 **Precision**: ~91%
- 🔄 **Recall**: 100% (no missed faults)

---

## 📦 To Run Locally

```bash
git clone https://github.com/THARUNIKA28/elevator-fault-detection-system.git
cd elevator-fault-detection
pip install -r requirements.txt
python app.py
