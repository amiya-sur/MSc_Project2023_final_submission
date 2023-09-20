# MSc_Project2023_final_submission
# Advanced Groundwater Level Forecasting in Memphis Aquifer - A Comparative Study of Time Series and Multivariate Analyses

This repository contains a data science project to develop robust predictive models for groundwater levels (GWL) in Carroll County, West Tennessee.

## Data

The project utilizes a real-world dataset that comprises time series measurements collected from various sources, including an observation well, soil moisture sensors, and a weather station. These data points serve as the foundation for the research and inform the predictive modeling efforts.

### Variables Studied:

#### Key Variables:

- **GWL (Groundwater Level)**: Measures water level in the well to track changes over time.
    
- **Soil Moisture**: Measures volumetric water content (m³/m³), essential for understanding the hydrological cycle in the region.
  
- **Air Temperature**: Ambient air temperature data are also included to explore its influence on soil moisture and, consequently, groundwater levels.

#### Additional Variables:

- **Water Temperature**: Measures the temperature of the water in the well, may indicate potential changes in water level with certain fluctuations in it.
  
- **Soil Temperature**: Measures soil temperature in degrees Celsius. May affect evaporation and consequently groundwater levels.
  
- **Saturation Extract EC**: Measures soil saturation extract electrical conductivity (mS/cm). May indicate mineral content affecting water flow into the aquifer.
  
- **Atmospheric Pressure**: Atmospheric pressure recorded by the datalogger (kPa). Similar to soil temperature, it may affect the rate of evaporation, thereby influencing water levels.
  
- **Max Precip Rate**: Measures maximum precipitation rate (mm/h), might have a direct relation with the rate of groundwater recharge from rainfall.
  
- **Solar Radiation**: Measures solar radiation intensity (W/m²), influencing evaporation and transpiration rates, affecting groundwater levels.

### Data Files:

Three CSV files are provided, containing the raw data for the aforementioned variables. These files include comprehensive meteorological and hydrological data essential for this study.

## Notebooks

The analysis is structured as a series of Jupyter Notebooks:

1. **Data Exploration and ARIMA Modelling**: Loads, preprocesses, and explores the dataset. Fits an ARIMA time series model as a baseline.
   
2. **Univariate LSTM**: Develops a univariate LSTM model using past GWL data only. Applies regularization via dropout.
  
3. **Multivariate LSTM**: Builds a multivariate LSTM incorporating key factors like precipitation and soil moisture identified via sensitivity analysis.
  
4. **Hybrid Model**: Proposes a novel hybrid ARIMA-LSTM model combining the strengths of both linear and nonlinear techniques.

## Key Results

- The hybrid ARIMA-LSTM model achieved the lowest RMSE and highest Nash-Sutcliffe Efficiency score on the test set.
  
- Incorporating meteorological factors improved multivariate LSTM performance over the univariate version.
  
- Overall, the data-driven models significantly outperformed the statistical ARIMA baseline.

## Contributions

This work makes a timely contribution at the intersection of hydrological modeling and machine learning. The code and notebooks provided enable reproducible research.

---

Please refer to the individual notebooks for model details and in-depth analysis. Feel free to reuse or adapt the code for your own projects.


