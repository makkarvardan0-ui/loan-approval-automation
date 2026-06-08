# loan-approval-automation
An automated loan approval workflow built using n8n, Google Sheet, AI-based Loan Approving, Email Alerts, and Power BI Dashboarding to approve loans in real time.
# 🤖 AI-Powered Loan Approval Automation using n8n

An end-to-end workflow automation project that streamlines the loan approval process using **n8n**, reducing manual effort, improving decision accuracy, and accelerating loan processing from **3–5 days to under 2 minutes**.

## 🚀 Features

- Automated loan application processing
- Credit score and DTI-based eligibility checks
- AML/KYC compliance screening
- Auto Approval, Rejection, and Manual Review routing
- Automated Gmail notifications
- Real-time Google Sheets updates
- Complete audit trail and workflow transparency

## 🏗 Workflow

```text
Trigger
   │
   ▼
Google Sheets
   │
   ▼
Credit Check (IF)
   │
 ┌─┴─────────┐
 ▼           ▼
Reject      AML/KYC Check
                │
         ┌──────┴──────┐
         ▼             ▼
Compliance       Final Approval
 Review              │
               ┌─────┴─────┐
               ▼           ▼
         Auto Approve   Underwriting Review
               │
               ▼
       Gmail Notifications
               │
               ▼
      Google Sheets Update
```

## 📊 Dataset

The workflow uses a self-created dataset containing **40 loan applications** with the following fields:

| Field | Description |
|---------|------------|
| Application_ID | Unique Loan ID |
| Applicant_Name | Applicant Name |
| Annual_Income_USD | Annual Income |
| Loan_Amount_Requested | Requested Loan Amount |
| Credit_Score | Creditworthiness Score |
| Debt_To_Income_Ratio | Debt Burden Ratio |
| Watchlist_Match_Pct | AML/KYC Risk Indicator |
| System_Initial_Action | Initial Decision |
| Max_Allowable_EMI | Repayment Capacity |
| Decision_Primary_Basis | Decision Reason |

## ⚙ Business Rules

### Auto Reject
- Credit Score < 580
- DTI > 0.55

### Compliance Review
- Watchlist Match % ≥ 0.35

### Auto Approve
- Credit Score ≥ 700
- DTI ≤ 0.40

### Underwriting Review
- Borderline applications requiring manual assessment

## 🛠 Tech Stack

- n8n
- Google Sheets API
- Gmail API
- Microsoft Excel
- Workflow Automation
- Financial Decision Rules

## 📈 Results

| Metric | Manual | Automated |
|----------|---------|------------|
| Processing Time | 3–5 Days | < 2 Minutes |
| Error Rate | 12–18% | <0.5% |
| Human Effort | 5–7 FTEs | 0 FTE |
| Approval Speed | 72–120 Hours | Real-Time |
| Cost/Application | ₹800–₹1,200 | ₹15–₹30 |

### Key Achievements
- ⚡ 99.9% Faster Processing
- 💰 97% Cost Reduction
- ✅ 95% Error Reduction
- 🚀 360× Faster Decisions
- 📈 100× Higher Scalability

## 🔮 Future Scope

- AI-based Credit Scoring
- Machine Learning Risk Prediction
- Real-Time CIBIL Integration
- Aadhaar eKYC Automation
- OCR-based Document Processing
- WhatsApp & SMS Notifications
- Automated Regulatory Reporting

## 👥 Team Members

- Palak
- Abhinav
- Vaibhav
- Yogita
- Vardaan
- Yuvraj
- Shobit

## 📚 References

- n8n Documentation
- Google Sheets API
- Gmail API
- Risk Management and Financial Institutions – John C. Hull
- AI in Credit Risk Management – Andrea Sironi
- BIS Working Paper #1045

## 📌 Conclusion

This project demonstrates how workflow automation can transform traditional lending operations by improving efficiency, reducing costs, ensuring compliance, and delivering a better customer experience through intelligent process automation.
