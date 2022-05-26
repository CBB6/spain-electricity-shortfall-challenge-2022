# SPAIN-ELECTRICITY SHORTFALL TEAM CBB6
* In this project we are going to create a project model that is capable of accurately predicting the energy shortfall


# AUTHORS
* CBB6
    * Thulani Nyama(project manager, coordinator)
    * Tumishang Monkoe (project manager,content creator)
    * Ntsikelelo Ngcai (github manager)
    * Pamela Bokaba (scribe)
    * Mike Ngwenya(researcher)
    * Lungelo Ndlovu
# TABLE OF CONTENTS
   * PROBLEM STATEMENT
   * PROBLEM LANDSCAPE
   * TOOLS
   * EXPLORATORY DATA ANALYSES
   * DATA ENGINEERING
   * MODELLING
   * MODEL PERFORMANCE
   * MODEL EXPLAINATION
   * API
   * PRESENTATION

# PROBLEM STATEMENT
 * Spain has a daily energy shortfall,there is a requirement to identify patterns in the energy shortfall data to create a regression model that can accurately predict    energy shortfall.
 
# PROBLEM LANDSCAPE 
   * A regression model that is created for the issue in Spain’s energy shortfalls, is identifying patterns and predicting shortfalls, to inform the residents of Spain       when to expect electricity shortfalls.
 

# TOOLS
* Trello
  * used for setting goals for the project
  * monitoring the progress of the team with Trello boards
  *used to assign team members
  *manage the project
  * sign up to Trello follow the link https://trello.com/signup 
  * GITHUB.com
  * Used for documenting the project on README.md / WIKI
  *The project and to create repositories
  *Used to collaborate
  * sign up for Github to start colllaborating folllow the link  https://r.search.yahoo.com/_ylt=A0geK.LtfY9i7qwAtZ9XNyoA;_ylu=Y29sbwNiZjEEcG9zAzEEdnRpZAMyNDI4MlVTLUNfMQRzZWMDc3I-/RV=2/RE=1653599854/RO=10/RU=https%3a%2f%2fgithub.com%2fsignup/RK=2/RS=1swEjw0QOx81.Fx6D5hPDjF3zyM-
*  JUPYTER NOTEBOOK
* Loading Python
* Import Python libraries
* You can also log on to jupyter follow the link https://jupyter.org/
     
*  KAGGLE
    * evaluate the accuracy of the best machine learning model
    * access the largest datascience community 	https://r.search.yahoo.com/_ylt=A0geKIzVf49iP.YAsRFXNyoA;_ylu=Y29sbwNiZjEEcG9zAzIEdnRpZAMyNDI4MlVTLUNfMQRzZWMDc3I-/RV=2/RE=1653600341/RO=10/RU=https%3a%2f%2fwww.kaggle.com%2f/RK=2/RS=.5YVEy61t0tS6wDTJDFL_bEhrzc-
* AWS-cloud computing
	* create an account with AWS https://r.search.yahoo.com/_ylt=AwrJ7FkTgY9iBN4A9SlXNyoA;_ylu=Y29sbwNiZjEEcG9zAzEEdnRpZAMyNDI4MlVTLUNfMQRzZWMDc3I-/RV=2/RE=1653600659/RO=10/RU=https%3a%2f%2faws.amazon.com%2fresources%2fcreate-account%2f/RK=2/RS=SVaLjEmsWC5s9MUgsWrDCaJ3kYk-


*  INSTALLATIONS
     * Python libraries
* LOADING THE DATA
   * loading the train data on jupyter notebook - https://github.com/CBB6/spain-electricity-shortfall-challenge-2022/blob/main/df_train.csv
   * loading the test data on jupiter notebook - https://github.com/CBB6/spain-electricity-shortfall-challenge-2022/blob/main/df_test.csv
# EXPLORATORY DATA ANAYSIS(EDA)
   * DATA STATISTICS  (In-depth analysis of all the variables in the DataFrame)
      * Checked the first rows of the DataFrame (df)
      * Droped empty rows
      * Showed the number of columns/rows in the train dataframe
      * RangeIndex: 8763 entries, 0 to 8762
	       Data columns (total 48 columns)
       * Checked the dataframe information of data type, count null values of columns
       *  Viewed basic statistical details, 
	        count	mean	std	min	Q1	Q2	Q3	max

       * Checked for outliers in different columns
	      df_train.kurtosis()
	    * We made use of kurtosis to analyze outliers in each column. 
	    * We plotted a figure that shows columns with outliers
	    * using the skew() function  we checked for the skewness of the data over the column axis
       * Plotted relevant features
	    * Seaborn boxplot to summarize the data into a visual 'Valencia_wind_speed'
	    * Seaborn bar plot   xlabel='Valencia_wind_deg', ylabel='load_shortfall_3h
       * matplotlib.pyplot histogram for the 'load_shortfall_3h
	    * Plotted correlation heat map for predictor variable in train
	    * plotted distributions of all the features in train
       * Checked for missing values in training data
       * plotted the percentage of  missing values in train data set
# DATA ENGINEERING
   * Checked the mode from both data sets to replace missing values with
   * Removed missing values/ features replace with 0
   * Imputed Categorical features using OrdinalEncoder()
   * Transformed Features such as Time, Year, month, day and created a new feature ‘start hour’ 
   * Scaled the train dataset 
   * Added load_short_fall_3h as last column on training data
   * 

# MODELLING
   * Split dataset X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3332, random_state=42
   * Checked the shape of the training and testing data
   * Created a decision_tree model
   * DecisionTreeRegressor(max_depth=100, random_state=42)
   * NNR.MLPRegressor model(random_state=42)
   * Bagging_annt_regressor (base_estimator=annt)
   * Ensembled model with Baggin
   * Ensembled model with AdaBost
   * Trained Bagging ensemble models
   * Trained AdaBoost ensemble models
   * Bagging ensembled predictions
   * AdaBoosted predictions
   * Evaluated models
	
	
# MODEL PERFORMANCE
   * Compared model performance 
   * Tested RMSE
   *  Decision Tree Model Ensembled with Bagging   3503.378937
       Neural Network Model Ensembled with Bagging  5841.772288
                                               Test RMSE
       Neural Network Model Ensembled with Bagging  5504.771821



# MODEL EXPLAINATION
   * The model with the best RMSE is regression  trees, it is a predictive model
   * Decision trees takes consideration of each possible outcome
   * Decision trees is used to predict continuous outputs, our electricity shortfall will be continuous  outputs this makes it an ideal model to use                                    
	        
 	


	


	
	
 


