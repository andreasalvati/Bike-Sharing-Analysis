# Bike sharing analysis with Dask

The objective is to rewrite the Bike Sharing analysis done in the Python for Statistical Programming subject using Dask data structures and ecosystem instead of plain pandas.

## Analysis Goals

* Creation of a git repository with a proper README, incremental commits, and some sort of automatic or programmatic download of the data before the analysis
* Use of dask.dataframe and distributed.Client for all the data manipulation 
* Use of Dask-ML for distributed training and model selection

## Project Details

* **Task**: predict the bike sharing usage
* **Training data**: whole 2011 and first 3 quarters of 2012.
* **Test data**: 4th quarter of 2012.  Do not fit your models with these data! They should just be used to see how good/bad your model predictions are.
* **Error metric**: R2 score (scikit-learn's default for regression).
* **Running Time**: 00:10:11

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
