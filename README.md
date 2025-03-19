# Consumer Price Index Analysis: India (1960–2024) 📊

This project analyzes key economic indicators for India, including:
- **Consumer Price Index (CPI)**
- **Inflation**
- **GDP Growth**
- **Interest Rates**
- **Unemployment Rates**
- **Wages**
- **Labour Force Participation Rate (LFPR)**

---

## 📁 Folder Structure

- **`Project Overview/`**: Goals, scope, and vision of the project.
- **`Data/`**: 
   - **`Data Source/`**: Raw data files and primary sources.  
     - [Dataset Source](https://github.com/ahmedmujtaba24/ahmedmujtaba24-Consumer-Price-Index-Analysis/blob/main/datasetsource.pdf)   
   - **`Processed Data/`**: Cleaned and structured data for analysis.  
     - [Golstats.xlsx](https://github.com/ahmedmujtaba24/ahmedmujtaba24-Consumer-Price-Index-Analysis/blob/main/Golstats.xlsx)
   - **`Raw Data/`**: Original, unprocessed data files.  
     - [Raw Data](https://github.com/ahmedmujtaba24/ahmedmujtaba24-Consumer-Price-Index-Analysis/blob/main/raw_data.md)
- **`Methodology/`**: Detailed approach to handling missing data and analysis.
- **`Code/`**:  
   - **`Data Frame/`**: Scripts for organizing data.  
   - **`Missing Value Handling/`**: Scripts for interpolating missing values.
- **`Report/`**: Final findings and insights.  
  - **[Report](https://drive.google.com/file/d/1kAkN1ch3SVy5YpS5PNqdQxGRywwwf7Mn/view?usp=drive_link)**  
- **`Visuals/`**: Charts and graphs showcasing trends.  
  - **[Visual Report](https://drive.google.com/file/d/19Ofx4QLmIJAC686UNN6n4FuUPUqNQtal/view?usp=drive_link)**  

---

## 📊 Key Insights
- **CPI and Inflation**: How have prices and inflation evolved over the decades?
- **Wages and LFPR**: What are the trends in wages and labor force participation?
- **Economic Events**: How did major events (e.g., 1991 liberalization, 2020 pandemic) impact the economy?

---

## 🔗 Data Sources
- **Primary**: Reserve Bank of India (RBI), Ministry of Statistics and Programme Implementation (MoSPI), Ministry of Labour and Employment.
- **Secondary**: World Bank, JSTOR, Statista.

---

## 🛠 Code Overview

### 1️⃣ **Data Preprocessing**
```python
import pandas as pd

# Load CPI data
cpi_df = pd.read_csv("Data/Raw/cpi_data.csv")
cpi_df.dropna(inplace=True)  # Remove missing values

# Save processed data
cpi_df.to_csv("Data/Processed/cpi_cleaned.csv", index=False)
