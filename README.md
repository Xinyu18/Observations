# Ground-based SO₂ Observation Data

## 📌 Description
This repository contains the ground-based SO₂ observation data used in the study **"[Inversion of a Near-Real-Time China Gridded Hourly SO₂ Emission Inventory Using Deep Learning Combined with 3D Variational Assimilation]"**. The dataset consists of raw station measurements and quality-controlled observations for 3DVar assimilation.

## 📁 Data Structure
The data is organized into two main folders:

### **1. Raw_Observations/**  
📌 This folder contains the original station-based SO₂ observations downloaded from the **China National Environmental Monitoring Center (CNEMC)**.  
- **Format**: CSV files, one file per day.
- **Naming convention**: `china_sites_YYYYMMDD.csv` (e.g., `china_sites_20230120.csv`).

### **2. Processed_for_3DVar/**  
📌 This folder contains the quality-controlled SO₂ data used in the 3D-Variational assimilation (3DVar) experiments.  
- **Format**: TXT files, one file per hour.
- **Naming convention**: `YYYYMMDDHH.txt` (e.g., `2023012006.txt`).
- **Columns**:
  - Column 1: **Latitude** (degrees)
  - Column 2: **Longitude** (degrees)
  - Column 12: **SO₂ Concentration** (µg/m³)
  -  Other columns are included in the dataset but are not relevant to this study. Missing values are represented by `-999.000`.

## 📌 Data Source
- The raw observation data were obtained from **CNEMC (China National Environmental Monitoring Center)**:  
  🔗 [https://air.cnemc.cn:18007/](https://air.cnemc.cn:18007/)
- The processed data were generated following the quality control method described in **Chen et al. (2019)**.

## 📖 Citation & License
If you use this dataset, please cite the following sources:  
- 📄 Your paper: **"[Inversion of a Near-Real-Time China Gridded Hourly SO₂ Emission Inventory Using Deep Learning Combined with 3D Variational Assimilation]"**  
- 📄 CNEMC data source  
- 📄 Quality control reference: **Chen, D., Liu, Z., Ban, J., & Chen, M. (2019). The 2015 and 2016 wintertime air pollution in China: SO2 emission changes derived from a WRF-Chem/EnKF coupled data assimilation system. Atmospheric Chemistry and Physics, 19(13), 8619–8650. https://doi.org/10.5194/acp-19-8619-2019**  

📌 **This dataset is shared for academic use only.** Please follow CNEMC’s terms and conditions when using the raw observation data.

## 📩 Contact
For any questions, please contact:  
👤 **[Xinyu He]**  
📧 [xinyuuhe@163.com]  
🏢 [National University of Defense Technology]
