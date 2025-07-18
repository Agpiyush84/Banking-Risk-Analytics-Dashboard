# 🏦 Banking Risk Analytics Dashboard

A Power BI project designed to evaluate customer profiles and support data-driven loan approvals by minimizing lending risk.

---

## 📌 Problem Statement

Understand risk analytics in banking by analyzing client data to predict loan repayment likelihood.

---

## ✅ Solution

Built interactive dashboards using **Power BI** to assess applicant profiles (loans, deposits, income) and help banks make informed decisions.

---

## 🧰 Tools Used

- Power BI (DAX, Power Query)
- Excel (data source)

---

## 📁 Dataset Overview

Multiple relational tables including:

- `Clients - Banking`
- `Banking Relationship`
- `Gender`
- `Investment Advisor`
- `Period`

---

## 🧹 Data Preparation

- Created `Engagement Timeframe` using date difference
- Binned `Estimated Income` into **Low** and **Mid** bands
- Cleaned relationships and removed duplicates

---

## 🧮 Key DAX Measures

```DAX
Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])
Bank Loan = SUM('Clients - Banking'[Bank Loans])
Total Deposit = [Bank Deposit] + [Savings Account] + [Foreign Currency Account] + [Checking Accounts]
Total Fees = SUMX('Clients - Banking', [Total Loan] * 'Clients - Banking'[Processing Fees])
Engagement Days = DATEDIFF('Clients - Banking'[Joined Bank], TODAY(), DAY)
```

## 📊 KPIs Tracked

- **Total Clients**
- **Total Loan & Deposits**
- **Business Lending**
- **Credit Card Balance**
- **Fees Collected**
- **Engagement Length**

---

## 📈 Dashboards

- **Home** – Overview of KPIs  
- **Loan Analysis** – Loan type, client segment  
- **Deposit Analysis** – Account-wise distribution  
- **Summary** – Overall banking performance  

---

## 🔍 Insights

- Low-income clients pose higher risk  
- Private banks have more clients  
- Foreign currency accounts used by select investors  
- Engagement time reveals client loyalty  

---

## 🚀 Future Enhancements

- Add credit score analysis  
- Integrate alerts for risky applicants  
- Enable what-if scenario simulation  

---

## 🙋‍♂️ Author

**Piyush Agarwal**  
📧 agpiyush84@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/agpiyush84/)
