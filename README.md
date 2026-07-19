# Inventory Turnover & Stock Optimization (Business Data Warehouse)

This repository contains cleaned datasets, visualizations, and analysis notebooks for inventory turnover and stock-optimization experiments focused on Indian car manufacturers.

**Key ideas:** use historical sales data to analyze demand patterns, compute turnover metrics, and explore visual insights that support inventory decisions.

Contents
- Data CSVs (raw and cleaned): `all_car_data.csv`, `all_car_data_final.csv`, `all_car_data_final_high_corr.csv`, `all_car_data_final_high_corr_outlier_removed.csv`, and per-manufacturer files (`hyundai_india_inventory.csv`, `maruti_suzuki_inventory.csv`, `tata_motors_inventory.csv`).
- Correlation and profiling outputs: `correlation_matrix.csv`, `correlation_matrix_clean.csv`, `highly_correlated_pairs.csv`, `all_car_data_final_encoded.csv`.
- Visualizations: `bar_fig_all_car_data_obj/`, `box_fig_all_car_data_obj/`, `line_fig_all_car_data_obj/` (PNG/SVG plots).
- Notebook: `DWDM.ipynb` contains the main EDA, plots, and comments.
- HTML report: `all_car_data_final_encoded_profile.html` (data profile output).

Quick Start
1. Ensure you have Python 3.8+ and these packages installed:

```
pip install -r requirements.txt
```

If a `requirements.txt` is not present, install commonly used packages:

```
pip install pandas numpy matplotlib seaborn jupyter
```

2. Open the notebook and run cells interactively:

```bash
jupyter notebook DWDM.ipynb
```

3. Or view the static profile report in a browser:

```bash
start all_car_data_final_encoded_profile.html
```

What to look for
- `DWDM.ipynb` runs exploratory data analysis: distributions, correlation analysis, outlier handling, and visualization of `Units_Sold` by category (Car_Model, Car_Type, Company, Season, Region, etc.).
- Visual folders contain the generated plots used in the analysis.

Notes & Next Steps
- If you plan to reproduce the analysis, start from `all_car_data.csv` and run the notebook end-to-end.
- Consider adding a `requirements.txt` and a short script to regenerate figures automatically (useful for reproducibility).

License & Author
- Author: Yuvanshu Dadhich

Contact
- For questions or improvements, open an issue or contact the author via the GitHub repository.
