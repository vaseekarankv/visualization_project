# 🌍 The Unequal Energy Divide: Power, Prosperity, and Clean Growth

> An interactive Tableau visualization exploring global energy inequality across countries — examining the links between GDP, electricity access, population, and renewable energy adoption.

---

## 📌 Project Overview

Energy access is one of the most critical markers of development, yet stark disparities persist worldwide. This project visualizes these inequalities using a **multidimensional bubble chart** in Tableau, making it easy to explore how wealth, population, and clean energy adoption intersect across nations.

The visualization highlights the **5,000 kWh per capita Energy Poverty Threshold** — a benchmark below which countries face significant development challenges.

---

## 📊 Dataset

| Source | Description |
|--------|-------------|
| [Ember Energy](https://ember-energy.org/data/yearly-electricity-data/) | Yearly electricity generation & capacity data by country |
| [World Bank](https://data.worldbank.org/indicator/SP.POP.TOTL) | Total population by country |
| [Our World in Data](https://ourworldindata.org/grapher/gdp-per-capita-worldbank-constant-usd) | GDP per capita (constant USD) |

**Key fields in the dataset (`Final_CountryOnly.csv`):**
- `Area`, `ISO3`, `Continent`, `Year`
- `GDP_per_capita`, `Electricity_per_capita_kWh`, `Population`
- `Emissions_per_capita_tonnes`, `Electricity_Access_Percent`
- `Urban_Population_Percent`, `Category`, `Subcategory`, `Variable`, `Value`
- Year-over-year absolute and percentage changes
- Membership flags: EU, OECD, G20, G7, ASEAN

---

## 🔍 Key Insights

- **Energy poverty is widespread:** Many countries in Sub-Saharan Africa and South Asia fall well below the 5,000 kWh/capita threshold.
- **GDP strongly correlates with electricity access**, but outliers reveal that wealth alone doesn't guarantee equitable energy distribution.
- **Renewable energy adoption varies dramatically** — some developing nations are leapfrogging to clean energy, while certain high-GDP countries still rely heavily on fossil fuels.
- **Population size matters:** Large bubbles (e.g., India, China) show how scale compounds both energy challenges and opportunities.

---

## 🖼️ Dashboard Preview

![Dashboard Preview](images/dashboard.png)

*The bubble chart encodes four variables simultaneously: GDP per capita (X-axis), electricity per capita (Y-axis), population (bubble size), and renewable energy share (bubble color).*

---

## ✨ Key Features

- **Multidimensional bubble chart** encoding GDP, electricity, population, and renewables
- **Interactive filters** for GDP group, region, continent, and year
- **Detailed tooltips** with per-country metrics on hover
- **Energy Poverty Threshold line** at 5,000 kWh/capita
- **OECD status grouping** for comparative analysis

---

## 🚀 How to Explore

1. Clone this repository.
2. Open `Visualization.twb` in **Tableau Desktop** (2025.2+).
3. When prompted, point to `data/Final_CountryOnly.csv` in the cloned folder.
4. Interact with the filters and tooltips to explore the data.

> **Note:** [Tableau Public](https://www.tableau.com/products/public/download) is free to download and can open `.twb` files.

---

## 📁 Repository Structure

```
├── data        
├── images/
│   └── dashboard.png               # Dashboard screenshot
├── docs/
│   └── DMV_REPORT.pdf              # Full project report
├── Visualization.twb                # Tableau workbook
├── .gitignore                       # Ignores Tableau temp files
└── README.md                        # Project documentation
```

---

## 🛠️ Tools Used

- **Tableau Desktop / Tableau Public** — visualization and dashboard design
- **Python (pandas)** — data cleaning, merging, and integration
- **Data sources** — Ember Energy, World Bank, Our World in Data

---

## 👥 Authors

Project completed by **Vaseekaran Krishnan Vinodhan** and **Avinash Rajasekar** as part of **CSC1143 Data Management & Visualisation (10631)**.

---

## 📝 License

This project is for educational and portfolio purposes. The underlying data is sourced from publicly available datasets (see references above).

---

## 💬 Feedback

Have suggestions or questions? Feel free to [open an issue](../../issues) or reach out. We'd love to hear your thoughts!
