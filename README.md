# 🦠 COVID-19 Data Analysis with Python

## 📌 Project Overview

This project explores the global spread of COVID-19 using data collected and maintained by [Our World in Data](https://github.com/owid/covid-19-data).

The analysis examines the geographical distribution of confirmed cases, the evolution of the pandemic in Italy, and hospitalization and intensive care data across selected European countries.

## 🎯 Objectives

The project aims to:

* Explore the structure and quality of the dataset
* Analyze the distribution of COVID-19 cases across continents
* Examine the evolution of total and new cases in Italy during 2022
* Compare ICU patient distributions in Italy, France, and Germany
* Analyze hospitalization data for Italy, France, Germany, and Spain
* Identify missing data and assess whether imputation would be appropriate

## 📂 Dataset

The analysis uses the [Our World in Data COVID-19 dataset](https://github.com/owid/covid-19-data/tree/master/public/data), which contains worldwide information on confirmed cases, deaths, vaccinations, hospitalizations, intensive care admissions, and demographic indicators.

The dataset is loaded directly from the following source:

[Download the OWID COVID-19 dataset](https://raw.githubusercontent.com/owid/covid-19-data/refs/heads/master/public/data/owid-covid-data.csv)

> **Note:** Our World in Data continuously maintains and updates the dataset. Historical values and results may therefore change when the notebook is executed again.

## 🔍 Analysis Workflow

### Data Exploration and Preparation

* Inspected dataset dimensions, metadata, and data types
* Examined the distinction between countries, continents, and aggregate geographical entities
* Identified and counted missing values
* Converted the `date` column to datetime format
* Extracted the year into a separate variable
* Filtered the data by country and date range
* Exported selected subsets as CSV files

### ● Global Case Distribution

The cumulative number of reported cases was calculated for each continent and compared with the global total.

The analysis found that:

* Asia accounted for approximately **38.86%** of global cases
* Europe accounted for approximately **32.60%**
* North America accounted for approximately **16.04%**
* South America accounted for approximately **8.87%**
* Oceania accounted for approximately **1.93%**
* Africa accounted for approximately **1.69%**

### ●  COVID-19 Cases in Italy

The analysis examined the evolution of total and new COVID-19 cases in Italy throughout 2022.

Days without new-case measurements were excluded because new cases were reported weekly in the dataset. The analysis shows that Italy reached approximately **25.1 million cumulative reported cases** by the final available observation of 2022.

### ● ICU Patient Comparison

A box plot was used to compare the distribution of ICU patients in Italy, France, and Germany from May 2022 through April 2023.

France and Germany showed broadly similar ICU patient distributions, with generally higher values than Italy during the period analyzed.

### ● Hospitalization Data

Hospitalization data for Italy, France, Germany, and Spain were examined for 2021.

The analysis identified complete daily data for Italy, France, and Spain. Germany had **365 missing values**, meaning that hospitalization data were unavailable for the entire year. Since no observations were recorded, replacing or imputing the missing values would not have been appropriate.

> The aggregated hospitalization figures represent the sum of daily hospitalized-patient counts and should not be interpreted as the number of unique patients or hospital admissions.

## 🛠️ Tools and Libraries

* **Python**
* **Pandas** — data loading, cleaning, filtering, and aggregation
* **Matplotlib** — chart creation and customization
* **Seaborn** — statistical data visualization
* **Jupyter Notebook** — interactive analysis and documentation

## 📊 Visualizations

The project includes:

* A pie chart showing the percentage distribution of global cases by continent
* Line charts showing total and new cases in Italy during 2022
* A box plot comparing ICU patient distributions across Italy, France, and Germany
* A bar chart comparing available hospitalization data for selected European countries

## 🎓 Project Context

This project was developed as part of the EPICODE Data Analyst program and subsequently documented as a portfolio case study.
