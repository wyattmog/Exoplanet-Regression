# Exoplanet Regression Analysis

This project performs regression analysis on NASA exoplanet data to predict planetary characteristics, specifically the calculated radius of exoplanets based on various features.

## Dataset

The analysis uses the NASA Exoplanets dataset from Kaggle:

- **Source**: [NASA Exoplanets Dataset](https://www.kaggle.com/datasets/adityamishraml/nasaexoplanets)
- **Description**: Contains information about confirmed exoplanets discovered by NASA

## Project Overview

This Jupyter notebook performs a comprehensive analysis including:

1. **Data Loading and Exploration**
   - Loading exoplanet data from local CSV file
   - Initial data exploration and statistics
   - Checking for duplicates and missing values

2. **Data Preprocessing**

   - Feature engineering (creating calculated mass and radius features)
   - Encoding categorical variables (planet types)
   - Outlier detection and removal using Z-scores
   - Log transformation for skewed features
   - Feature selection based on correlation analysis

3. **Machine Learning Models**

   - Linear Regression
   - Polynomial Regression
   - Principal Components Regression (PCR)
   - Support Vector Regression (SVR)
   - Hyperparameter tuning using GridSearchCV

4. **Clustering Analysis**

   - DBSCAN clustering
   - K-Means clustering
   - Agglomerative clustering
   - 2D and 3D visualizations

5. **Model Evaluation**
   - Performance metrics (MAE, MSE, RMSE, R²)
   - Comparative analysis of different models
   - Visualization of results

## Key Features

- **Target Variable**: Calculated radius of exoplanets
- **Features**: Distance, orbital radius, calculated mass, planet type encoding
- **Preprocessing**: Outlier removal, log transformation, feature scaling
- **Models**: Multiple regression algorithms with hyperparameter optimization

## Results

The notebook compares various regression models and provides insights into:

- Model performance metrics
- Feature importance and correlations
- Clustering patterns in the data
- Optimal hyperparameters for each model

## Setup Instructions

### Prerequisites

1. **Python Environment**:
   - Python 3.7 or higher
   - Jupyter Notebook or JupyterLab

2. **Dataset**:
   - The `exoplanet.csv` file should be placed in the same directory as the notebook
   - Dataset source: [NASA Exoplanets Dataset on Kaggle](https://www.kaggle.com/datasets/adityamishraml/nasaexoplanets)

### Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/wyattmog/Exoplanet-Regression.git
   cd Exoplanet-Regression
   ```

2. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook Exoplanet_Regression.ipynb
   ```

## Usage

1. Ensure the `exoplanet.csv` file is in the same directory as the notebook
2. Run the notebook cells sequentially
3. Follow the analysis through data preprocessing, modeling, and evaluation

## File Structure

```
Exoplanet-Regression/
├── Exoplanet_Regression.ipynb    # Main analysis notebook
├── exoplanet.csv                 # NASA Exoplanets dataset
├── README.md                     # This file
└── requirements.txt              # Python dependencies
```

## Dependencies

See `requirements.txt` for a complete list of dependencies. Key libraries include:
- pandas: Data manipulation and analysis
- numpy: Numerical computing
- scikit-learn: Machine learning algorithms
- matplotlib/seaborn: Data visualization
- scipy: Statistical functions

## Contributing

Feel free to fork this project and submit pull requests for any improvements.

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

Wyatt Mogelson

## Acknowledgments

- NASA for providing the exoplanet data
- Kaggle community for hosting the dataset
- scikit-learn developers for the machine learning tools
