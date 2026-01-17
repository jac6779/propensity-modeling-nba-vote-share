PREDICTING NBA AWARDS VOTING SHARE USING PLAYER PERFORMANCE METRICS
===================================================================

PROJECT OVERVIEW
----------------
This project investigates whether advanced NBA player performance metrics can be used to predict award voting outcomes, specifically All-NBA / MVP vote share. Using historical player-season data, the project applies exploratory analysis, feature engineering, and regression-based modeling to estimate how voters allocate award points.

The project is designed as an end-to-end applied data science case study, demonstrating the full workflow from data exploration through predictive modeling and interpretation.

BUSINESS / ANALYTICAL OBJECTIVE
-------------------------------
NBA awards voting reflects a combination of individual performance, efficiency metrics, team success, and narrative factors. This project frames voting as a predictive analytics problem:

Given a player’s season performance metrics, can we estimate their share of award votes?

Potential applications of this type of modeling include:
- Sports analytics and performance forecasting
- Evaluating consistency and bias in voting outcomes
- Ranking and comparison systems driven by performance data
- Decision-support models influenced by human judgment

DATASET DESCRIPTION
-------------------
The dataset consists of player-season level NBA data, including traditional box score statistics, advanced efficiency metrics, team-related indicators, and historical voting outcomes.

Dataset characteristics:
- Approximately 12,700 player-season records
- Each row represents a single player’s performance in a given season

Target variable:
- points_share: proportion of total award votes received by the player

EXPLORATORY DATA ANALYSIS (EDA)
-------------------------------
The EDA phase focused on:
- Understanding the distribution of award vote share
- Identifying correlations between advanced metrics and voting outcomes
- Evaluating multicollinearity among predictors
- Comparing statistical profiles of elite players versus the overall population

Key observations:
- Advanced metrics such as PER, VORP, and BPM show strong relationships with vote share
- Award voting outcomes are highly skewed, with a small number of players receiving the majority of votes
- A large portion of players receive zero vote share, making prediction challenging

DATA PREPROCESSING & FEATURE ENGINEERING
----------------------------------------
The preprocessing phase prepared a model-ready dataset suitable for regression analysis.

Key steps included:
- Cleaning and validating numeric and categorical fields
- Removing irrelevant or redundant columns
- Selecting advanced performance metrics with strong predictive signal
- Ensuring consistent data types and scaling where appropriate

The final feature set balances interpretability with predictive power.

MODELING APPROACH
-----------------
Several regression-based models were evaluated to predict player vote share.

Models used:
- Linear Regression (baseline)
- Regularized regression variants
- Tree-based regression models (where applicable)

Evaluation strategy:
- Train/test split
- Regression metrics such as R-squared and RMSE
- Feature importance analysis to interpret model behavior

KEY FINDINGS
------------
- Advanced performance metrics explain a meaningful portion of award vote share
- Metrics such as PER and VORP consistently ranked among the strongest predictors
- Linear models captured overall trends but struggled with extreme outliers (elite MVP-level seasons)
- Voting outcomes appear largely aligned with advanced analytics, though narrative and team context likely contribute additional influence beyond pure statistics

INSIGHTS & TAKEAWAYS
--------------------
- Award voting can be partially modeled as a data-driven ranking problem
- Advanced metrics serve as strong proxies for voter decision-making
- Predicting exact vote share remains difficult due to narrative effects, media exposure, and team success factors not fully captured in individual statistics

This highlights the limits of purely quantitative models in domains influenced by human judgment.

FUTURE IMPROVEMENTS
-------------------
Potential extensions of this work include:
- Reframing the problem as classification (vote vs no vote)
- Incorporating team success metrics more explicitly
- Adding temporal or narrative-based features
- Using ensemble or non-linear models for improved performance
- Comparing predicted rankings to actual voting rankings

TOOLS & TECHNOLOGIES
--------------------
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Jupyter Notebook

REPOSITORY STRUCTURE
--------------------
01_All_NBA_Vote_Share_EDA.ipynb
02_All_NBA_Vote_Share_Preprocessing.ipynb
03_All_NBA_Vote_Share_Modeling.ipynb

PORTFOLIO CONTEXT
-----------------
This project demonstrates:
- End-to-end ownership of a predictive modeling problem
- Strong data cleaning and feature engineering skills
- Applied regression modeling and evaluation
- Clear interpretation and communication of results

While the subject matter is sports analytics, the techniques used are directly transferable to marketing analytics, customer scoring models, predictive ranking systems, and other business decision-support applications.
