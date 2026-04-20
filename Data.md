## Dataset

This project uses a **multi-source oceanographic dataset** by integrating satellite, in-situ, and atmospheric data to analyze upper ocean thermal behavior in the Bay of Bengal.

### 🔹 Data Sources

1. **MODIS (Satellite Data)**
   - Provides **Sea Surface Temperature (SST)**
   - High spatial coverage of ocean surface conditions
   - Represents *skin temperature* of the ocean

2. **Argo Float Data (In-situ)**
   - Provides **subsurface temperature and salinity profiles**
   - Used to extract **bulk temperature (≤ 10 dbar)**
   - Enables vertical ocean structure analysis

3. **ERA5 Reanalysis Data**
   - Provides **wind speed (U10, V10 components)**
   - Used to compute **wind magnitude**
   - Captures atmospheric influence on ocean mixing

---

### 🔹 Data Processing

- All datasets were aligned spatially and temporally  
- MODIS SST and ERA5 wind data were **interpolated to Argo locations**  
- Local Solar Time (LST) was computed using longitude-based adjustment  

---

### 🔹 Derived Features

The following key features were engineered:

- **ΔT (Temperature Difference)**  
  Difference between surface (MODIS SST) and subsurface (Argo) temperature  

- **TSI (Thermal Stability Index)**  
  Measures stratification and stability of the upper ocean  

- **Wind Speed**  
  Derived from ERA5 data  

- **Local Solar Time (LST)**  
  Captures diurnal heating patterns  

---

### 🔹 Final Dataset Features

The fused dataset includes:
- Surface temperature (MODIS SST)  
- Subsurface temperature (Argo)  
- Wind speed (ERA5)  
- ΔT and TSI (engineered features)  
- Spatial coordinates (latitude, longitude)  
- Time variables  

---

### 🔹 Notes

- Due to large size and external dependencies, raw datasets are not included in this repository  
- Data can be accessed from:
  - MODIS: NASA OceanColor  
  - Argo: IFREMER ERDDAP  
  - ERA5: Copernicus Climate Data Store  
