# 🌍 Renewable Energy Forecasting & Climate Data Modelling (2025–2035)

[![GitHub](https://img.shields.io/badge/GitHub-Repository-blue?logo=github)](https://github.com/AishikDas2104/Renewable-Energy-Forecasting-Climate-Data-Modelling-2025-2035-)
[![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

## 📋 Overview

This project provides a comprehensive data-driven analysis and forecasting framework for **renewable energy generation in Paris** from 2025 to 2035. It models **solar and wind energy production** using historical climate data and future projections to estimate the potential for sustainable energy transition.

### Key Features

- 🌞 **Solar Energy Modeling**: Estimates rooftop solar PV generation based on irradiance data
- 💨 **Wind Energy Forecasting**: Predicts wind turbine power output using wind speed data
- 📊 **Climate Data Integration**: Utilizes historical and projected climate datasets
- 🎯 **Multiple Scenarios**: Evaluates conservative, realistic, and aggressive adoption scenarios
- 💰 **Cost & Emissions Analysis**: Compares renewable vs. fossil fuel economics and environmental impact
- 📈 **Future Projections**: Models energy generation potential through 2035

## 🏗️ Project Structure

```
green_energy_paris/
├── config/
│   └── settings.yaml          # Configuration for scenarios and parameters
├── notebooks/
│   └── 01_data_cleaning.ipynb # Data cleaning and analysis notebook
├── raw data/                  # Raw climate datasets (not tracked in git)
├── .gitignore                 # Git ignore rules
├── README.md                  # This file
└── requirements.txt           # Python dependencies
```

## 🔧 Configuration

The project uses a flexible configuration system defined in [`config/settings.yaml`](config/settings.yaml):

### Solar Energy Parameters
- **Panel Efficiency**: 21% (High-efficiency N-type/TOPCon panels)
- **System Losses**: 13% (Optimized inverters & MPPT)
- **Rooftop Area Scenarios**:
  - Conservative: 8,000,000 m²
  - Realistic: 20,000,000 m²
  - Aggressive: 55,000,000 m²

### Wind Energy Parameters
- **Turbine Capacity**: 3.6 MW (Modern onshore turbines like Vestas V136)
- **Turbine Count Scenarios**:
  - Conservative: 50 turbines
  - Realistic: 120 turbines
  - Aggressive: 320 turbines

### Emissions & Costs
- **Emissions** (g CO₂/kWh):
  - Fossil Gas: 418
  - Solar PV: 55
  - Wind: 13
- **Costs** (€/MWh):
  - Fossil Gas: €100
  - Solar PV: €45
  - Wind: €60

## 📊 Data Sources

This project analyzes climate data for Paris, including:
- Solar irradiance (W/m²)
- Wind speed (m/s)
- Temperature
- Historical weather patterns
- Climate projection models

## 🚀 Getting Started

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook/Lab
- Conda or pip for package management

### Installation

1. **Clone the repository**:
   ```bash
   git clone git@github.com:AishikDas2104/Renewable-Energy-Forecasting-Climate-Data-Modelling-2025-2035-.git
   cd Renewable-Energy-Forecasting-Climate-Data-Modelling-2025-2035-
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   # Using conda
   conda create -n green_energy python=3.8
   conda activate green_energy
   
   # Or using venv
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

5. **Open and run** `notebooks/01_data_cleaning.ipynb`

## 📈 Analysis Workflow

1. **Data Acquisition**: Collect historical climate data for Paris
2. **Data Cleaning**: Process and validate climate datasets
3. **Feature Engineering**: Extract relevant features (irradiance, wind speed, temperature)
4. **Energy Modeling**:
   - Calculate solar PV generation using irradiance and panel parameters
   - Estimate wind power output using wind speed and turbine specifications
5. **Scenario Analysis**: Compare different adoption scenarios
6. **Economic & Environmental Impact**: Assess costs and emissions reductions
7. **Future Projections**: Forecast renewable energy potential through 2035

## 🎯 Scenarios

The project evaluates three deployment scenarios:

| Scenario | Solar Rooftop Area | Wind Turbines | Description |
|----------|-------------------|---------------|-------------|
| **Conservative** | 8 million m² | 50 | Baseline adoption with existing infrastructure |
| **Realistic** | 20 million m² | 120 | Moderate growth with policy support |
| **Aggressive** | 55 million m² | 320 | Ambitious buildout with strong political commitment |

The **active scenario** (default: aggressive) can be configured in `config/settings.yaml`.

## 📊 Expected Outcomes

This analysis aims to provide:
- Annual renewable energy generation estimates (GWh/year)
- CO₂ emissions reduction potential (tonnes/year)
- Cost savings compared to fossil fuel generation (€/year)
- Capacity factor analysis for solar and wind
- Monthly and seasonal generation patterns
- Feasibility assessment for different scenarios

## 🤝 Contributing

Contributions are welcome! Please feel free to submit issues or pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Aishik Das**
- GitHub: [@AishikDas2104](https://github.com/AishikDas2104)

## 🙏 Acknowledgments

- Climate data providers
- Renewable energy research community
- Open-source Python data science ecosystem

## 📚 Future Work

- [ ] Integration with real-time weather APIs
- [ ] Machine learning models for demand forecasting
- [ ] Interactive dashboard for scenario exploration
- [ ] Grid integration analysis
- [ ] Battery storage optimization
- [ ] Economic viability analysis with varying energy prices

---

**⭐ If you find this project useful, please consider giving it a star!**
