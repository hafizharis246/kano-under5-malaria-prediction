# Kano Under-5 Malaria Case Prediction & Spatial Climate Pipeline (2021–2025)

## Overview
This repository contains a data-driven research project conducted in collaboration with public health researcher **Debra Ukamaha Okeh**. The study models and predicts monthly malaria transmission dynamics among children under 5 years old in Kano State, Nigeria, using multi-source environmental features derived from **Google Earth Engine (GEE)** spanning from **January 2021 to December 2025**.

Inspired by recent epidemiological machine learning literature ([*Modelling the impact of climate variability on malaria transmission dynamics across the different ecological zones in Taraba State, Nigeria: A machine learning approach*](https://www.sciencedirect.com/science/article/pii/S294992402600011X)), this work analyzes key climate drivers of malaria and provides an adaptable modeling pipeline for sub-Saharan public health analytics.

---

## Key Research Objectives
1. **Predictive Modeling:** Estimate monthly under-5 malaria incidence in Kano State using environmental predictors.
2. **Feature Importance Analysis:** Identify which environmental variables—Temperature, Rainfall, or Relative Humidity—have the strongest correlation with malaria cases.
3. **Encoding Benchmark:** Compare model performance across three temporal feature encoding techniques to capture seasonality:
   - **Cyclic Encoding** (Sine/Cosine transformations for continuous monthly representation)
   - **One-Hot Encoding**
   - **Label Encoding**
4. **Data Visualization:** Map and graph climatic trends against case counts to uncover seasonal lag effects and transmission spikes.

---

## Dataset Schema (Kano State: Jan 2021 – Dec 2025)

The Kano State training dataset consists of monthly aggregated data across six primary variables:

| Column Name | Description |
| :--- | :--- |
| `Year` | Observation year (`2021`–`2025`) |
| `Month` | Observation month (`Jan`–`Dec`) |
| `Under_5_Cases` | Reported malaria cases in children under 5 years old |
| `Temperature` | Monthly average surface/air temperature (°C) extracted via GEE |
| `Rainfall` | Total monthly precipitation (mm) extracted via GEE |
| `Relative humidity` | Monthly average relative humidity (%) extracted via GEE |

---

## Nationwide Extension & Open Data Access

Beyond Kano State, we extracted and processed **complete nationwide population data and environmental metrics for all 36 States and the Federal Capital Territory (FCT)**, structured at the **Local Government Area (LGA)** level across Nigeria.

Researchers and practitioners interested in extending this methodology to other LGAs, States, or ecological zones can access the curated dataset below:

📁 **[Access Full Nigeria LGA-Level Environmental & Population Dataset (Google Drive)](https://drive.google.com/drive/folders/1aoSfPmdjyNtSdHkprxdYZvn64-DTX0Hk?usp=drive_link)** *(Insert your Google Drive link here)*

---

## Key Findings
*(Fill in once results are finalized)*
- **Top Predictor:** [e.g., Rainfall / Relative Humidity / Temperature] demonstrated the strongest correlation with under-5 malaria outbreaks in Kano State.
- **Optimal Encoding:** [Cyclic / One-Hot / Label] encoding achieved the best predictive accuracy by maintaining smooth seasonal continuity across month transitions.

---

## Contributors & Acknowledgments
- **Hafiz Haris Mehmood** – Machine Learning Researcher
- **Debra Ukamaha Okeh** – Public Health Research Lead

- *"Modelling the impact of climate variability on malaria transmission dynamics across the different ecological zones in Taraba State, Nigeria: A machine learning approach,"* ScienceDirect, 2026. [Read Full Paper](https://www.sciencedirect.com/science/article/pii/S294992402600011X)
