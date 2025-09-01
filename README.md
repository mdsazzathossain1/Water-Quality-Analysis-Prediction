# Water-Quality-Analysis-Prediction
This notebook analyzes drinking and irrigation water quality using statistical, multivariate, and index-based methods. It includes factor analysis, PCA, correlation analysis, Water Quality Index (WQI), and Irrigation Water Quality Index (IWQI). Both wet and dry season datasets are studied to evaluate variations in water quality.\

Key Features:

Missing value analysis and cleaning.

PCA and Factor Analysis for dimensionality reduction.

Correlation-based parameter selection.

Drinking Water Quality Index (WQI) using weighted arithmetic method.

Irrigation Water Quality Assessment with Na%, MH, PI, SAR, KI, RSC, PS, TH.

Irrigation Water Quality Index (IWQI) for overall irrigation suitability.

Seasonal comparison: wet vs dry seasons.

🔑 Step-by-Step Breakdown

Data Import & Preprocessing

Loads water quality datasets for wet and dry seasons.

Handles missing values with custom analysis functions.

Drops unnecessary attributes (ID, location codes, etc.).

Factor Analysis (Suitability Tests)

Applies Kaiser-Meyer-Olkin (KMO) Test and Bartlett’s Test of Sphericity.

Determines whether PCA and factor analysis are suitable for the dataset.

Principal Component Analysis (PCA)

Standardizes data with Z-scores.

Visualizes parameter variability with boxplots.

Generates scree plots to decide optimal components.

Extracts loadings of parameters on principal components.

Selects key water quality parameters based on loadings > 0.3.

Correlation Analysis

Generates heatmaps for parameter correlation.

Detects highly correlated features (threshold > 0.7).

Removes redundant parameters to refine feature set.

Drinking Water Quality Index (WQI)

Uses weighted arithmetic index method.

Steps:

Calculate proportional constant K.

Assign weights (Wi) to each parameter.

Compute quality rating (Qi) for each parameter.

Calculate WQI for wet & dry seasons.

Categorizes water quality into Excellent, Good, Poor, Very Poor, Unsuitable.

Irrigation Water Quality Assessment

Converts concentration from mg/L → meq/L.

Calculates various indices:

Na% (Sodium Percentage)

Magnesium Hazard (MH%)

Permeability Index (PI%)

Sodium Adsorption Ratio (SAR)

Kelley’s Index (KI)

Residual Sodium Carbonate (RSC)

Potential Salinity (PS)

Total Hardness (TH)

Summarizes seasonal water suitability for irrigation.

Irrigation Water Quality Index (IWQI)

Defines weights for each parameter using factor analysis.

Computes irrigation suitability based on IWQI.

Categorizes water as Excellent, Good, Moderate, Poor, Unsuitable for irrigation.
