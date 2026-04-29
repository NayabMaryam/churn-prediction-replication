# Churn Prediction — Replication Study

Replication of:
> *A Comprehensive Evaluation of Machine Learning and 
> Deep Learning Models for Churn Prediction*  
> MDPI Information, Vol. 16, Issue 7, 2025  
> DOI: https://doi.org/10.3390/info16070537

---

## Paper Details

| Field | Info |
|---|---|
| Journal | MDPI Information (Open Access) |
| Published | June 2025 |
| Paper Link | https://www.mdpi.com/2078-2489/16/7/537 |
| Models | XGBoost, LFE-CNN, DFE-CNN, Ensemble |
| Datasets | Insurance, ISP, Telecom (all Kaggle) |

---

## Replication Results vs Paper

| Dataset | Paper Target | Our Best Model | Our Accuracy | Status |
|---|---|---|---|---|
| Insurance | 95.96% | LFE-CNN | 95.83% | ✅ Close match |
| ISP | ~96% | XGBoost | 94.08% | ⚠️ 1.9% below |
| Telecom | ~98% | XGBoost | 95.05% | ⚠️ 3.0% below |

---

## Repository Structure
churn-prediction-replication/
├── notebooks/
│   ├── 01_eda.ipynb
│   ├── 02_preprocessing.ipynb
│   ├── 03_xgboost.ipynb
│   ├── 04_cnn_models.ipynb
│   └── 05_ensemble.ipynb
├── results/
│   ├── master_results.csv
│   ├── all_models_roc_curves.png
│   └── ...
├── report/
│   └── replication_report.pdf
├── requirements.txt
└── README.md

---

## How To Run

1. Open any notebook in Google Colab
2. Mount Google Drive when prompted
3. Run cells in order from top to bottom

Install dependencies:
pip install -r requirements.txt

---

## Datasets

| Dataset | Source |
|---|---|
| Insurance Churn | kaggle.com/datasets/mukulsingh/insurance-churn-prediction |
| ISP Churn | kaggle.com/datasets/mehmetsabrikunt/internet-service-churn |
| Telecom Churn | kaggle.com/datasets/mnassrib/telecom-churn-datasets |

---

## Key Findings

- LFE-CNN achieved 95.83% on Insurance — close to paper's 95.96%
- XGBoost outperformed CNNs on ISP and Telecom
- Telecom CNN underperformed due to small dataset (3,333 rows)
- ISP size discrepancy due to paper's reporting inconsistency

---

## References

AbdelAziz N.M. et al., "A Comprehensive Evaluation of Machine 
Learning and Deep Learning Models for Churn Prediction," 
Information, vol. 16, no. 7, p. 537, Jun. 2025.
