
# 📊 NovaRetail+ Customer Behavior Analysis




# 📌 Project Overview
NovaRetail+ is a large e-commerce platform operating in Latin America with millions of users.
 The Growth and Retention team aims to better understand customer behavior and its association with revenue generation.
This project explores a dataset of 15,000 customers to identify behavioral factors that are most strongly associated with annual revenue per user.
The analysis is exploratory and correlational, meaning the goal is to identify patterns and associations, not causal relationships.

# 🎯 Business Question
Which customer behavior factors are most strongly associated with annual revenue generation?
Understanding these relationships can help guide strategies to:
increase customer engagement


improve conversion


maximize customer lifetime value



# 📂 Dataset
The dataset contains 15,000 observations and 12 variables describing customer demographics, behavior, and revenue.
Customer behavior variables
visitas_mes


compras_mes


gasto_publicidad_dirigida


Customer attributes
edad


nivel_ingreso


miembro_premium


satisfaccion


abandono


Categorical variables
tipo_dispositivo


region


Target variable
ingreso_anual


The dataset contains no missing values.

# 🔎 Methodology
The analysis combines Exploratory Data Analysis (EDA) with multiple statistical techniques depending on the variable type.
Numerical relationships
Pearson correlation


Spearman correlation


Binary vs numerical variables
Point-biserial correlation


Categorical relationships
Cramér's V


Visualizations
Correlation heatmaps


Scatterplots


Distribution analysis


Pairplots


These methods allow the identification of associations between variables while acknowledging that correlation does not imply causation.

# 📈 Key Insights
## 1️⃣ Purchase frequency is the strongest factor associated with revenue
Evidence
Correlation between compras_mes and ingreso_anual:
Pearson: 0.97


Spearman: 0.97


Scatterplots show a clear upward relationship between purchase frequency and annual revenue.
Interpretation
Customers who make purchases more frequently tend to generate significantly higher annual revenue.
Business implication
Strategies that encourage repeat purchases could increase overall revenue.
Examples:
loyalty programs


personalized recommendations


recurring purchase incentives



## 2️⃣ Platform engagement is moderately associated with revenue
Evidence
Correlation between visitas_mes and ingreso_anual:
Pearson: 0.34


Spearman: 0.32


Interpretation
Customers who visit the platform more frequently tend to generate more revenue, although the relationship is moderate.
Business implication
Improving the conversion rate from visits to purchases may increase revenue.
Potential strategies:
personalized product recommendations


improved checkout experience


targeted promotions



## 3️⃣ Targeted advertising is associated with higher engagement
Evidence
Correlation between gasto_publicidad_dirigida and visitas_mes:
Pearson: 0.58


Spearman: 0.56


Interpretation
Users with higher targeted advertising exposure tend to visit the platform more often.
Business implication
Personalized advertising may help increase user engagement, although its direct relationship with revenue is weaker.

## 4️⃣ Demographic variables show little association with revenue
Evidence
Correlations close to zero:
edad vs ingreso_anual → 0.02


nivel_ingreso vs ingreso_anual → 0.02


Cramér's V between categorical variables also shows very weak relationships (~0.01).
Interpretation
Customer revenue appears to depend more on platform behavior than demographic characteristics.
Business implication
Behavior-based segmentation may be more effective than demographic segmentation.

# ⚠️ Limitations
This analysis is correlational, therefore:
Correlation ≠ causation
The results only show associations between variables.
Additionally, the dataset does not include potentially relevant variables such as:
average order value


product categories


promotion history


customer tenure


These factors could influence revenue and should be considered in future analyses.

# 🚀 Future Work
Possible extensions of this analysis include:
Customer segmentation
Segment customers based on behavioral patterns such as:
low engagement users


highly active users


high-value customers



Predictive modeling
Develop regression or machine learning models to predict annual customer revenue.
Potential features:
visits


purchases


marketing exposure



Churn analysis
Investigate factors associated with customer abandonment in order to improve retention strategies.

# 🧰 Tools & Technologies
Python


Pandas


NumPy


Matplotlib


Seaborn


SciPy



# 📁 Project Structure
NovaRetail_Customer_Analysis

data/
  novaretail_comportamiento_clientes_2024.csv

notebooks/
  exploratory_analysis.ipynb

images/
  correlation_heatmap.png
  scatterplots.png

README.md

# 📌 Key Takeaway
Customer revenue appears to be driven primarily by behavior within the platform, especially purchase frequency, rather than demographic characteristics.
Focusing on engagement and conversion optimization may therefore be an effective strategy for increasing revenue.

⭐ If you found this project interesting, feel free to connect with me on LinkedIn or explore more projects in my portfolio.

