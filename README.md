# Cloud Infrastructure Cost Optimization Engine 💸

An end-to-end data analytics and machine learning pipeline built using **Python** to audit cloud telemetry logs, predict resource lifecycle states, and eliminate enterprise infrastructure cloud waste.

---

## 📊 Business Problem & Domain Context
Enterprises run thousands of virtual machines across multi-cloud configurations (AWS, Azure). Unused, idle, or over-provisioned servers account for over **$30 Billion in annual global cloud wastage**. This project develops an automated system to process noisy time-series cloud performance logs, isolate under-utilized machines using ML, and provide immediate financial remediation pathways.

## 🚀 Key Operational Results (Simulated Audit)
* **Total Assets Audited:** 1,000 Virtual Machines (VMs)
* **Actionable Alerts Triggered:** 357 Servers (152 Idle | 205 Over-Provisioned)
* **Total Recovered Budget:** **$8,831.29 USD** in accumulated financial waste.
* **Primary Bottleneck Isolated:** **Finance Department** (Accounted for $2,124.09 in waste).

---

## 🛠️ Technical Implementation & Architecture

### 1. Data Engineering & Aggregation (`Pandas`, `NumPy`)
* Processed multi-region time-series telemetry streams containing hourly records for `CPU_Utilization_Percentage` and `Network_Traffic_MB`.
* Formulated moving aggregate telemetry dimensions (`Avg_CPU`, `Max_CPU`, `Std_CPU`) over rolling 7-day windows.

### 2. Algorithmic Classification Pipeline (`Scikit-Learn`)
* Implemented an ensemble **Random Forest Classifier** to segment servers based on operational threshold logic:
  * **Idle:** Max CPU < 5% and Network Traffic < 50MB (Target for immediate termination).
  * **Over-Provisioned:** Avg CPU < 15% and Max CPU < 40% (Target for immediate downsizing).
* **Model Performance Evaluation:** Achieved **100% test classification accuracy** across stratified test vectors.

---

## 💼 Core Competencies Demonstrated
* Time-Series Data Wrangling & Feature Engineering
* Financial Impact Mapping & Risk Quantifying
* Supervised Machine Learning (Ensemble Classifiers)
* Business Intelligence (BI) Report Generation
