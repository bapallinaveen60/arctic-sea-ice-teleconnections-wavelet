# Arctic Sea Ice Variability and Climate Teleconnections  
### A Wavelet Analysis Approach

## 📌 Overview
Arctic sea ice plays a crucial role in the global climate system by regulating Earth’s energy balance through albedo feedback. Over recent decades, Arctic sea ice has exhibited a strong declining trend along with pronounced variability across seasonal, interannual, and decadal timescales.

This project investigates the temporal variability of Arctic Sea Ice Concentration (SIC) and its teleconnections with major climate indices using advanced time–frequency analysis techniques. A wavelet-based framework is employed to capture non-stationary relationships between sea ice and large-scale climate modes.

---

## 🌍 Study Area
The study region encompasses the Arctic Ocean and surrounding marginal seas north of ~60°N, including:
- Beaufort Sea
- Chukchi Sea
- Laptev Sea
- East Siberian Sea
- Kara Sea
- Barents Sea
- Central Arctic Basin

The spatial boundary was defined using NSIDC reference imagery and digitized into a GIS-based polygon for accurate data extraction.

---

## 📊 Data Sources
- **Sea Ice Concentration (SIC)**:  
  National Snow and Ice Data Center (NSIDC), monthly, ~25 km resolution
- **Climate Indices**:
  - ENSO (Niño 3.4)
  - North Atlantic Oscillation (NAO)
  - Arctic Oscillation (AO)  
  (NOAA)
- **Incoming Solar Radiation**:
  ERA5 reanalysis (~0.25° × 0.25°)

---

## 🎯 Objectives
- Analyze long-term and seasonal trends in Arctic sea ice concentration
- Identify dominant periodicities using Continuous Wavelet Transform (CWT)
- Examine time–frequency relationships between sea ice and climate indices using:
  - Cross Wavelet Transform (XWT)
  - Wavelet Transform Coherence (WTC)
- Investigate causal relationships using Granger causality analysis

---

## ⚙️ Methodology
The analysis pipeline includes:
1. Data collection and preprocessing
2. Time series construction and seasonality removal
3. Trend detection using Mann–Kendall test and Sen’s slope
4. Frequency analysis using FFT
5. Time–frequency analysis using CWT
6. Teleconnection analysis using XWT and WTC
7. Causality testing using Granger causality

Wavelet analysis is particularly suitable as it handles non-stationary climate signals and provides localized time–frequency information.

---

## 📈 Key Results
- Arctic sea ice concentration shows a statistically significant long-term decreasing trend
- Dominant annual (~12-month) and interannual (~2–5 year) periodicities were identified
- Strong and persistent anti-phase relationships were observed between SIC and:
  - ENSO (2–8 year band)
  - Solar radiation (especially post-2005)
- NAO and AO exhibit intermittent but significant teleconnections at interannual timescales
- Granger causality results indicate:
  - Strong short-term causal influence of solar radiation on sea ice
  - Delayed influence of NAO and AO
  - No direct causal influence detected from ENSO

---

## 🛠️ Tools & Techniques
- Python
- NumPy, Pandas
- PyWavelets
- Matplotlib, Seaborn
- Statistical trend analysis (Mann–Kendall)
- GIS (QGIS / ArcGIS for spatial preprocessing)


## 👤 Authors
**Baipilli Naveen**  
M.Tech Climate Change, IIT Hyderabad  
