# Studienarbeit - Patient Classification Using NLP

This research project focuses on detecting and classifying psychiatric patients based on medical records using machine learning and Natural Language Processing (NLP) techniques.

## Project Overview

The repository currently contains Jupyter notebooks used for research, data exploration, and model development. The primary goal is to analyze patient datasets to identify psychiatric conditions through disease-wise segregation and statistical analysis.

## Files and Notebooks

### 1. [Studienarbeit _Code.ipynb](Studienarbeit%20_Code.ipynb)
The main research notebook containing:
- **Data Ingestion**: Loading patient data from `Dataset.xlsx` and `MasterfileComplication.xlsx`.
- **Data Preprocessing**: Cleaning medical terminology, merging dataframes on patient `case` numbers, and segmenting psychiatric data.
- **Initial Analysis**: Preliminary classification logic and data filtering.

### 2. [Exploratory_Data_Analysis.ipynb](notebook/Exploratory_Data_Analysis.ipynb)
Located in the `notebook/` directory, this file provides deep insights into the data:
- **Disease Categories**: Detailed analysis of Abdominal, Cardiovascular, CNS, Infections, Psychiatric, and Respiratory diseases.
- **Visualizations**: Statistical distribution plots using `seaborn` and `matplotlib`.
- **Flag Generation**: Implementation of logic to identify cases with no recorded diseases (`No_Disease_Flag`).

## Core Logic

- **Data Merging**: Combines patient health records with clinical segregation files.
- **Preprocessing**: Handles missing values and drops non-essential diagnostic columns to focus on classification features.
- **Metrics**: Tracks case counts across various medical departments to establish baseline distributions.

## Dependencies

The project relies on standard Python data science libraries:
- `pandas`: Data manipulation and analysis.
- `numpy`: Numerical computing.
- `matplotlib` & `seaborn`: Data visualization.
- `openpyxl`: Excel file support.
- `re` & `string`: Text processing.

## Getting Started

To run these notebooks locally:
1. Ensure the required Excel data files are present in the root directory.
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn openpyxl
   ```
3. Open the notebooks in Jupyter Lab or VS Code and run the cells sequentially.
