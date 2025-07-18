# 🏦 Banking Risk Analytics Dashboard – Loan Risk Profiling (Simulated)

This project delivers an interactive dashboard solution for banking client and loan risk analytics. Leveraging **Power BI**, **DAX**, **Excel**, and **CSV-based relational modeling**, the analysis provides data-driven insights into lending risks, deposit trends, and customer profiles across thousands of records.

---

## 📌 Project Overview

The objective of this project is to evaluate banking clients' financial profiles and assess the likelihood of loan repayment. The solution aids banks in minimizing risk exposure through KPI tracking, advanced DAX metrics, and interactive visualizations.

Key focus areas:
- Loan and deposit profiling  
- Customer segmentation and behavior  
- Engagement timeline analysis  
- Lending risk and fee structures  
- Account type trends across client base  

---

## 🧰 Tools & Technologies

- **Power BI** – DAX, Power Query for visual analytics  
- **Excel** – Primary data source and structure  
- **CSV Files** – Modular, relational datasets  
- **PowerPoint / PDF** – Reporting and presentation  

---

## 📁 Files Included

- `Banking Dashboard (2025).pbix` – Power BI dashboard  
- `Banking Report.pdf` – Analytical summary report  
- `Banking PPT.pptx` – Project presentation  
- `Banking.xlsx` – Raw and cleaned data  
- `banking-clients.csv` – Client data  
- `banking-relationships.csv` – Relationship mapping  
- `clients.csv`, `gender.csv`, `investment-advisors.csv` – Supporting datasets  
- `README.md` – Project documentation  

---

## 📈 Key KPIs Tracked

- Total Clients  
- Total Bank Loans & Deposits  
- Credit Card Balances  
- Processing Fees Collected  
- Client Engagement Duration  
- Business Lending Segments  

---

## 🧮 DAX Measures Used

```DAX
Total Clients = DISTINCTCOUNT('Clients - Banking'[Client ID])

Bank Loan = SUM('Clients - Banking'[Bank Loans])

Total Deposit = [Bank Deposit] + [Savings Account] + [Foreign Currency Account] + [Checking Accounts]

Total Fees = SUMX('Clients - Banking', [Total Loan] * 'Clients - Banking'[Processing Fees])

Engagement Days = DATEDIFF('Clients - Banking'[Joined Bank], TODAY(), DAY)
```

## 📊 Power BI Dashboard Visuals

- 📊 **Home Overview** – Core KPIs, client counts, total loans & deposits  
- 🏦 **Loan Analysis** – Loan types, fee structures, and risk segments  
- 💰 **Deposit Analysis** – Account types, balance distribution  
- 🧮 **Client Summary** – Income brackets, gender distribution  
- 📅 **Engagement Timeline** – Client tenure and loyalty analysis  
- 📌 **Fees & Revenue** – Estimated revenue via processing fees  

---

## 🔍 Key Insights

- 🧾 Low-income clients pose a higher risk of loan default  
- 🏛 Private banks attract more clients compared to public banks  
- 🌍 Foreign currency accounts are used by niche high-net-worth clients  
- 📅 Long engagement periods indicate greater client trust and stability  
- 💵 Fees collected are proportionally higher from high-loan clients  

---

## 🚀 Getting Started

1. Clone or download the repository  
2. Open `Banking Dashboard (2025).pbix` in Power BI Desktop  
3. Explore insights using interactive filters  
4. Review `Banking Report.pdf` or `Banking PPT.pptx` for presentation content  
5. View or clean datasets from `.csv` or `Banking.xlsx` as needed  

---

## 🙋‍♂️ Author

**Piyush Agarwal**  
📧 agpiyush84@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/agpiyush84/)
