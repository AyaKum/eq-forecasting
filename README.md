# Almaty Earthquake Forecasting – Dataset & Code

This repository contains the cleaned dataset and the accompanying code used in the paper:

**“Supervised Learning for Earthquake Forecasting in the Almaty Seismic Zone”**  
(accepted at *The 16th International Conference on Emerging Ubiquitous Systems and Pervasive Networks, EUSPN 2025*).

---

## Contents
- **`almaty_eq_cleaned.csv`** – Cleaned and feature-engineered earthquake catalog.  
  - Source: USGS (1960–2024), within 1000 km radius around Almaty.  
  - Columns include:
    - `time` – UTC timestamp of the earthquake event  
    - `latitude` – latitude of event (decimal degrees)  
    - `longitude` – longitude of event (decimal degrees)  
    - `depth` – focal depth in kilometers  
    - `magnitude` – magnitude (Mw) reported by USGS  
    - `rolling_mean_magnitude` – rolling average of last 10 magnitudes  
    - `time_since_last` – hours since the previous event  
    - `dist_to_strong` – geodetic distance (km) to the last Mw ≥ 6.0 earthquake  
    - `time_to_strong` – time difference (days) since the last Mw ≥ 6.0 earthquake  
    - `closest_eq_time` – timestamp of nearest strong event  
    - `closest_eq_index` – index of nearest strong event in catalog  
    - `distance_to_closest_eq` – distance (km) to nearest strong event  
    - `time_diff_to_closest_eq` – time difference (days) to nearest strong event  

- **`classification models optimization.ipynb`** – Jupyter notebook for classification task (Mw ≥ 4.5 vs Mw < 4.5).  
- **`regression models optimization.ipynb`** – Jupyter notebook for regression task (magnitude prediction).  
- **`README.md`** – Project description and instructions.  

---

## Requirements
The code was developed in Python 3.10 with the following libraries:
- `pandas`, `numpy`, `scikit-learn`  
- `xgboost`  
- `imblearn` (for ADASYN)  
- `matplotlib`, `seaborn`  
- `geopy` (for geodetic distance calculations)


## Citation
If you use this dataset/code, please cite our paper:

> Marat Nurtas, Aizhan Altaibek, Zhanibek Ydyrys, Ayazhan Kumarkhanova.  
> *Supervised Learning for Earthquake Forecasting in the Almaty Seismic Zone*.  
> Proceedings of the 16th International Conference on Emerging Ubiquitous Systems and Pervasive Networks (EUSPN 2025), Istanbul, Türkiye, October 28–30, 2025.

