# 🎮 What Makes a Video Game Successful?

**Course:** STA 4241 - Statistical Learning  
**Project Title:** Video Game Sales Analysis  
**Team Members:** Munchootsorn Wangsriviroj, William Rocha, Jackson Windhorst, Sean Murray, Nicholas Clewley  

---

## Project Goal
The goal of this project is to understand what factors affect video game sales. Using real-world data, this project explores trends and builds predictive models to help forecast global sales based on features such as genre, platform, and ratings.

---

##  Executive Summary
This analysis uses a Kaggle dataset of 16,000+ video game records to explore what makes a video game successful.  
We examined how genre, platform, critic score, and user score influence global sales through data cleaning, visualization, and modeling.  
Linear Regression, Lasso Regression, and Decision Tree models were applied, and clustering techniques grouped games by performance.  

**Key Findings:**
- Critic scores and release timing strongly influence global sales.  
- Decision Tree performed best (R² = 0.692).  
- Cluster analysis showed most games sell modestly, with only a few blockbusters dominating sales.

---

## Model Building Process
1. **Define the Problem** – Predict global video game sales and identify key success factors.  
2. **Data Collection** – Kaggle dataset (16,000+ records, including global/regional sales, genre, platform, scores).  
3. **EDA** – Visualization of trends, correlations, and top-performing categories.  
4. **Modeling** – Linear Regression, Lasso Regression, Decision Tree, K-Means, Hierarchical Clustering.  
5. **Evaluation** – MAE, RMSE, and R² used to assess performance.  
6. **Deployment** – Insights for developers and publishers to inform future game planning.

---

## Model Evaluation

| Model | MAE | RMSE | R² |
|-------|-----|------|----|
| Linear Regression | 0.403 | 1.445 | 0.504 |
| Decision Tree | 0.202 | 1.139 | 0.692 |
| Lasso Regression | 0.202 | 1.445 | 0.5041 |

**Conclusion:**  
Decision Tree outperformed other models, providing the most accurate predictions and explaining ~69% of variance in global sales.

---

## Clustering Results

**K-Means (K=3):**
- Cluster 0: Majority of games with low sales.  
- Cluster 1: High critic scores but moderate sales.  
- Cluster 2: Top-selling hits (outliers).  

**Hierarchical Clustering:**  
Provided additional grouping confirmation but added limited new insight.

---

## Learning Algorithms Implemented
- **Linear Regression:** Baseline predictive model.  
- **Lasso Regression:** Feature selection.  
- **Decision Tree:** Variable importance and non-linear relationships.  
- **K-Means & Hierarchical Clustering:** Unsupervised grouping based on sales and scores.  

---

##  Reproducibility
All analysis and modeling are contained in the Jupyter Notebook.  
To reproduce results:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn
jupyter notebook
