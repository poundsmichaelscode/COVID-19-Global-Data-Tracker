 COVID-19-Global-Data-Tracker

 COVID-19 Global Trends Analysis & Reporting Project

 📌 Project Overview

This project involves analyzing global COVID-19 data to track trends in cases, deaths, recoveries, and vaccinations over time and across countries. The goal is to clean and process real-world data, conduct exploratory data analysis (EDA), and present insights through compelling visualizations and narrative reporting.

 🚩 Project Objectives

* ✅ Import and clean COVID-19 global data
* ✅ Analyze time trends (cases, deaths, vaccinations)
* ✅ Compare metrics across countries/regions
* ✅ Visualize trends with charts and maps
* ✅ Communicate findings in a Jupyter Notebook or PDF report



 🗂️ Project Segments (Step-by-Step Guide)

 1️⃣ Data Collection

Goal: Obtain a reliable COVID-19 dataset.

Source: Our World in Data COVID-19 Dataset
Action: Download `owid-covid-data.csv` and save it to your working directory.

 2️⃣ Data Loading & Exploration

Goal:** Load and understand the dataset structure.

Tasks:

 Load the dataset: `pandas.read_csv()`
  View columns: `df.columns`
 Preview data: `df.head()`
 Check for missing values: `df.isnull().sum()`

Key Columns:** `date`, `location`, `total_cases`, `total_deaths`, `new_cases`, `new_deaths`, `total_vaccinations`

Tools: pandas

3️⃣ Data Cleaning

Goal: Prepare the dataset for analysis.

Tasks:

 Filter for countries of interest (e.g., Kenya, USA, India)
 Drop rows with missing critical values
 Convert `date` to datetime format: `pd.to_datetime()`
 Fill or interpolate missing numeric values

Tools: pandas

 4️⃣ Exploratory Data Analysis (EDA)

Goal: Describe and explore data trends.

Tasks:

 Plot total cases/deaths over time
 Compare daily new cases across countries
 Compute death rate: `total_deaths / total_cases`

Visualizations:

 Line charts (cases/deaths over time)
 Bar charts (top countries by total cases)
 Optional: Heatmaps for correlation analysis

Tools: matplotlib, seaborn



 5️⃣ Visualizing Vaccination Progress

Goal: Analyze and visualize vaccination rollout.

Tasks

 Plot cumulative vaccinations over time
 Compare % of vaccinated populations

Charts:

Line charts
 Optional: Pie charts for vaccinated vs. unvaccinated

Tools: matplotlib, seaborn

 6️⃣ (Optional) Choropleth Map

Goal: Visualize global case or vaccination data geographically.
Tasks:

 Prepare data with `iso_code`, `total_cases` or vaccination rate
 Create a choropleth map

Tools: Plotly Express or geopandas (advanced)

 7️⃣ Insights & Reporting

Goal: Present key findings and insights.

Tasks:

 Write 3-5 key insights (e.g., "Country X had the fastest vaccine rollout")
 Identify anomalies or interesting patterns
Use markdown cells for explanations

Deliverables:

 A well-documented Jupyter Notebook containing:

   Code
   Visualizations
   Narrative insights
Optional: Export to PDF or PowerPoint

 🛠️ Recommended Tools

 Jupyter Notebook (or VS Code + Jupyter extension)
 pandas
 matplotlib
 seaborn
 Optional: plotly, geopandas



 📤 Output Example

The final notebook/report should contain:

 Cleaned and processed data Time series plots for cases, deaths, and vaccinations
 Country comparisons
 Summary of findings in markdown
 Optional interactive maps or additional charts


 📁 Folder Structure


COVID19_Analysis_Project/
├── data/
│   └── owid-covid-data.csv
├── notebooks/
│   └── covid_analysis.ipynb
├── images/
│   └── charts_and_graphs.png
├── README.md
└── requirements.txt
 ✅ How to Run

1. Clone the repository.
2. Install required libraries: `pip install -r requirements.txt`
3. Run the Jupyter Notebook in the `notebooks/` folder.

 📚 Credits

 Data Source: Our World in Data ([https://ourworldindata.org/covid-data](https://ourworldindata.org/covid-data))
 Inspiration: Real-world data storytelling and pandemic response tracking.

 📄 License

This project is open-source and free to use under the MIT License.
