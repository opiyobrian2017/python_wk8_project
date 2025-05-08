### Project title and short description
COVID-19 Global Data Tracker Project
Description
- 

### Objectives of the project
✅ Import and clean COVID-19 global data
✅ Analyze time trends (cases, deaths, vaccinations)
✅ Compare metrics across countries/regions
✅ Visualize trends with charts and maps
✅ Communicate findings in a Jupyter Notebook or PDF report

### List of tools and libraries used
- Tools
  Anaconda Jupyter Notebook

- Libraries used
pandas
numpy
matplotlib
seaborn
plotly.expres

### How to run/view the project
Use the links for the notebook by clicking the links herein:
notebook:https://nb.anaconda.cloud/jupyterhub/user/f3f165c5-43ca-4fe1-9a62-9df0203edc15/lab/tree/anaconda_projects/3abecacd-49ed-4fc7-9d55-581793031eef/wk8_covid19_project.ipynb?
Narrative: https://nb.anaconda.cloud/jupyterhub/user/f3f165c5-43ca-4fe1-9a62-9df0203edc15/lab/tree/Narrative.md?


### Any insights or reflections
-check on the narrative


### Project guide
🗂️ Project Segments (Step-by-Step Guide)
1️⃣ Data Collection

Goal: Obtain a reliable COVID-19 dataset.

✅ Data Sources:

Our World in Data COVID-19 Dataset (CSV & API)

Johns Hopkins University GitHub Repository

👉 Recommended for beginners: Use the cleaned CSV from Our World in Data (easy to load with pandas).

✅ Action:

Download owid-covid-data.csv from the above link.

Save in your working folder.


2️⃣ Data Loading & Exploration

Goal: Load the dataset and explore its structure.

✅ Tasks:

Load data using pandas.read_csv().

Check columns: df.columns.

Preview rows: df.head().

Identify missing values: df.isnull().sum().

✅ Tools:

pandas

📌 Key columns:

date, location, total_cases, total_deaths, new_cases, new_deaths, total_vaccinations, etc.


3️⃣ Data Cleaning

Goal: Prepare data for analysis.

✅ Tasks:

Filter countries of interest (e.g., Kenya, USA, India).

Drop rows with missing dates/critical values.

Convert date column to datetime: pd.to_datetime().

Handle missing numeric values with fillna() or interpolate().

✅ Tools:

pandas

4️⃣ Exploratory Data Analysis (EDA)

Goal: Generate descriptive statistics & explore trends.

✅ Tasks:

Plot total cases over time for selected countries.

Plot total deaths over time.

Compare daily new cases between countries.

Calculate the death rate: total_deaths / total_cases.

✅ Visualizations:

Line charts (cases & deaths over time).

Bar charts (top countries by total cases).

Heatmaps (optional for correlation analysis).

✅ Tools:

matplotlib

seaborn

5️⃣ Visualizing Vaccination Progress

Goal: Analyze vaccination rollouts.

✅ Tasks:

Plot cumulative vaccinations over time for selected countries.

Compare % vaccinated population.

✅ Charts:

Line charts.

Optional: Pie charts for vaccinated vs. unvaccinated.

✅ Tools:

matplotlib

seaborn

6️⃣ Optional: Build a Choropleth Map

Goal: Visualize cases or vaccination rates by country on a world map.

✅ Tools:

Plotly Express

Or geopandas (advanced)

✅ Tasks:

Prepare a dataframe with iso_code, total_cases for the latest date.

Plot a choropleth showing case density or vaccination rates.

7️⃣ Insights & Reporting

Goal: Summarize findings.

✅ Tasks:

Write 3-5 key insights from the data (e.g., "X country had the fastest vaccine rollout").

Highlight anomalies or interesting patterns.

Use markdown cells in Jupyter Notebook to write your narrative.

✅ Deliverables:

A well-documented Jupyter Notebook combining:

Code

Visualizations

Narrative explanations

Optional export: Notebook → PDF or a PowerPoint with screenshots.

🛠️ Recommended Tools:

✅ Jupyter Notebook (or VS Code with Jupyter extension)
✅ pandas
✅ matplotlib & seaborn
✅ Optional: plotly, geopandas



🌍 Helpful References:

Kaggle Dataset - https://www.kaggle.com/datasets
