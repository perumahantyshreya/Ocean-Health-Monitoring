# Smart Ocean Health Monitoring: Thermal Event Detection Using Multi-Source Data Fusion in the Bay of Bengal

## Overview
This project analyzes upper ocean thermal conditions using multi-source data fusion and machine learning to detect thermal events in the Bay of Bengal.

## Objective
- Combine MODIS, Argo, and ERA5 datasets  
- Compute ΔT and Thermal Stability Index (TSI)  
- Classify ocean thermal states  

## Methodology
- Data fusion (satellite + in-situ + wind data)
- Feature engineering (ΔT, TSI)
- Random Forest classifier

## Results
- Accuracy: **96–98%**
- Wind speed identified as most influential feature

## Tech Stack
- Python  
- xarray, pandas, numpy  
- scikit-learn  

## Key Learnings
- Multi-source fusion improves prediction accuracy  
- Thermal indicators can predict ecosystem changes early  

## Future Work
- Include biological indicators  
- Improve data resolution  
