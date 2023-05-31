# Prediction-of-Stock-Log-Returns-using-Deep-Neural-Network

README Prediction of Stock Log Returns using DNN

This README explains how to recreate the results in the jupytor notebooks. All files needed for results are in the zip.

For data manipulation, open "Data creation and manipulation.ipynb". This notebook can not actually run, since the datasets needed are too large. One can still get a good idea as to how we create the dataset. Additionally, we included the Keras RNN model in the bottom of the notebook.


For the main portfolio results, open "Prediction of Stock Log Returns.ipynb":

1. Read in the optimal_df for either 2005-2011 , 2012-2018 , 2019-2022. These files can be loaded by the use of the pickle library. An example of this could be:
		
		optimal_df = pickle.load( open( "optimal_df_05_11.p", "rb" ) )

2. When the optimal_df is loaded, please run the cell which loads in the Nasdaq100 data using the "NASDAQ100_index.csv" file.

2. The optimal_df is a dataframe containing the stock predictions for that given month, including the optimal hyperparameters. This dataframe can be viewed by simple pandas commands.

3. Run the functions: optimal_hyper, select_stocks,make_pf. When this is done it is possible to use the function optimal_hyper, which calculates all the portfolio results which are described in the thesis. 

4. Tables from thesis can also be created by running the cell for these tables.

5. It is now possible to run the plots.

6. Loss plots can also be plottet within these periods.
