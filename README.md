# Computer Hardware Investigation
1. Introduction <br><br>
   The CPU (Central Processing Unit) is considered to be the 'brain' of your computer. In this project, we investigate CPU performance for various CPU models produced by prominent manufacturers during the 1980s. The project explores the differences in performance amongst the most popular manufacturers in the dataset, as well as amongst the best performing manufacturers in the dataset. It explores the distributions of the numerical features in the dataset, looks at statistical characteristics of those features, and builds multiple predictive models designed to predict CPU performance based on important features. Finally, of the built models, the optimal model for predicting CPU performance is selected. <br><br>
2. Data <br><br>
   The data used in this project is sourced from the Machine Learning Repository of the University of California, Irvine:<br>
   Feldmesser, J. (1987). Computer Hardware [Dataset]. UCI Machine Learning Repository. https://doi.org/10.24432/C5830D.<br><br>

   Explanations of the columns present in this dataset are as follows:
   - Vendor Name: categorical variable containing the names of the CPU manufacturers contained in this dataset.
   - Model Name: categorical variable containing the names of the models for each CPU in the dataset.
   - MYCT: Machine Cycle Time - numerical variable measured in nanoseconds. The time it takes CPU to complete 1 cycle.
   - MMIN: Main Memory Minimum - numerical variable measured in kilobytes. The minimum amount of memory the CPU can use.
   - MMAX: Main Memory Maximum - numerical variable measured in kilobytes. The maximum amount of memory the CPU can use.
   - CACH: Cache Memory - numerical variable measured in kilobytes. The amount of cache memory the CPU has.
   - CHMIN: Minimum Channels - numerical variable measured in units. The smallest number of paths for data transfer the CPU can use.
   - CHMAX: Maximum Channels - numerical variable measured in units. The largest number of paths for data transfer the CPU can use.
   - PRP: Published Relative Performance - the target variable that we aim to predict.
   - ERP: Estimated Relative Performance - a prediction on the target variable that was provided by the authors of the article.<br><br>
3. Project Structure and Methodology <br><br>
   - Imported dataset using the API of UCI.
   - Using metadata, checked which dataframe/dictionary contained comprehensive information.
   - Performed Exploratory Data Analysis: look at distributions, popularity, correlations.
   - Used statistical visualizations to show correlations between CPU features, and differences in Vendor performance.
   - Made a custom statistical function to better understand the characteristics of the distributions of each numerical feature, such as skewness.
   - Built multiple machine learning predictive models: Ridge regression, Lasso Regression, Decision Trees, Random Forests.
   - Enhanced the predictive ability of the best performing model.
   - Finally, the overall best performing model was selected after comparing the R^2 values of all created models. <br><br>
4. Future Work <br><br>
   - Encode the 0th col (Vendor Names) - ordinal (label) or one-hot based on better performance.
   - Use this Encoded feature as a predictor, as the manufacturer may have a statistically signigicant influence on the prediction of Relative Performance.
   - Obtain current data (mid-2020s) for CPU performance metrics from current prominent CPU manufacturers.
   - Repeat CPU performance investigation using that current data. Comment on comparisons, similarities, differences between the 1980s and 2020s.
   - Display feature weights and elaborate on this; can be visualized.
   - Elaborate on the R^2 value illustrating that our model explains __ percent of the variability found in the dataset.
   - Compare my model's MAE, MSE, RMSE with those of the article's authors' ERP predictions. Visualize these comparisons. <br><br>
