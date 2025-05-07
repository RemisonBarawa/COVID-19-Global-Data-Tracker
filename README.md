COVID-19 Global Data Tracker
Project Description
The COVID-19 Global Data Tracker is a data analysis project that visualizes and analyzes global COVID-19 trends, focusing on cases, deaths, and vaccinations for selected countries (Kenya, United States, India). Using Python and data science libraries, the project processes real-world data from Our World in Data, performs exploratory data analysis (EDA), and generates visualizations, including line plots, bar charts, and an interactive choropleth map. The results are presented in a Jupyter Notebook with narrative insights, suitable for reporting or presentation.
Objectives

Data Import and Cleaning: Load and preprocess the Our World in Data COVID-19 dataset, handling missing values and formatting dates.
Trend Analysis: Analyze time-based trends in cases, deaths, and vaccinations for selected countries.
Country Comparison: Compare metrics (cases, deaths, vaccinations) across Kenya, United States, and India.
Visualization: Create line plots, bar charts, and a choropleth map to visualize trends and geographic distribution.
Reporting: Summarize findings in a Jupyter Notebook with visualizations and written insights.

Tools and Libraries

Python 3.9+: Programming language for data analysis.
Jupyter Notebook: Interactive environment for running and documenting the analysis.
Pandas: Data manipulation and analysis.
Matplotlib: Static visualizations (line and bar plots).
Seaborn: Enhanced statistical visualizations.
Plotly Express: Interactive choropleth map.
Anaconda: Environment management and package installation.

How to Run/View the Project
Prerequisites

Anaconda (2023.09 or later) installed (anaconda.com).
Stable internet connection (for dataset download) or a local copy of owid-covid-data.csv.
Basic familiarity with Anaconda Prompt and Jupyter Notebook.

Setup

Create a Conda Environment:
Open Anaconda Prompt and run:conda create -n covid_tracker python=3.9
conda activate covid_tracker




Install Libraries:
Install required packages:conda install pandas matplotlib seaborn plotly jupyter




Download or Prepare Dataset:
The code downloads owid-covid-data.csv from Our World in Data.
If download fails, save the CSV locally and update the code to:df = pd.read_csv('owid-covid-data.csv')





Running the Project

Launch Jupyter Notebook:
Create a project folder (e.g., C:\Users\YourUsername\COVID_Tracker).
In Anaconda Prompt, navigate to the folder:cd C:\Users\YourUsername\COVID_Tracker


Start Jupyter:jupyter notebook


Alternatively, use Anaconda Navigator to launch Jupyter Notebook.


Open or Create Notebook:
In Jupyter’s browser interface (http://localhost:8888), open COVID19_Tracker.ipynb or create a new notebook and paste the project code.
Ensure the notebook is saved in the project folder.


Run the Notebook:
Run cells sequentially (Shift + Enter) to:
Load and clean data.
Generate visualizations (saved as PNGs).
Create an interactive choropleth map (saved as HTML).
Save insights (Markdown file).


The final cell outputs: Analysis complete. Visualizations saved as PNGs, choropleth map as HTML, and insights as Markdown.



Viewing Outputs

Output Files (in the working directory, e.g., C:\Users\YourUsername\COVID_Tracker):
PNG Visualizations:
total_cases_over_time.png: Line plot of cases over time.
total_cases_bar.png: Bar plot of cases on the latest date.
vaccinations_over_time.png: Line plot of vaccinations.
Open in an image viewer (e.g., Windows Photos).


HTML Map:
choropleth_map.html: Interactive map showing cases by country.
Open in a web browser (e.g., Chrome).


Markdown Insights:
insights.md: Key findings in Markdown format.
Open in a text editor or Markdown viewer (e.g., VS Code).




Check Directory:
Run in a notebook cell:import os
print(os.getcwd())
print(os.listdir())


Navigate to the printed directory in File Explorer/Finder.


Export Notebook (optional):
Save as PDF: File > Download as > PDF via LaTeX (requires conda install -c conda-forge texlive-core).
Save as HTML: File > Download as > HTML.



Insights and Reflections
Key Insights

Case Trends: The United States consistently had the highest cumulative cases, reflecting its large population and early pandemic impact.
Vaccination Rollout: India’s rapid vaccination campaign outpaced Kenya, likely due to its manufacturing capacity and population-driven urgency.
Death Rates: Kenya’s lower death rate compared to the US may stem from underreporting, demographic differences, or healthcare variations.
Anomalies: India’s 2021 case spike (likely Delta variant) highlights the impact of variants on densely populated regions.
Geographic Distribution: The choropleth map emphasizes high case density in populous countries, underscoring the need for targeted interventions.

Reflections

Data Quality: The Our World in Data dataset is comprehensive but has missing values (e.g., vaccinations), requiring careful cleaning. Interpolation for vaccinations was effective but assumes linear trends, which may oversimplify reality.
Visualization Impact: Interactive Plotly maps enhance engagement compared to static Matplotlib plots, making them ideal for presentations.
Challenges: Initial setup (e.g., Conda errors, dataset download) was complex for beginners. Using a local dataset and clear setup instructions mitigated issues.
Future Improvements:
Add more countries or metrics (e.g., hospitalization rates).
Incorporate time-series forecasting for predictive insights.
Enhance the notebook with widgets for interactive filtering.


Learning Outcome: The project reinforced skills in data cleaning, EDA, and visualization, while highlighting the importance of robust error handling and documentation for reproducibility.

