# qbc8-superstore

This repository contains the analysis and insights from the **Superstore** dataset as part of the **QBC8 Data Analysis Bootcamp** by Quera. The project is conducted by **Group 4**, consisting of **Sahar Hannani** and **Behrad Badeli**.

## Project Overview

The goal of this project was to perform a comprehensive analysis of the Superstore dataset using various data analysis techniques, including **Machine Learning**, **Hypothesis Testing**, and **Power BI**. We used a variety of tools and techniques to generate valuable insights and predictions about the dataset.

## Project Structure

The project is organized as follows:

```
qbc8-superstore
├── data
│   ├── discount.csv               # Dataset with discount data
│   ├── ML
│   │   ├── confusion_shipping.csv  # Confusion matrix for shipping predictions
│   │   ├── feature_imp_profit.csv  # Feature importance for profit predictions
│   │   ├── feature_imp_ship.csv    # Feature importance for shipping predictions
│   │   ├── profit_metrics.csv      # Metrics for profit predictions
│   │   ├── shipping_metrics.csv    # Metrics for shipping predictions
│   │   ├── y_profit_predicted.csv  # Predicted profit values
│   │   └── y_profit_true.csv       # True profit values
│   ├── MLdata.csv                 # Cleaned and preprocessed dataset for ML
│   └── nodiscount.csv             # Dataset without discount data
├── db
│   └── Superstore_fixed.sql       # SQL script for data transformation and cleaning
├── flake.lock                    # Flake lock file for package management
├── flake.nix                     # Flake file for the Nix package manager
├── LICENSE                        # License file
├── notebooks
│   ├── Models.ipynb               # Jupyter notebook for machine learning models
│   └── Stats.ipynb                # Jupyter notebook for statistical analysis
├── poetry.lock                   # Poetry lock file for dependency management
├── powerBI
│   └── superstore.pbix            # Power BI project file for visualization
├── pyproject.toml                 # Python project configuration
└── README.md                     # This file
```

## Key Methods and Techniques

### Machine Learning
In this project, we used **Random Forest** for both **regression** and **classification** tasks. We tuned the model using **Grid Search** and **Cross-Validation** to improve its accuracy. 

- **Random Forest**: Used to predict both shipping and profit outcomes based on various features of the Superstore dataset.
- **Grid Search and CV**: Utilized for hyperparameter tuning to achieve optimal model performance.

### Hypothesis Testing
For the statistical analysis, we applied the **Mann-Whitney U test** to compare the distributions of two independent groups. This was due to the non-normality of the dataset. We also attempted a **log transformation** of the data to achieve normality, but it didn’t yield satisfactory results.

- **Mann-Whitney U test**: Used for non-parametric hypothesis testing, given the data’s non-normal distribution.
- **Log Transformation**: Attempted to normalize data for better hypothesis testing.

### Power BI
We used **Power BI** to create a **star schema**-based **data warehouse** and developed a **dashboard** to provide interactive visualizations of the Superstore data. The dashboard includes insights related to profits, sales, and shipping performance.

- **Star Schema**: Designed a data warehouse structure in Power BI to efficiently manage and analyze the data.
- **Dashboard**: Created a Power BI dashboard to visualize key performance metrics and trends.

## Dependency Management

This project uses **Poetry** for dependency management, ensuring a consistent and reproducible environment. To install the dependencies, run:

```bash
poetry install
```

## Getting Started

To run the project locally:

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/qbc8-superstore.git
   ```

2. Install the dependencies using Poetry:

   ```bash
   poetry install
   ```

3. Run Jupyter notebooks for analysis:

   ```bash
   jupyter notebook notebooks/Models.ipynb
   ```

4. For Power BI, open the `superstore.pbix` file in Power BI Desktop.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
