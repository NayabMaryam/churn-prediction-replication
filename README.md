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
