# Songs-Popularity-Predictions
Access the Spotify Past Decades Songs Attributes datasets at: https://www.kaggle.com/cnic92/spotify-past-decades-songs-50s10s

# Datasets Description 
There are a total of 7 datasets available, each containing a set of attributes describing Spotify's most popular songs from a decade between 1950 and 2010. A popularity score is assigned to each song. The number of entries adds up 667 after combining all datasets. 

# Analysis
I have demonstrated how to utilize Python packages (e.g. pandas, NumPy, Seaborn, Matplotlib, and sci-kit-learn) to handle missing values, prepare dataset for modelling, and train and evaluate multiple regression models.  

To facillitate comparison with different regression models, I have kept all sections with codes and results in one notebook. 

# Sections 

**1.	Data cleaning and investigation**
- Aftering merging the 7 datasets, 5 rows with null values are removed. Alternative approach to handling missing values are discussed in the notebook.
- Columns with sparse features that do not contribute to model learning are removed from the dataset. Models trained with sparse features are prone to overfitting as sparse features introduce noises to the dataset, causing the model to fit the noises during training. 
- Data preparation with encoding categorical variables.

	
**2.	Pearson's Correlation**
-  Heatmap of Pearson's Correlation is created to illustrate the strength of relationship between the numerical independent variables and response variable. The results help identify variables that are likely to be good predictors.


**3.	Regression Models**
- Visualizations are created to efficiently present the performance of the following models during training and testing with hyperparameter tuning. The model evaluation metric chosen is Root Mean Square Error (RMSE).

   - Decision tree regressor
   - Random forest regressor 
   - Gradient boosting regressor
