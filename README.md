# AI-Loan-Approval-Automation-n8n
Automated loan approval system built with n8n, Google Sheets, JavaScript, and Gmail. Features risk assessment, loan decision automation, and email notifications for financial process automation.

# 🏦 AI-Powered Loan Approval Automation using n8n

## 📌 Project Overview

This project automates the loan approval process using **n8n**, **Google Sheets**, **JavaScript**, and **Gmail Automation**.

The workflow reads loan application data from Google Sheets, evaluates each applicant based on predefined financial risk assessment rules, classifies applicants into risk categories, generates loan decisions automatically, updates records in real time, and sends approval or rejection notifications through email.

This project demonstrates how workflow automation can be used in financial institutions to streamline lending operations, reduce manual effort, improve consistency, and enhance customer communication.

---

# 🎯 Objectives

* Automate loan approval decisions
* Reduce manual processing effort
* Improve operational efficiency
* Standardize risk assessment
* Generate automated email notifications
* Demonstrate workflow automation in finance
* Improve decision-making speed

---

# 🏗️ Solution Architecture

```text
Google Sheets
      ↓
Loan Application Data
      ↓
n8n Workflow
      ↓
JavaScript Risk Assessment Engine
      ↓
Risk Classification
      ↓
Loan Decision
      ↓
Update Google Sheet
      ↓
Email Notification
```

---

# ⚙️ Workflow Process

## Step 1 — Read Applicant Dataset

The workflow extracts applicant information from Google Sheets.

The dataset contains:

* Applicant Name
* Credit Score
* Monthly Income
* Existing Debt
* Employment Type
* Loan Amount
* Loan Status

---

## Step 2 — Execute Risk Assessment Logic

A JavaScript code node evaluates each application using predefined business rules.

The system checks:

* Creditworthiness
* Income Stability
* Debt Burden
* Repayment Capacity
* Loan Affordability

---

## Step 3 — Calculate Risk Category

Applicants are classified into three categories:

### 🟢 Low Risk

Characteristics:

* Credit Score ≥ 750
* Stable Income
* Low Debt-to-Income Ratio
* Strong Repayment Potential

Decision:

```text
APPROVED
```

---

### 🟡 Medium Risk

Characteristics:

* Credit Score between 650 and 749
* Moderate Debt Burden
* Requires Manual Review

Decision:

```text
UNDER REVIEW
```

---

### 🔴 High Risk

Characteristics:

* Credit Score Below 650
* High Existing Debt
* Weak Repayment Capacity

Decision:

```text
REJECTED
```

---

## Step 4 — Generate Loan Decision

Based on risk evaluation, the workflow automatically generates:

* Approved
* Rejected
* Under Review

No manual intervention is required.

---

## Step 5 — Update Google Sheet

The workflow updates:

* Risk Category
* Loan Status
* Approval Decision
* Processing Timestamp

This ensures that all records remain updated in real time.

---

## Step 6 — Send Automated Email Notification

Applicants automatically receive:

### Approval Email

Sent when the loan application meets approval criteria.

### Rejection Email

Sent when the applicant is classified as high risk.

### Review Notification

Sent when additional verification is required.

---

# 🧠 Risk Assessment Logic

| Rule | Description                   |
| ---- | ----------------------------- |
| R1   | Credit Score Evaluation       |
| R2   | Income Stability Check        |
| R3   | Debt-to-Income Ratio Analysis |
| R4   | Loan Affordability Assessment |
| R5   | Risk Categorization           |
| R6   | Decision Generation           |

---

# 📊 Risk Classification Matrix

| Credit Score | Risk Level  | Decision     |
| ------------ | ----------- | ------------ |
| 750+         | Low Risk    | Approved     |
| 650–749      | Medium Risk | Under Review |
| Below 650    | High Risk   | Rejected     |

---

# 📸 Project Screenshots

## Google Sheets Dataset

<img src="./screenshots/dataset.png.png" width="1000"/>

The dataset contains applicant details used for loan evaluation and decision-making.

---

## n8n Workflow Automation

<img src="./screenshots/workflow.png.png" width="1000"/>

The workflow demonstrates:

* Data Extraction
* Risk Assessment
* Conditional Routing
* Google Sheets Update
* Gmail Automation

---

## Loan Approval Email

<img src="./screenshots/approved-email.png.png" width="1000"/>

Automated approval email generated for eligible applicants.

---

## Loan Rejection Email

<img src="./screenshots/rejected-email.png.png" width="1000"/>

Automated rejection notification generated for high-risk applicants.

---

# 🛠️ Tech Stack

| Technology          | Purpose               |
| ------------------- | --------------------- |
| n8n                 | Workflow Automation   |
| Google Sheets       | Data Storage          |
| JavaScript          | Risk Assessment Logic |
| Gmail               | Email Automation      |
| Financial Analytics | Decision Making       |
| Risk Assessment     | Loan Evaluation       |

---

# 📂 Repository Structure

```text
AI-Loan-Approval-Automation-n8n/
│
├── README.md
├── Loan_Approval_Automation.json
│
├── screenshots/
│   ├── dataset.png.png
│   ├── workflow.png.png
│   ├── approved-email.png.png
│   └── rejected-email.png.png
│
└── dataset/
    └── Loan_Dataset.xlsx
```

---

# 🚀 Run Locally

## Step 1 — Clone Repository

```bash
git clone https://github.com/your-username/AI-Loan-Approval-Automation-n8n.git
```

---

## Step 2 — Open n8n

```text
Launch n8n
      ↓
Import Workflow JSON
      ↓
Configure Credentials
      ↓
Connect Google Sheets
      ↓
Connect Gmail
```

---

## Step 3 — Import Workflow

Import:

```text
Loan_Approval_Automation.json
```

---

## Step 4 — Configure Google Sheets

Add Google API credentials and connect the spreadsheet.

---

## Step 5 — Configure Gmail

Add Gmail credentials for automated notifications.

---

## Step 6 — Execute Workflow

Run the workflow and monitor results in Google Sheets.

---

# 📈 Business Impact

This automation provides several business benefits:

### Faster Processing

Reduces loan evaluation time significantly.

### Reduced Manual Work

Automates repetitive tasks.

### Consistent Decision Making

Ensures standardized approval criteria.

### Better Customer Communication

Applicants receive instant notifications.

### Improved Operational Efficiency

Reduces dependency on manual review processes.

---

# 💼 Skills Demonstrated

* Workflow Automation
* Financial Risk Assessment
* Loan Processing
* Business Process Automation
* Google Sheets Integration
* Gmail Automation
* JavaScript Development
* Financial Analytics

---

# 🔮 Future Improvements

* AI-Based Credit Scoring
* Machine Learning Risk Models
* Real-Time Dashboard Integration
* Power BI Reporting
* API Connectivity
* Cloud Deployment
* Predictive Risk Analytics

---

# 🎓 Academic Context

**Course:** AI Agents & Automation

**Program:** MBA (Applied Finance)

**Project Type:** Financial Process Automation

**Domain:** Loan Approval & Risk Assessment

---

# 👨‍💻 Developed By

## Jiya Gupta

MBA (Applied Finance)

Financial Analytics • Workflow Automation • Risk Assessment • Business Intelligence

GitHub: https://github.com/jiyagupta25012006-art

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

Your support helps showcase the project and encourages further development.

