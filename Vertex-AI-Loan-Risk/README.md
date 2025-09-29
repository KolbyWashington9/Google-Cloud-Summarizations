# Vertex AI – Loan Risk Prediction

## Objective  
This lab focused on using Vertex AI AutoML to train and deploy a machine learning model that predicts loan repayment risk based on tabular data. The end-to-end workflow included preparing a dataset, training, evaluation, deployment, and generating predictions.

---

## Tools & Services Used  
- Vertex AI (AutoML for tabular data)  
- Cloud Storage (CSV dataset source)  
- Cloud Shell & curl (for predictions)  

---

## Steps Performed  
1. **Prepared the training data**  
   - Created a Vertex AI dataset named `LoanRisk`.  
   - Imported a CSV file (`loan_risk.csv`) from Cloud Storage.  
   - (Optional) Generated descriptive statistics to explore features.  

2. **Trained the AutoML model**  
   - Objective: **Classification** (predict repay = 0 or default = 1).  
   - Selected target column: `Default`.  
   - Excluded irrelevant features (e.g., ClientID).  
   - Set training budget to 1 node hour and enabled early stopping.  

3. **Evaluated the model performance** (demonstration with pretrained model)  
   - Reviewed **Precision/Recall curve** to balance threshold trade-offs.  
   - Analyzed the **Confusion Matrix**, showing strong accuracy for repay and moderate accuracy for default.  
   - Examined **Feature Importance**, identifying loan amount, income, and age as key predictive features.  

4. **Deployed the model** (demonstration steps only)  
   - Defined an endpoint in Vertex AI.  
   - Configured machine type (`e2-standard-8`) and enabled explainability with feature attribution.  
   - Connected the deployed model to the dataset for monitoring.  

5. **Generated predictions**  
   - Configured environment variables and downloaded input JSON file.  
   - Used curl to send prediction requests.  
   - Model returned confidence scores for classes `0` (repay) and `1` (default).  

---

## Key Learnings  
- Vertex AI AutoML simplifies the ML workflow: dataset import, training, evaluation, deployment, and prediction.  
- Evaluation metrics like the precision/recall curve and confusion matrix guide model performance tuning.  
- Feature importance (Explainable AI) provides transparency into model decisions.  
- Vertex AI endpoints allow scalable deployment and real-time predictions through APIs.  

---

## Real-World Application  
- **Credit risk assessment** for banks and lending institutions.  
- **Fraud detection** where categorical risk classifications are required.  
- **Customer evaluation systems** where explainability builds trust in automated decision-making.  

---

## Reflection  
This lab highlighted the power of Vertex AI AutoML in building production-ready machine learning models without extensive coding. It provided insights into the importance of evaluation metrics and feature importance, while also demonstrating how easily models can be deployed and consumed through REST endpoints.
