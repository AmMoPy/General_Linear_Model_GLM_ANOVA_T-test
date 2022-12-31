### Background

We've previously discussed the inner working of Ordinary least squares regression [here](https://github.com/AmMoPy/Fifty_shades_of_OLS_), it's time to focus on statistical analysis and uncovering patterns using [The General Linear Model (GLM)](https://en.wikipedia.org/wiki/General_linear_model).

##### We'll be exploring: 
- Practical application of GLM covering ANOVA and Post hoc analysis
- Importance of explanatory data analysis (EDA) in understanding data, uncovering hidden patterns and drawing correct conclusions for modeling
- Pitfalls leading to wrong conclusions

##### Following a step-by-step approach to understand individual concepts then wrapping it up with an attempt to automate parts of EDA process!


##### Table of contents

* <a href="#eda" style='color:#a52a2a'>Exploratory Data Analysis (EDA)</a>
* <a href="#uni" style='color:#a52a2a'>Univariate Analysis</a>
* <a href="#" style='color:#a52a2a'>Bivariate analysis - Numeric vs Numeric variables</a>
    * <a href="#corr" style='color:#dc143c'>Correlation</a>
    * <a href="#tl" style='color:#dc143c'>Trend Lines</a>
    * <a href="#rhomo" style='color:#dc143c'>Residuals Homoscedasticity assumption</a>
    * <a href="#rnorm" style='color:#dc143c'>Residuals Normality assumption</a>
    * <a href="#expvi" style='color:#dc143c'>Experimenting with violation fixes</a>
* <a href="#bicat" style='color:#a52a2a'>Bivariate analysis - Categorical vs Categorical variables</a>
* <a href="#bicatv" style='color:#a52a2a'>Bivariate analysis - Categorical vs numeric variables</a>
    * <a href="#anov" style='color:#dc143c'>One-way ANOVA</a>
    * <a href="#mltcom" style='color:#dc143c'>Multiple comparisons tests</a>
* <a href="#multi" style='color:#a52a2a'>Multivariate analysis</a>
* <a href="#mdl" style='color:#a52a2a'>Modeling</a>
    * <a href="#fd" style='color:#dc143c'>Full Data</a>
    * <a href="#ms" style='color:#dc143c'>Model Selection</a>
    * <a href="#sg" style='color:#dc143c'>Smokers Group</a>
    * <a href="#nsg" style='color:#dc143c'>Non-Smokers Group</a>
* <a href="#ms" style='color:#a52a2a'>Modeling Summary</a>
* <a href="#auto" style='color:#a52a2a'>Automation</a>
    * <a href="#scra" style='color:#dc143c'>Starting from scratch - Insurance Dataset</a>
    * <a href="#hp" style='color:#dc143c'>House Price Dataset</a>

Notebook @ [Kaggle](https://www.kaggle.com/code/amrmuhammad/glm-anova)
