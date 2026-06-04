# Mississippi Lake Levels Historical Comparison

Track and visualize water level trends for major Mississippi lakes over time.

## Overview

This project monitors historical water levels for:
- **Enid Lake** - North-central Mississippi
- **Grenada Lake** - North Mississippi
- **Sardis Lake** - North Mississippi
- **Pickwick Lake** - Northeast Mississippi

## Data Sources

- [USGS National Water Dashboard](https://dashboard.waterdata.usgs.gov/app/nwd/en/?aoi=wsc-lmg)
- [USGS Water Data](https://waterdata.usgs.gov/ms/nwis/current/?type=lake)

## Project Structure

```
.
├── README.md
├── data/
│   └── historical_levels.csv
├── scripts/
│   ├── fetch_historical_data.py
│   └── generate_sample_data.py
├── notebooks/
│   └── analyze_trends.ipynb
└── visualizations/
    └── plot_levels.py
```

## Getting Started

### Installation

```bash
pip install -r requirements.txt
```

### Generate Sample Data (for testing)

```bash
python scripts/generate_sample_data.py
```

### Visualize Water Levels Over Time

```bash
python visualizations/plot_levels.py
```

This will generate charts showing:
- Water level trends for each lake over years
- Comparison of all lakes on one plot
- Seasonal patterns and anomalies

### Fetch Real Historical Data from USGS

```bash
python scripts/fetch_historical_data.py
```

## Data Format

Historical data is stored in `data/historical_levels.csv`:

```
date,lake,water_level_ft,normal_level_ft
2020-01-01,Enid Lake,288.5,290.0
2020-01-15,Enid Lake,289.2,290.0
2021-01-01,Enid Lake,291.1,290.0
...
```

## Features

- ✅ Historical water level tracking
- ✅ Multi-year trend analysis
- ✅ Interactive visualizations
- ✅ Seasonal pattern detection
- ✅ Lake comparison charts
- 📋 CSV export functionality
- 🔄 Automated data collection (planned)

## Visualizations Included

1. **Individual Lake Trends** - Each lake's water level over time
2. **Comparative Overview** - All lakes on one graph
3. **Deviation from Normal** - How far each lake is from its normal level
4. **Seasonal Patterns** - Month-by-month analysis

## Contributing

Contributions welcome! Please feel free to fork and submit pull requests.

## License

MIT License
