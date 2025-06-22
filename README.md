# 📊 Sales & Regional Insights Analysis — Jar Internship Submission

This project was developed as part of the selection process for the **Internship/PPO opportunity at [Jar](https://www.myjar.app/)**. It explores sales, profitability, target achievement, and regional performance using real-world-style retail datasets, with actionable insights and recommendations.

---

## 🧾 Objective

To analyze order, product, and target data to:
- Identify high/low-performing product categories  
- Track sales-target alignment trends  
- Discover top-performing regions  
- Provide actionable, data-driven business suggestions  

---

## 🗂️ Project Structure

```bash
jar-sales-analysis/
├── data/
│   ├── orders.csv             # Raw orders data
│   ├── order_details.csv      # Raw order‐line details
│   └── targets.csv            # Monthly sales targets
├── analysis.ipynb             # Jupyter notebook with full data pipeline, analysis, and plots
├── solution.pdf               # Written summary of insights & business recommendations
└── README.md                  # Project overview and instructions
```
---

## 📦 Datasets Used

1. **Orders Dataset**  
   Includes `Order ID`, `Order Date`, `Customer Name`, `State`, and `City`.

2. **Order Details Dataset**  
   Contains `Order ID`, `Amount`, `Profit`, `Quantity`, `Category`, and `Sub-Category`.

3. **Sales Target Dataset**  
   Provides monthly targets by `Category` in `Mon-YY` format (e.g., Apr-18).

---

## ⚙️ Tech Stack

- **Python 3.8+**  
- **Key Libraries:** `pandas`, `numpy`, `matplotlib`, `seaborn`

---

## 🧹 Data Preprocessing & Cleaning

- Dropped fully empty rows and critical NaNs (Order ID, date, state, city).  
- Converted date strings (e.g., `Apr-18`) to proper `datetime`.  
- Merged orders & order details on `Order ID`.  
- Standardized and validated all columns before analysis.

---

## 📈 Key Analysis Areas

### 1️⃣ Sales & Profitability (by Category)
- **Metrics:** Total Sales, Avg Profit per Order, Profit Margin %  
- **Top performer:** Clothing (highest margin)  
- **Underperformer:** Furniture (lowest margin despite solid revenue)  

### 2️⃣ Target Achievement (Furniture)
- Computed month-over-month % change in targets.  
- Observed stable growth (~0.9–1.9%), with spikes in Jul-18, Nov-18, Mar-19.  
- **Recommendation:** Align future targets to seasonal demand curves.

### 3️⃣ Regional Insights (Top 5 States)
- Ranked by order count → computed Total Sales & Avg Profit.  
- **Leaders:** Madhya Pradesh, Maharashtra (highest volume & revenue)  
- **High-value:** Delhi (few orders, highest avg profit)  
- **Opportunity:** Improve margins in Gujarat & Rajasthan.

---

## 💡 Business Recommendations

- **Clothing:** Scale promotions—high margin, repeat buys.  
- **Electronics:** Revisit discount strategy to boost margins.  
- **Furniture:** Optimize logistics/costs or revise pricing.  
- **Regions:** Invest further in MP & Maharashtra; explore premium offerings in Delhi.

---

## 🔮 Expansion Opportunity

**Digital Gold Donations**  
Partner with temples and trusts to allow devotees to donate certified digital gold via the Jar app—modernizing tradition, ensuring compliance, and creating a new meaningful use-case.

---

## 🚀 How to Run

1. **Clone** the repo:  
   ```bash
   git clone https://github.com/yourusername/jar-sales-analysis.git
   cd jar-sales-analysis
2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    Launch the notebook:
    jupyter notebook analysis.ipynb
    ```
