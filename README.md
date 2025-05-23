# 📊 Fashion Inventory EDA & Dashboard

## 🏷 Project Title  
**Understanding Stock Patterns & Discount Behavior in Fashion Inventory**

---

##  Problem Statement / Business Objective  
**How can we effectively manage stock levels by identifying patterns of overstock and stockouts across product categories and brands to improve inventory efficiency and customer satisfaction?**

---

##  About the Dataset  
- **Source**: Internal sales/inventory data (fictional or anonymized for the project)  
- **Size**: 15,000 records  
- **Format**: Excel file  

### Key Columns:
- `Brand`
- `Product Type`
- `Variant Price`
- `Compare At Price`
- `Is In Stock`
- `Discount (%)`
- `Ideal For`
- `Size`

---

##  Data Cleaning Process  
**Tools Used**: Python (Pandas), Excel  

### Steps Taken:
- Checked for nulls and missing values  
- Converted(Standardized) date columns and extracted month names for analysis
- Created new calculated columns like `Discount (%)`, `Heavy Discount`, and `Margin Segment`  
- Replaced missing values with "Null" 
- Mapped stock status into binary (1 = In Stock, 0 = Out of Stock) where needed for analysis

---

## 🔍 Exploratory Data Analysis (Key Findings)

**Performed in Python** using Jupyter Notebook  
**Full notebook:** `Day 21 and 22 Challenge - Jupyter Notebook.pdf`

### 🔗 Related Files

[📓 View Day 21 & 22 EDA Notebook (Google Drive PDF)](https://drive.google.com/file/d/17xE0jm1W58s7dIlbAu8HqgR5VzUkp05x/view?usp=drivesdk)


- **Top brands**: Anouk, Biba, and Libas dominate the stock list  
- **Most common product type**: Straight Kurta  
- **Average discount**: Nearly 40%, with some discounts up to 90%  
- **Stock split**: Close to 50/50 between In Stock and Out of Stock. In Stock (7610) vs. Out of Stock (7322) 
- **Seasonality**: Spike in deliveries around August
- **Chi-Squared Test**: No significant link between high discount and stockouts
  

### Margin Segments:
- **8,123** Low Margin products (high discount)  
- **3,519** High Margin products  
- **3,358** Medium Margin products

---

## 📊 Dashboard Summary  
**Built in Microsoft Excel**  
![image](https://github.com/user-attachments/assets/db7305b7-2d90-46a8-891c-4518f073c64a)

### Dashboard Includes:

- **KPIs**: Average Discount, Total Deliverables, No. of Brands & Products  
- **Bar Charts**: Top Brands & Product Types  
- **Line Chart**: Monthly Sales Trend  
- **Pie Chart**: Stock Status  
- **Margin Analysis**: Low vs. High Margin Products  
- **Filters**: Brand, Ideal For, Heavy Discount Flag

---

## 💡 Insights & Recommendations

| Insight | Action |
|--------|--------|
| High discounts don’t lead to higher stockouts | Focus on popular brands and better demand planning, not just price cuts |
| Most products fall under low-margin due to frequent discounting | Review pricing strategy and supplier deals to protect margins |
| “Straight Kurta” is the most overstocked product | Monitor performance vs. stock levels to avoid oversupply |
| August shows peak deliveries. | Stock up ahead of known seasonal peaks to meet demand |

---

## 🛠️ Tools Used  
- **Python** (Pandas, Matplotlib, Seaborn)  
- **Excel** (for dashboard design & interactivity)  
- **Jupyter Notebook** (for EDA and statistical analysis)

---

## ✍️ Lessons Learned / Reflections  

Cleaning and enriching data (like creating discount percentages and margin segments) adds powerful insight with simple math.  
- EDA gives direction: It helps you understand what matters before building a dashboard.  
- Simple charts tell big stories: Pie charts, bar charts, and KPI cards, when well-labeled, are enough to communicate trends to stakeholders.  
- Documenting the process forces clarity; it helps you spot gaps and explain your value to others.

---

## 🧑‍💻 Author  
**Pamella Ishiwu**  
Participant in #30DaysOfDataWithAnnie Challenge  




