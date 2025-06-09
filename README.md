🚗 Azure Automated ML: Chicago Parking Ticket Payment Prediction  
## Classification


## Azure ML Screenshot :![Screenshot 2025-06-08 200250](https://github.com/user-attachments/assets/c54d7b34-331e-471d-a486-cf5cd63dceba)



---

## 🔍 Overview

This project uses **Azure**'s **Automated ML (AutoML)** platform to predict whether a person will pay a Chicago parking ticket based on various features. The classification task is aimed at improving city collection strategies and understanding factors contributing to unpaid violations.

---

## ❓ Business Problem

- Can we predict if a parking ticket will remain **outstanding** or get **paid**?
- Which algorithms best classify ticket payment behavior?

---

## ⚙️ Project Configuration

| Parameter                     | Value                         |
|------------------------------|-------------------------------|
| **Target column**            | `PaymentIsOutstanding`        |
| **Primary metric**           | AUC Weighted                  |
| **Positive class label**     | 1                             |
| **Train-Test Split**         | 70/30                         |
| **Cross-validation type**    | Monte Carlo (5 runs, 20%)     |
| **Compute Instance**         | Standard_D4s_v3 (1 VM)        |
| **Max concurrent iterations**| 2                             |
| **Max nodes per iteration**  | 2                             |
| **Experiment timeout**       | 2 hours                       |

---

## 🧪 Best Model Summary

| Metric               | Value                                       |
|----------------------|---------------------------------------------|
| **Best Model**       | VotingEnsemble (3 XGBoost + 2 LightGBM)     |
| **AUC Weighted**     | 0.75607                                     |
| **Accuracy (approx)**| 75%                                         |
| **Deployment Status**| Ready to deploy                             |

> ✅ **VotingEnsemble** model provided the most robust performance, effectively combining multiple boosted classifiers.

---

## 🧠 Tools and Techniques Used

- **Azure** Machine Learning Studio  
- Automated ML Classification  
- Ensemble Modeling (XGBoost, LightGBM)  
- Monte Carlo Cross-validation  
- Model Interpretability & Deployment  
- AUC-weighted Scoring

---

## 📎 Clone This Repository

```Using bash
# Using HTTPS
git clone https://github.com/iman-ezatfar/Azure-Auto-ML-Chicago-Ticket.git
```
```Using CLI
# Using GitHub CLI
gh repo clone iman-ezatfar/Azure-Auto-ML-Chicago-Ticket
```

```Using SSH
# Using SSH
git clone git@github.com:iman-ezatfar/Azure-Auto-ML-Chicago-Ticket.git
```

## Contact

<a href="https://www.linkedin.com/in/imanezatfar"><img src="https://img.icons8.com/color/48/000000/linkedin.png" alt="LinkedIn"/></a>
<a href="mailto:iman.ezatfar89@gmail.com"><img src="https://img.icons8.com/color/48/000000/gmail.png" alt="Gmail"/></a>
