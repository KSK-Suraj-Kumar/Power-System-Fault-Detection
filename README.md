# 🔌 Power Distribution Fault Classification using Machine Learning

## 📌 Project Overview
This project aims to automatically **detect and classify fault types** in a power distribution system using **machine learning techniques**. The solution leverages the **Random Forest Classifier** within the **IBM Watsonx.AI** platform, using historical and simulated electrical, environmental, and operational data to improve fault diagnosis and response times.

---

## 🧠 Objective
To build a machine learning model that can predict and classify various types of power system faults—such as **Line-to-Ground (LG)**, **Line-to-Line (LL)**, and **Three-phase (LLL)**—based on input features like voltage, current, power load, environmental conditions, and asset health.

---

## 🛠️ Tech Stack
- **Machine Learning Algorithm**: Random Forest Classifier  
- **Platform**: IBM Watsonx.AI  
- **Data Format**: CSV  
- **Feature Engineering & Hyperparameter Tuning**: Performed within Watsonx AutoAI tools  
- **Model Evaluation**: Accuracy, confusion matrix, feature importance

---

## 📥 Data Description
The input dataset includes the following features:
- `fault_id`: Unique identifier
- `fault_location_lat`, `fault_location_lon`: Geographic coordinates
- `voltage`, `current`, `power_load`: Electrical measurements
- `temperature`, `windspeed`, `weather_condition`: Environmental factors
- `maintenance_status`, `component_health`: Asset condition indicators
- `duration_of_fault`, `down_time`: Operational impact
- `fault_type`: Target label (LG, LL, LLG, LLL, etc.)

---

## 🔁 System Workflow

1. **Data Collection**  
   - Aggregated from simulated and/or historical logs  
2. **Preprocessing & Feature Engineering**  
   - Cleaned data, encoded categorical values, extracted relevant features  
3. **Model Training**  
   - Used Random Forest with hyperparameter tuning  
4. **Prediction**  
   - The trained model classifies fault type for new input instances  
5. **Evaluation**  
   - Accuracy achieved: **41%** (Initial version)  
   - Insight: Better accuracy possible with improved data and advanced models

---

## ✅ Key Features
- Multi-class classification of fault types  
- Integrated feature importance ranking  
- Scalable to real-time applications with sensor/SCADA integration  
- Built entirely on a cloud-based platform (IBM Watsonx.AI)

---

## 🔮 Future Scope
- Add fault **location prediction**  
- Improve accuracy using **deep learning (CNN/LSTM)**  
- Deploy on **edge devices** for real-time detection  
- Integrate with live **PMU/SCADA systems**  
- Expand dataset with **real-world fault events**

---

## 📈 Results
- **Model Accuracy**: 41%  
- **Challenges**: Data similarity across classes, limited real-world examples  
- **Takeaway**: Proof-of-concept successfully built; further enhancement is achievable with richer data and deeper models.

---

## 👨‍💻 Author
**Suraj Kumar K**  
For inquiries or contributions, feel free to reach out.

---

## 📄 License
This project is for educational and research purposes only.


