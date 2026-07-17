# Video Game Sales: Exploratory Data Analysis (EDA)

## Project Overview
This project is part of the Advance Soft Logics AI/ML Internship (Week 2 Deliverable). It encompasses a complete Exploratory Data Analysis (EDA) pipeline on historical video game sales data. The objective of this analysis is to profile, clean, aggregate, and visualize raw data to uncover actionable business insights regarding global game revenue, regional market dependencies, and genre popularity trends over time.

## Key Findings (Executive Summary)
Through programmatic data cleaning, aggregation (GroupBy & Pivot Tables), and visualization, this analysis revealed:
1. **Data Integrity:** The raw dataset required targeted cleaning. We dropped 271 rows missing release years and filled 58 missing publisher records with 'Unknown' to preserve valid sales data.
2. **Market Dominance:** The **Action** and **Sports** genres are the undisputed historical leaders, generating over 1,722 million and 1,309 million units in global sales, respectively.
3. **Regional Dependencies:** While most top Western publishers (like Electronic Arts) rely on North America for revenue, **Nintendo** leverages a massive, disproportionate market share in Japan (455M+ units).
4. **Growth Trends:** A time-series heatmap analysis indicates an explosive industry "gold rush" between 2005 and 2010, where top genres consistently pushed past 100+ million global sales annually.

## Folder Structure
```text
├── venv/                   # Isolated Python virtual environment
├── vgsales.csv             # Raw Kaggle dataset (16,000+ records)
├── eda_analysis.ipynb      # Main Jupyter Notebook with cleaning, analysis, and visuals
├── requirements.txt        # Project dependencies (pandas, matplotlib, seaborn)
└── README.md               # Project documentation
```

## Setup & Installation Instructions
To reproduce this analysis on your local machine, follow these exact steps:

**1. Clone the repository:**
```bash
git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
cd your-repo-name
```
*(Note: Replace the URL above with your actual GitHub repository link)*

**2. Set up the virtual environment:**
```bash
# For Windows
python -m venv venv
.\venv\Scripts\activate

# For Mac/Linux
python3 -m venv venv
source venv/bin/activate
```

**3. Install project dependencies:**
```bash
pip install -r requirements.txt
```

**4. Launch the Jupyter Notebook:**
```bash
jupyter notebook
```
*Once Jupyter opens in your web browser, click on `eda_analysis.ipynb` to view the code, charts, and executive summary.*

## Technologies Used
* **Python 3.x**
* **Pandas:** Data wrangling, cleaning, and multi-dimensional aggregation
* **Matplotlib & Seaborn:** Advanced data visualization (Bar Charts, Scatter Plots, Heatmaps)
* **Jupyter Notebooks:** Interactive code execution and markdown documentation
* **Git/GitHub:** Version control and incremental commit tracking
