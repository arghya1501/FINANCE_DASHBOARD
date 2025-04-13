
# 📊 Real-Time Budget & Performance Tracking

**Authors:** Arghyadip Pandey & Aritra Chakraborty

## 📁 Project Overview

This Excel project is designed to automate and simplify **budget tracking and employee performance analysis** across multiple organizations and projects. It consolidates project-wise work hours, monthly billing, and budget utilization into an easy-to-analyze, dynamic system.

---

## ⚙️ Features

- Automated **Master Data Sheet** for financial summary
- Tracks:
  - Employee work hours (weekly, monthly)
  - Project-wise and month-wise costs
  - Budget utilization & remaining percentage
- Conditional formatting to indicate:
  - 🔴 Critical (balance < 10%)
  - 🟡 Warning (balance < 25%)
  - 🟢 Healthy (balance > 25%)
- Built-in formulas for delta calculation & summaries
- Can be integrated with **Power BI** for advanced visualizations

---

## 🏢 Company-Wise Analysis

### 1. **IBM**
- Projects: A, B, C, D
- Each with 5 employees, ₹5,000,000 budget
- Key Findings:
  - Project D & B: High burn rate (21% and 29% left)
  - Project A: Most cost-efficient (54% left)
- 🔁 Recommendations:
  - Reallocate resources from Project A
  - Monitor Project D & B to avoid overruns

### 2. **IQVIA**
- Projects: E, F (7 employees), G (6 employees)
- Budget Depletion:
  - E & F have only 7% budget left
  - G retains 31%
- 🧠 Insights:
  - Heavy early spending; G has better cost retention
- ⚠️ Action:
  - Adopt G’s strategies across others
  - Monitor E & F urgently

### 3. **BAJAJ**
- Projects H & I (10 employees each)
- Project H: ₹11.6M left (26%)
- Project I: ₹9.7M left (22%)
- Recommendations:
  - Focus on Project I optimization
  - Control peak month (Month 4–7) spending

### 4. **RI**
- Projects: J–O (3–4 employees)
- Projects J (4% left) & K (overspent by 2%) are critical
- Others have 40–52% left
- Suggestion:
  - Cut costs in J & K
  - Adopt methods from N & O

### 5. **CTC**
- Projects: P (7), Q (7), R (6)
- Project P is near depletion (11% left)
- Projects Q & R maintain 43%
- Tip:
  - Audit Jan 2024 (highest spend)
  - Monitor Project P closely

---

## 📊 Master Data Sheet Automation

- Dynamic conditional formatting
- Remaining budget:
  - IQVIA = 15% → ⚠️ Warning zone
  - BAJAJ = 24% → ⚠️ Close to critical
- Recommendations:
  - Add employee allocation and billing trends
  - Automate via Power BI or Excel Slicers for real-time tracking

---

## 🔎 Excel Query Snippets (Examples)

### Total Labor Cost Calculation
```excel
=SUMIFS(WorkHours!C2:C100, WorkHours!A2:A100, "Project A") * HourlyRate
```

### Remaining Budget %
```excel
=(TotalBudget - SpentAmount)/TotalBudget
```

### Conditional Formatting Rule
```excel
=IF(Remaining%<10%, "Red", IF(Remaining%<25%, "Yellow", "Green"))
```

---

## 📌 Conclusion

A powerful Excel-based budget and performance management tool across multiple companies. Effective for visual tracking, early alerts, and budget optimization strategies.

---

## 📽️ Presentation

See the accompanying PPT for visuals, summaries, and executive insights.
