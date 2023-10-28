# Advanced Groundwater Level Forecasting in Memphis Aquifer

## Overview
With the pressing global challenges surrounding water scarcity, this repository showcases an in-depth scientific investigation focusing on groundwater level (GWL) forecasting in Carroll County, West Tennessee. As a part of this research, we leverage state-of-the-art time series and machine learning techniques, including ARIMA, LSTM, and a novel hybrid ARIMA-LSTM model, to accurately predict groundwater levels, drawing insights from environmental and meteorological variables.

## Table of Contents
- [Data Description](#data-description)
- [Research Methodology](#research-methodology)
- [Model Architectures](#model-architectures)
- [Key Findings](#key-findings)
- [Contributions and Impacts](#contributions-and-impacts)
- [Future Directions](#future-directions)
- [Usage and Notebooks](#usage-and-notebooks)
- [Acknowledgments](#acknowledgments)

## Data Description
The dataset offers a rich tapestry of variables that encompass:

- **Observation Wells Data**: A foundational dataset from TDA-1, an observation well that reliably measures "Water Column" and "Water Temperature."
- **Soil Moisture Arrays**: These sensors capture attributes like "degree_C Soil Temperature," “m3/m3 Water Content,” and “mS/cm Saturation Extract EC”.
- **Weather Station ATMOS Data**: Provides year-round metrics like "mm/h Max Precip Rate," "degree_C Air Temperature," and "W/m2 Solar Radiation."

Detailed data sources and their geographical representations can be found in the provided notebooks.

## Research Methodology
The research journey is segmented into:

1. **Data Exploration and Pre-processing**: Ensures data consistency, handles missing values, and detects abnormalities.
2. **Feature Engineering**: Sensitivity analysis is employed to prioritize impactful variables.
3. **Model Development**: Traditional ARIMA, Univariate LSTM, Multivariate LSTM, and our proposed hybrid ARIMA-LSTM model are meticulously crafted and evaluated.

## Model Architectures
- **ARIMA**: A linear statistical model was used as a benchmark, with the model specifics outlined in the notebooks.
- **Univariate LSTM**: Explores the time-dependent nature of groundwater levels without incorporating external variables.
- **Multivariate LSTM**: Incorporates meteorological data to enhance predictions.
- **Hybrid ARIMA+LSTM**: Our innovative model captures both linear trends (via ARIMA) and non-linear patterns (via LSTM) by integrating ARIMA residuals as input features for the LSTM.

## Key Findings
1. The hybrid ARIMA-LSTM model emerged as the most accurate, demonstrating the merit of combining linear and non-linear forecasting techniques.
2. Meteorological variables significantly influenced groundwater dynamics, revealing intricate correlations between environmental factors.
3. Notable trends, such as rising soil temperatures coinciding with increasing water levels, were observed, hinting at broader environmental impacts, possibly linked to climate change.

## Contributions and Impacts
This study bridges the gap between hydrological modeling and machine learning, offering a scientifically robust framework that can assist policymakers and stakeholders in adaptive water resource management. Moreover, it aligns with initiatives like CAESER, enriching our understanding of West Tennessee's hydrological landscape.

## Future Directions
While the research achieves significant milestones, areas for future exploration include:

- Investigating optimal weight and bias initialization in neural networks.
- Exploring alternative LSTM architectures and regularization techniques.
- Expanding the dataset to include more regions and variables, enhancing model generalizability.

## Usage and Notebooks
The project is structured as a series of Jupyter Notebooks:

- `Data Exploration and ARIMA Modelling.ipynb`: Introduction, data loading, preprocessing, and ARIMA model development.
- `Univariate LSTM.ipynb`: Development of the Univariate LSTM model.
- `Multivariate LSTM.ipynb`: Incorporation of meteorological factors to refine predictions.
- `Hybrid Model.ipynb`: Development and insights from the proposed hybrid ARIMA-LSTM model.

## Acknowledgments
We express our gratitude to Mr. Farhad from the University of Memphis and the CAESER initiative for their invaluable support and insights.
