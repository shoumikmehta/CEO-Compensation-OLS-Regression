# CEO Compensation and OLS Regression Analysis  

## Introduction  
This project investigates the determinants of CEO compensation across firms using Ordinary Least Squares (OLS) regression. Executive pay has been a topic of debate in corporate governance, particularly around whether it reflects firm performance or is driven by other structural factors. By combining company-level data with salary information, this study provides insights into how firm size, profitability, and industry sector influence CEO pay.  

## Data  
Two datasets were used:  
- **Companies_2025_s1.csv** – Contains firm-level characteristics including total assets, revenues, and sector classifications.  
- **Salaries_2025_s1.csv** – Provides CEO salary and compensation details for the same firms.  

The datasets were merged on a firm identifier to create a consolidated view of pay and firm metrics. Basic cleaning steps were performed to address missing values and ensure consistency. Outliers were treated using winsorization to avoid distortion from extreme pay figures.  

## Methodology  
The analysis followed a structured approach:  
1. **Descriptive Statistics** – Summary measures were calculated for CEO compensation and firm characteristics.  
2. **Visualizations** – Histograms, scatter plots, and correlation matrices were generated to highlight key relationships.  
3. **Regression Analysis** – An OLS regression model was built with CEO compensation as the dependent variable and firm-level metrics as predictors.  
4. **Model Evaluation** – The model’s explanatory power was assessed using R², adjusted R², and statistical significance of coefficients.  

## Results  
The findings indicate several consistent patterns:  
- **Firm Size Effect:** Larger firms (measured by assets and revenue) pay significantly higher compensation to their CEOs.  
- **Profitability Link:** Profitability is a statistically significant determinant, with more profitable firms rewarding CEOs with higher pay.  
- **Industry Differences:** Compensation levels vary across industries, with CEOs in technology and finance earning substantially more than those in manufacturing or service sectors.  
- **Impact of Outliers:** Extreme pay values inflated variation in the raw data. After applying winsorization, the regression model produced more robust and interpretable results.  

Overall, the final regression model explains a meaningful proportion of the variation in CEO compensation, with adjusted R² values suggesting good model fit.  

## Discussion  
These results align with established corporate governance literature, where firm size and performance are strong predictors of executive pay. However, structural differences across industries highlight that compensation is not solely tied to performance, but also influenced by sector-specific norms and competitive pressures.  

The analysis also underscores the importance of addressing outliers. Without adjustment, the distribution of CEO pay is highly skewed, which weakens regression estimates. By applying winsorization, the results better reflect typical compensation dynamics rather than being dominated by extreme cases.  

## Limitations  
While informative, the study is constrained by several factors:  
- The dataset does not include qualitative variables such as CEO experience, tenure, or board governance structures.  
- Compensation is measured only in salary terms, excluding bonuses, stock options, or other incentives.  
- The sample size, while sufficient for regression, may not generalize across all global firms.  

Future research could integrate additional variables and expand the dataset to provide a more holistic view of CEO compensation determinants.  

## Conclusion  
This project demonstrates how OLS regression can be used to explore executive compensation. The findings confirm that firm size, profitability, and sectoral differences play key roles in determining CEO pay. These insights contribute to broader debates on corporate governance, accountability, and fairness in executive remuneration.  

## How to Run  
1. Clone the repository and install dependencies listed in `requirements.txt`.  
2. Open `CEO_Compensation.ipynb` in Jupyter Notebook or Google Colab.  
3. Upload the two datasets (`Companies_2025_s1.csv` and `Salaries_2025_s1.csv`) and run all cells sequentially.  

## Author  
**Shoumik Mehta**  

