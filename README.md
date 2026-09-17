# 📊 Retail Analysis Project — Atliq Campaign Effectiveness

Analysis of two promotional campaigns (Diwali & Sankranti) across 50 stores in 10 Indian cities to measure sales & quantity growth.

## 📌 Business Context
Atliq ran Diwali and Sankranti campaigns with 5 promo types (25% OFF, 33% OFF, 50% OFF, ₹500 Cashback, BOGOF). The goal: measure campaign effectiveness and identify top/bottom performers.

## 🎯 Objectives
- Measure sales & quantity growth pre/post campaign
- Identify best/worst cities, stores, categories, and products
- Evaluate promo type effectiveness
- Diagnose reasons for underperformance

## 🗂️ Dataset
| Table | Rows | Granularity |
|-------|------|-------------|
| Products | 15 | Product-level |
| Stores | 50 | Store-level |
| Campaigns | 4 | Campaign-level |
| Events | 10,1500 | Sales-level |

## 🛠️ Tools Used
- **Power BI Desktop** — Data modeling, DAX measures, visualization
- **Power Query** — Data transformation
- **DAX** — Sales Growth %, Qty Growth %, city averages

## 📈 Key Insights
- 🎉 **Diwali** delivered **94.12% sales growth** and **155.31% qty growth** vs Sankranti's 50.87% / 66.25%
- 💰 **₹500 Cashback** was the best promo for sales growth (136.11%)
- 📦 **BOGOF** drove highest quantity growth (269.98%)
- 🏙️ **Madurai** topped city-wise growth (86.81% sales, 115.58% qty)
- 🏪 **STMDU-0** best store for sales; **STMYS-1** best for quantity
- ⚠️ **25% OFF** underperformed across all campaigns (-34.61% sales)

## 💡 Recommendations
1. Prioritize budget for volume-driven campaigns (BOGOF, Cashback)
2. Phase out 25% OFF promo
3. Investigate underperforming stores (STMYS-0, STCHE-1, STHYD-1)
4. Rework Personal Care category strategy (-34.20% sales)
5. Explore store expansion in Madurai, Bengaluru, Chennai

## 📂 Repository Structure
```
├── data/raw/           # Original CSVs
├── powerbi/            # .pbix dashboard file
├── powerbi/screenshots # Dashboard images
├── docs/               # Business context, insights, recommendations
└── sql/                # SQL exploration queries
```

## 🚀 How to Use
1. Clone the repo
2. Open `powerbi/Retail_Analysis.pbix` in Power BI Desktop
3. Refresh data source pointing to `data/raw/`
4. Explore interactive dashboard

## 👤 Author
**Noel George Mathew**
- LinkedIn: [your-link]
- GitHub: [@your-username]

## 📜 License
MIT License — see `LICENSE` file.

## ⚠️ Opening the Power BI File

The `.pbix` file includes cached data, so it will open and display 
all visuals immediately. However, if you want to refresh the data 
from source:

1. Open `powerbi/Retail_Analysis.pbix` in Power BI Desktop.
2. Go to **Home → Transform Data → Data Source Settings**.
3. Update the file paths to point to `data/raw/*.csv` in your local clone.
4. Click **Refresh**.

Data model: Products (15) → Events (10,150) ← Stores (50), Campaigns (4)
