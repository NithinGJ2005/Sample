# PrognosAI: AI-Driven Predictive Maintenance System

## 📌 Project Objective
To design and develop an **AI-based predictive maintenance system** capable of estimating the **Remaining Useful Life (RUL)** of industrial machinery using **multivariate time-series sensor data**.  
The system uses the **NASA CMAPSS dataset** and is designed to generalize across domains like turbines, pumps, and motors.  
This will help in:
- Enabling **timely maintenance decisions**  
- Minimizing **unplanned downtime**  
- Optimizing **asset utilization**  

---

## ⚙️ Project Workflow
1. **Data Ingestion**  
   - Load and preprocess the CMAPSS dataset (cycle-wise engine data).  

2. **Feature Engineering**  
   - Create rolling window sequences  
   - Compute Remaining Useful Life (RUL) targets  

3. **Model Training**  
   - Train time-series models (LSTM/GRU) to predict RUL  

4. **Model Evaluation**  
   - Evaluate using RMSE and compare predicted vs actual RUL  

5. **Risk Thresholding**  
   - Define thresholds to trigger maintenance alerts  

6. **Visualization & Output**  
   - Dashboards showing RUL trends and alert zones  

---

## 🏗️ Architecture
- **Data Processing** → `pandas`, `numpy`  
- **Visualization** → `matplotlib`, `seaborn`  
- **Model Training** → `TensorFlow/Keras` (LSTM, GRU)  
- **Evaluation** → `scikit-learn` metrics  
- **Deployment (optional)** → `Flask/Streamlit`, Docker  

---

## 📊 Dataset
- **Source**: [NASA CMAPSS dataset](https://data.nasa.gov/dataset/C-MAPSS-Aircraft-Engine-Simulator-Data/xaut-bemq)  
- **Files**: `train_FD001.txt`, `train_FD002.txt`, `train_FD003.txt`, `train_FD004.txt`  
- Each row contains:
  - Engine ID  
  - Cycle number  
  - 21 sensor measurements  

---

## 🚀 Installation & Usage
### 1. Clone the repo
```bash
git clone https://github.com/yourusername/RUL-PREDICTIVE-MAINTENANCE.git
cd RUL-PREDICTIVE-MAINTENANCE
```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate      # Linux/Mac
venv\Scripts\activate         # Windows
```

### 3. Install dependencies
```bash
pip install -r requirements.txt
```

### 4. Run data preprocessing
```bash
python src/data_preprocessing.py
```

### 5. Train the model
```bash
python src/train_model.py
```

---

## 📈 Future Improvements
- Experiment with **Transformers for time-series**  
- Hyperparameter tuning (learning rate, sequence length)  
- Deploy via **Streamlit dashboard**  
- Integrate **real-time streaming data**  

---

## 🧑‍💻 Contributors
- **Nithin G J** – Project Developer  
