# Pakistan: Emissions Trends, Carbon Inequality, and Climate Justice (2000–2020)

[![Course](https://img.shields.io/badge/Course-Climate%20Change%2C%20Sustainability%20and%20Development%20(212)-brightgreen)](https://www.tiss.edu/)
[![Institution](https://img.shields.io/badge/Institution-Tata%20Institute%20of%20Social%20Sciences%20(TISS)-blue)](https://www.tiss.edu/)
[![Program](https://img.shields.io/badge/Program-BS%20in%20Analytics%20%26%20Sustainability%20Studies-orange)](https://www.tiss.edu/)

---

## 📌 Project Overview

This repository contains the complete analytical submission for **Assignment I** of the course **Climate Change, Sustainability and Development (Course Code: 212)** at the **Tata Institute of Social Sciences (TISS), Mumbai**.

The project investigates **Pakistan's greenhouse gas emissions trajectory (2000–2020)**, dissecting historical emissions trends, per capita dynamics, regional and global carbon inequalities, and the ethical imperatives of climate justice in the Global South.

### 👤 Author & Academic Details
- **Student Name:** Jeel Anilkumar Markana
- **Roll Number:** M2024BSASS013
- **Program:** Bachelor of Science (BS) in Analytics and Sustainability Studies (2024–2028), Semester 4
- **Instructor / Course Guide:** Dr. Praveen Kumar
- **Assigned Country:** Pakistan
- **Submission Date:** April 2026

---

## 📂 Repository Structure

```text
Assignment_1/
│
├── README.md                                    # Comprehensive project documentation
├── Pakistan_Dashboard.html                      # Interactive HTML/Chart.js emissions dashboard
├── Final_Report.docx                            # Complete academic report with empirical analysis & citations
├── Dashboard_Speech.docx                        # Structured presentation transcript & timed talking points
├── Jeel Anilkumar Markana_M2024BSASS013_Pakistan.pdf # Final compiled PDF submission
├── Dataset_Pakistan.xlsx                        # Cleaned & consolidated time-series dataset (2000–2020)
├── Assignment - I_2026.pdf                      # Original assignment brief and evaluation criteria
│
├── Dataset/                                     # Raw data archives from primary repositories
│   ├── API_NY.GDP.PCAP.CD_DS2_en_csv_v2_46.zip  # World Bank: GDP per capita (current US$)
│   ├── API_SP.POP.TOTL_DS2_en_csv_v2_61.zip     # World Bank: Total Population
│   ├── annual-co2-emissions-per-country.filtered.zip # Our World in Data (OWID) / Global Carbon Project
│   ├── total-ghg-emissions.filtered.zip         # OWID: Total GHG emissions (Mt CO2e)
│   ├── share-of-cumulative-co2.filtered.zip     # OWID: Historical cumulative carbon share
│   └── electricity-prod-source-stacked.filtered.zip # OWID / Ember: Electricity generation by fuel source
│
└── Claude/                                      # Draft documents and research notes
    └── Jeel_Markana_M2024BSASS013_Pakistan.docx
```

---

## 🔬 Key Analytical Findings

### 1. Three Distinct Trajectory Phases (2000–2020)
* **2000–2007 (Economic Growth Phase):** Total $\text{CO}_2$ emissions expanded steadily from **103.94 Mt** to **147.90 Mt** alongside annual GDP growth rates of 5–7%, vehicle fleet expansion, and industrial energy demand.
* **2008–2015 (The Energy Crisis Plateau):** Emissions plateaued (~147–150 Mt) not as a result of decarbonization or green policy, but due to severe structural electricity shortages and rampant industrial load-shedding (up to 18 hours/day).
* **2016–2020 (The CPEC Coal Surge):** Emissions surged by **21.9%** from 176.74 Mt in 2016 to **215.51 Mt** in 2020, driven by the commissioning of large-scale coal-fired power plants (e.g., Sahiwal, Port Qasim) under the China-Pakistan Economic Corridor (CPEC).

### 2. Extreme Carbon Inequality
| Metric (2020) | Pakistan | India | Bangladesh | United States | China | World Average |
| :--- | :---: | :---: | :---: | :---: | :---: | :---: |
| **Total $\text{CO}_2$ (Mt)** | **215.51** | 2,422.73 | 95.73 | 4,689.95 | 10,896.52 | 35,158.23 |
| **Per Capita $\text{CO}_2$ (t/person)** | **0.92** | 1.73 | 0.58 | 14.14 | 7.72 | 4.48 |
| **Global Share of $\text{CO}_2$ (%)** | **0.66%** | 6.89% | 0.27% | 13.42% | 31.05% | 100.00% |
| **GDP per Capita (USD)** | **\$1,278** | \$1,907 | \$2,249 | \$63,516 | \$10,627 | \$10,938 |

### 3. The Climate Justice Paradox
* **Subsistence vs. Luxury Emissions:** Pakistan's emissions remain fundamentally **subsistence-level** (basic heating, cooking, agricultural livelihoods) rather than high-consumption luxury emissions (*Shue, 1993*).
* **Disproportionate Climate Vulnerability:** While contributing merely **0.66%** to global annual $\text{CO}_2$ emissions (and less than 0.3% historically), Pakistan ranks among the top 10 most climate-vulnerable countries globally (*Germanwatch CRI*). 
* **The 2022 Climate Disaster:** Anthropogenic warming intensified monsoon precipitation and accelerated glacial melt in the Hindu Kush-Himalayas, triggering the 2022 super-floods that submerged 1/3 of the country, displaced **33 million people**, and inflicted over **\$30 billion** in economic losses (*IPCC, 2022; UNDP, 2022*).
* **Policy Imperative:** Underscores the necessity of operationalizing **Common But Differentiated Responsibilities (CBDR)** and mobilizing grant-based (non-debt) climate finance through the UNFCCC Loss and Damage mechanism.

---

## 📊 Interactive Dashboard (`Pakistan_Dashboard.html`)

An interactive dashboard built with vanilla JavaScript, CSS grid/flexbox, and **Chart.js 4.4.1** for visual exploration:

### Features & Controls
- **KPI Summary Cards:** Real-time display of 2020 Total $\text{CO}_2$, Per Capita Emissions, Global Share %, and GDP per Capita.
- **Year & Range Slicers:** Interactive pills and dropdowns enabling instant filtering across 2000–2020.
- **Visualizations:**
  1. **Figure 1:** Total $\text{CO}_2$ Emissions (2000–2020) with phase breakdowns (Growth, Plateau, CPEC Surge).
  2. **Figure 2:** Per Capita $\text{CO}_2$ Emissions (2000–2020) tracking population dynamics vs. industrial expansion.
  3. **Figure 3:** Cross-Country Per Capita Comparison (Pakistan, India, Bangladesh, China, USA, World Average).
  4. **Figure 4:** Comparative Global $\text{CO}_2$ Share (Pakistan vs. India over time).
  5. **Figure 5:** Log-Scale Scatter Plot of GDP per Capita vs. Per Capita $\text{CO}_2$ (illustrating carbon inequality).

### How to View the Dashboard
Simply open the file in any modern web browser:
```powershell
# Windows PowerShell
Start-Process "Pakistan_Dashboard.html"
```
Or double-click `Pakistan_Dashboard.html` in File Explorer.

---

## 📚 Data Sources & References

### Primary Datasets
- **Our World in Data (OWID) & Global Carbon Project:** Annual $\text{CO}_2$ emissions, total GHG emissions, and cumulative shares.
- **World Bank World Development Indicators (WDI):** Population (`SP.POP.TOTL`) and GDP per capita in current USD (`NY.GDP.PCAP.CD`).
- **Ember / Energy Institute:** Electricity generation by fuel mix.

### Key Academic References
- **Eckstein, D., Künzel, V., & Schäfer, L. (2021).** *Global Climate Risk Index 2021.* Germanwatch.
- **IPCC (2022).** *Climate Change 2022: Impacts, Adaptation and Vulnerability.* Working Group II contribution to AR6. Cambridge University Press.
- **Ritchie, H., Roser, M., et al. (2023).** *$\text{CO}_2$ and Greenhouse Gas Emissions.* Our World in Data.
- **Roberts, J. T., & Parks, B. C. (2007).** *A Climate of Injustice: Global Inequality, North-South Politics, and Climate Policy.* MIT Press.
- **Shue, H. (1993).** *Subsistence Emissions and Luxury Emissions.* Law & Policy, 15(1), 39–59.
- **Stern, D. I. (2004).** *The Rise and Fall of the Environmental Kuznets Curve.* World Development, 32(8), 1419–1439.
- **UNDP (2022).** *Pakistan: Flood Impacts 2022.* United Nations Development Programme.

---

## 📄 License & Academic Integrity

This project is prepared strictly for academic evaluation at the Tata Institute of Social Sciences (TISS). All secondary data sources and literature have been acknowledged and cited in accordance with APA 7th edition guidelines.
