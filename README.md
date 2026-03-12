#Real Estate — Rent vs Buy Analyzer

I. Overview
Real Estate Rent vs Buy Analyzer answers one of the most important financial questions for urban Indians:

"Should I rent or buy a home in my city?"

Using real listing data from Indian metros, this project performs a city-level breakeven analysis, price-per-sqft comparisons, and affordability scoring to help users make informed decisions.

II. Key Findings
CityBreakeven (Years)VerdictBangalore50.2🔴 Buy ExpensiveKolkata43.4🔴 Buy ExpensiveMumbai42.2🔴 Buy ExpensiveHyderabad40.3🔴 Buy ExpensivePune39.7🔴 Buy ExpensiveChennai37.1🔴 Buy Expensive

III. Project Structure
Real-Estate-Analyzer/
│
├── notebooks/
│   └── Real_Estate_Rent_vs_Buy_Analyzer.ipynb  # Full analysis
│
├── data/
│   ├── rent_vs_buy_summary.csv                 # City-level comparison
│   └── rent_cleaned.csv                        # Cleaned rent dataset
│
└── README.md

IV. Datasets Used
Dataset                                                         Source
House Rent Prices of Metropolitan Cities in India               Kaggle
Real Estate Data from 7 Indian Cities                           Kaggle

Rent dataset: 193,011 listings across 8 cities
Buy dataset: 14,528 property listings

V. Methodology

Data Cleaning — Removed nulls, standardized city names, filtered outliers, converted price formats (₹Cr → numeric)
SQL Storage — Stored cleaned data in SQLite for structured querying
Price per SQFT Analysis — Calculated and compared rent vs buy cost per sqft
Breakeven Analysis — Divided buy price/sqft by rent price/sqft to estimate years needed to break even
Visualizations — Built interactive charts using Plotly

VI.  How to Run

1. Clone the repository
bashgit clone https://github.com/CVaruni/Real-Estate-Analyzer.git

2. Open the notebook in Google Colab or Jupyter
notebooks/Real_Estate_Rent_vs_Buy_Analyzer.ipynb

3.Upload the datasets from the data/ folder and run all cells
