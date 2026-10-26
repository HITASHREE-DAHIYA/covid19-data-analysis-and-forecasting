COVID-19 Data Analysis and Forecasting



Project Overview



* This project explores COVID-19 confirmed cases, deaths, and recoveries using Python. It includes visualizations of trends over       time and uses Prophet to generate a seven-day forecast from historical confirmed-case data.
* The notebook includes analyses for the overall dataset and for India.
* Note: Forecasts are exploratory estimates based on historical data. They are not medical advice or official public-health predictions.



Problem Statement



Given COVID-19 patient data, visualize and analyse trends in confirmed infections, deaths, and recoveries, and estimate the number of cases expected over the following week based on historical trends.



Objectives



• Inspect and summarize COVID-19 data.

• Visualize confirmed cases, deaths, and recoveries over time.

• Explore changes in confirmed cases using a growth-rate calculation.

• Use Prophet for a seven-day time-series forecast.

• Repeat relevant visualizations and forecasting for India.



Tools and Technologies

• Python

• Pandas

• NumPy

• Matplotlib

• Plotly

• Prophet



Project Files

• covid\_19\_project.ipynb — Jupyter notebook containing the analysis, visualizations, and forecasting workflow.

• covid\_19\_clean\_complete (1).csv — input dataset expected by the notebook. Obtain the dataset from the original course/source and place it in the notebook’s working directory, or update the file path in the notebook.

&#x20;

Workflow

1\. Import the Python libraries.

2\. Load the COVID-19 CSV file with Pandas.

3\. Inspect the dataset, summary statistics, and missing values.

4\. Convert the date field to a datetime type.

5\. Create Plotly line charts for confirmed cases, recoveries, and deaths.

6\. Explore the growth rate of confirmed cases.

7\. Prepare date and confirmed-case columns for Prophet.

8\. Fit a forecasting model and generate a seven-day forecast.

9\. Visualize the forecast and its components.

10\. Repeat the analysis for India.



How to Run

1.Download or clone the repository

•	After this project is published on GitHub, clone it with:

•	git clone <your-repository-url>

•	cd covid19-data-analysis-and-forecasting

•	Replace <your-repository-url> with the repository’s actual URL.



2\. Install the dependencies

•	Use Python 3.10 or another Python version supported by the Prophet release you install. In a terminal, run:

•	python -m pip install pandas ,numpy ,matplotlib ,plotly ,prophet 



3\. Add the dataset

Place the source CSV in the notebook’s working directory. Ensure its filename matches the path used in the notebook, or update the pd.read\_csv(...) line to match the actual filename.





4\. Launch Jupyter



•	open jupyter notebook

•	Open covid\_19\_project.ipynb and run the cells in order. If using Google Colab, upload the CSV or mount the relevant Drive folder     and update the file path as needed.



Important Validation Notes



Before relying on the results, verify the following in the notebook:



• Sort records chronologically before calculating changes over time.

• Aggregate confirmed cases by date before fitting a global Prophet model if the source contains multiple countries or regions per date.

• Filter India first and aggregate its records by date if multiple regional rows exist for the same date.

• Calculate India’s growth rate from the India time series, not by assigning it to the full dataset.

• Check for missing dates, duplicate date rows, and missing values.

• Interpret the forecast cautiously and report evaluation metrics only if the model has been evaluated on held-out historical data.

These checks are important because the source data may contain multiple records for the same date. The forecast should not be considered validated until the data preparation and model results have been checked.



Limitations



• COVID-19 reporting practices and testing rates changed over time.

• Historical trends alone cannot capture every policy change, variant, or change in public behaviour.

• Forecast accuracy depends on data quality and the modelling approach.

• Predictions are estimates and should not be interpreted as official case counts.









Future Improvements



• Add a documented data source and dataset citation.

• Improve date-wise aggregation and data validation.

• Evaluate forecast performance using a time-based holdout set and suitable metrics.

• Add saved chart images and a concise results section after verifying the notebook outputs.



Author

Hitashree Dahiya

https://www.linkedin.com/in/hitashree-dahiya



