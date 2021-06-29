# tfm_air_quality_ml_dashboard
Machine Learning Notebooks & Dashboard

![PyPI - Python Version](https://img.shields.io/pypi/pyversions/Pandas)
![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/FelixAngelMartinez/test_1)
![GitHub last commit](https://img.shields.io/github/last-commit/FelixAngelMartinez/test_1)
![GitHub all releases](https://img.shields.io/github/downloads/FelixAngelMartinez/test_1/total)
![GitHub issues](https://img.shields.io/github/issues-raw/FelixAngelMartinez/test_1)
![GitHub contributors](https://img.shields.io/github/contributors/FelixAngelMartinez/test_1)
![GitHub followers](https://img.shields.io/github/followers/FelixAngelMartinez?style=social)

## Description
Repository belonging to the development of the Master Thesis entitled "Intelligent system for monitoring indoor air quality and fight against COVID-19", which develops a system to monitor air quality in enclosed spaces using IoT devices and Machine Learning algorithms. All this developed with a Cloud approach.

This Master's Thesis has been developed within the framework of the "Master in Computer Engineering" of the University of Castilla la Mancha.

## Repository elements
In this repository there are 3 folders:
* **dashboard/**: in this directory we find the dashboard developed in Microsoft PowerBI to obtain insights from the data.
* **notebooks/**: in this directory we find 3 playbooks for Machine Learning, Extract Data Analytics and export to csv.
* **img/**: images used in the README.

## Dashborad
By using a dashboard, a large amount of information can be extracted at a glance and by personnel not specialized in data analysis. Since the dashboard is directly connected to the database, the latest values can be obtained directly from its graphical interface.
<img src="/img/dashboard.png?raw=true" width="440">

### Requirements
To run the dashboard/ directory file you need to have Microsoft PowerBI installed. The desktop version is free of charge.

## Notebooks

### Requirements
To run the notebooks from the notebooks/ directory we can do it preferably using [Google Colab](https://colab.research.google.com/), and you can also use [Azure Machine Learning Studio](https://ml.azure.com/) y [Anaconda](https://www.anaconda.com/).

The libraries needed to run the Python code are described within the code of each notebook.
### Machine Learning - Time-Series Forecasting
The time-series forecasting has been developed using the library  [Prophet](https://facebook.github.io/prophet/).
<img src="/img/co2_forecasting.png?raw=true" width="440">
<img src="/img/co2_seasonality.png?raw=true" width="440">

#### Flow
1. Query from CosmosDB
2. Dataframe procesing
3. Model fitting
4. Time-series forecasting
5. Model quality measures
6. Hyperparameter tuning

### Exploratory Data Analysis
Notebook used to perform an analysis of the data received by the CosmosDB database, finding seasonality in the data and outliers & anomalies.
<img src="/img/seasonality.png?raw=true" width="440">

#### Flow
1. Query from CosmosDB
2. Dataframe procesing
3. Exploratory Data Analysis
4. Seasonality
5. Outliers & Anomalies Detection

### Dataframe to CSV
The purpose of this notebook is to be able to export the data from the CosmosDB database to an excel file, which allows working with the data without a direct connection to the database. This allows to share the dataframe with people interested in its analysis.

## Master's thesis
The report of the project will be published in the university repository.
[UCLM Repository](https://ruidera.uclm.es/)

## License:
Project under license [LICENSE](LICENSE)

---
_Project carried out by:_
* **Félix Ángel Martínez Muela** - [Félix Ángel Martínez](https://github.com/FelixAngelMartinez)