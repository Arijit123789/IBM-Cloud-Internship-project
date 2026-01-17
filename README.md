# ⚡ Power System Fault Detection & Classification

**Capstone Project | IBM Cloud Internship**

An intelligent Machine Learning system designed to enhance power grid reliability by automatically detecting and classifying electrical faults in real-time. Deployed on **IBM watsonx.ai**, this model replaces slow manual detection with instant, data-driven diagnostics.

## 🚀 Overview
Power distribution systems are the backbone of modern society but are vulnerable to critical faults like short circuits. This project leverages **Random Forest Classification** to analyze electrical signals and identify fault types immediately, helping to prevent outages and equipment damage.

## 🎯 Key Features
* **Real-Time Detection:** Instantly analyzes 6 key electrical parameters (Current & Voltage phasors).
* **Multi-Class Classification:** Distinguishes between **Normal State** and various fault types (e.g., Line-to-Ground, Line-to-Line).
* **High Accuracy:** Achieved **98.7% accuracy** on test data with high precision and recall.
* **Cloud Deployment:** Fully deployed as a REST API using **IBM watsonx.ai**.

## 🛠️ Tech Stack
* **Language:** Python
* **Libraries:** Scikit-learn, Pandas, NumPy
* **Algorithm:** Random Forest Classifier
* **Cloud Platform:** IBM Cloud (watsonx.ai)
* **Tools:** Jupyter Notebooks

## 📊 Dataset
The model was trained on the **Power System Faults Dataset** from Kaggle.
* **Inputs:** $I_a, I_b, I_c$ (Current), $V_a, V_b, V_c$ (Voltage)
* **Source:** [Kaggle - Power System Faults Dataset](https://www.kaggle.com/datasets/ziya07/power-system-faults-dataset)

## ⚙️ How It Works
1.  **Data Acquisition:** Raw electrical data is preprocessed and scaled (StandardScaler).
2.  **Model Training:** A Random Forest Classifier learns to correlate voltage/current patterns with specific fault conditions.
3.  **Deployment:** The trained model is saved and exposed via an API endpoint on IBM Cloud.
4.  **Inference:** The API accepts a JSON payload of electrical values and returns the predicted system state.

## 📈 Performance
* **Algorithm Selected:** Random Forest (Selected over SVM and ANN).
* **Accuracy:** 98.7%
* **Result:** Excellent separation between "Normal" and "Fault" states with minimal confusion between specific fault types.

## 🔮 Future Scope
* Integration with **Phasor Measurement Units (PMUs)** for live substation data.
* Deep Learning (RNN/LSTM) implementation for predictive fault analysis.
* Edge deployment for ultra-low latency detection without internet dependency.

## 👨‍💻 Author
**Arijit Bhaya**
* **Program:** IBM SkillsBuild Internship (AI & Cloud)
* **College:** University of Engineering & Management, Kolkata
* [LinkedIn](https://www.linkedin.com/in/arijit-bhaya) | [GitHub](https://github.com/Arijit123789)

---
*Developed during the AICTE x IBM SkillsBuild Internship.*
