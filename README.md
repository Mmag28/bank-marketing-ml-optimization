# Data-Driven Multi-Channel Optimization for Banking

## Overview
This project applies **predictive modeling** and **multi-channel outreach strategies** to maximize ROI for a banking term deposit campaign.  
Starting from the [UCI Bank Marketing dataset](#data-source), the analysis demonstrates how machine learning can optimize targeting and channel sequencing to significantly improve performance compared to traditional phone-only campaigns.

---

## Project Description
The goal was to design a data-driven marketing strategy that:
1. Identifies customers most likely to subscribe to a term deposit.
2. Allocates outreach across multiple channels (SMS, App Push, Email, Phone) based on cost-effectiveness and conversion potential.
3. Operates under **real-world constraints** such as call center capacity, fixed budget, and industry channel cost benchmarks.

**Key Steps:**
- **Data Preparation**: Cleaning, feature engineering, and handling missing values.
- **Modeling**: Tested Logistic Regression, Decision Tree, Random Forest, and XGBoost.
- **Model Selection**: Chose XGBoost based on PR-AUC for imbalanced classification.
- **Scenario Simulation**: Modeled operational campaigns with budget caps, call limits, and conversion lift assumptions.

---

## Results
| Scenario               | Conversions | ROI   | Net Profit (USD) |
|------------------------|-------------|-------|------------------|
| Baseline (No Targeting)| 33.8K       | 4.93x | 9.4M             |
| XGBoost (Phone-Only)   | 141K        | 20.56x| 46.95M           |
| Multi-Channel          | 163.5K      | 24.76x| 54.93M           |

✅ **+USD 55M net profit** using multi-channel targeting compared to baseline.  
✅ **Fewer calls** needed than a phone-only targeted approach.

---

## Technical Stack
- **Languages**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Scikit-learn, XGBoost
- **Model Evaluation**: PR-AUC, ROC-AUC, F1 Score, Precision, Recall
- **Tools**: Jupyter Notebook

---

## Data Source
**Dataset**: [Bank Marketing Data Set](https://archive.ics.uci.edu/dataset/222/bank+marketing)  
**License**: Creative Commons Attribution 4.0 International (CC BY 4.0)  
**Citation**:
> Moro, S., Cortez, P., & Rita, P. (2014). A Data-Driven Approach to Predict the Success of Bank Telemarketing. *Decision Support Systems*, 62, 22–31. UCI Machine Learning Repository. [https://doi.org/10.24432/C5K306](https://doi.org/10.24432/C5K306)

---

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/banking-multichannel-optimization.git
2. Install dependencies
   pip install -r requirements.txt
3. Open the notebook in Jupyter
   jupyter notebook

Author
Marco Magnolo
