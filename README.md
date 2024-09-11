# Computer Hardware Investigation
1. Introduction <br><br>
   The CPU (Central Processing Unit) is considered to be the 'brain' of your computer. In this project, we investigate CPU performance for various CPU models produced by prominent manufacturers during the 1980s. The project explores the differences in performance amongst the most popular manufacturers in the dataset, as well as amongst the best performing manufacturers in the dataset. It explores the distributions of the numerical features in the dataset, looks at statistical characteristics of those features, and builds multiple predictive models designed to predict CPU performance based on important features. Finally, of the built models, the optimal model for predicting CPU performance is selected. <br><br>
2. Data <br><br>
   The data used in this project is sourced from the Machine Learning Repository of the University of California, Irvine:<br>
   Feldmesser, J. (1987). Computer Hardware [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5830D.<br><br>

   Explanations of the columns present in this dataset are as follows:
   - (description of predictor variables and their meaning and influence on CPU performance)
   - Vendor Name:
   - Model:
   - MYCT:
   - MMIN:
   - MMAX:
   - CACH:
   - CHMIN:
   - CHMAX:
   - PRP:
   - ERP: <br><br>
3. Project Structure and Methodology <br><br>
   - Import dataset using the API of UCI
   - Using metadata, check which dataframe/dictionary contained comprehensive information
   - Perform Exploratory Data Analysis: look at distributions, popularity, correlations
   - Use statistical visualizations to show correlations between CPU features, and differences in Vendor performance
   - Make custom statistical function to better understand the distributions of each numerical feature
   - Build predictive models: Ridge regression, Lasso Regression, Decision Trees, Random Forests
   - Enhance the predictive ability of the best performing model
   - Finally, select the overall best performing model<br><br>
4. Results and Analysis <br><br>
   - Include visualizations and evaluation metrics
   - Outline major findings and describe insightful parts of findings
   - Impact: <br><br>
5. Future Work <br><br>
   - Include the encoded version of 0th col as a feature
   - Repeat CPU performance investigation using current data (mid-2020s)
   - Determine feature weights to see which impacted performance most and least
   - Show the R^2 line plotted in a scatter plot
   - Compare my model's MAE, MSE, RMSE with those of the article's authors' ERP predictions <br><br>
