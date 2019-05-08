# Bike_Sharing_Analysis

Rewrite the Bike Sharing analysis using Dask

(Even if the original analysis was done in group, this should be done individually)

Submission format: A .zip produced by `$ git archive master --format=zip -o LastName_FirstName_Dask.zip` and a link to the GitHub repository, which must be public right after the deadline.

The objective is to rewrite the Bike Sharing analysis done in the Python for Statistical Programming subject using Dask data structures and ecosystem instead of plain pandas.

The reasons for choosing this are:

The dataset is comparatively small, and the extra computing time is given by feature engineeering and model selection, which lowers the risk
Everybody has performed this analysis and is relatively familiar with it, which makes it easier than carrying a data science project from scratch, given the time constraints
Rewriting an existing analysis to make it more performant is more aligned with the objectives of the subject and reflects more real world escenarios
The "business objectives" are more clear than in the group assignment
The maximum score of the assignment is 5 points and the grading will be as follows:

Creation of a git repository with a proper README, incremental commits, and some sort of automatic or programmatic download of the data before the analysis (1 point). Notice that the data should not be checked out in the repository. Including data files in git repositories is considered a bad practice.
Use of dask.dataframe and distributed.Client for all the data manipulation (2 points). Remember that calling .compute() in a Dask DataFrame turns it into a pandas dataframe, which resides in RAM and loses the distributed advantages. The more Dask structures are used, the higher the grade.
Use of Dask-ML for distributed training and model selection https://ml.dask.org/ (1 point). See below for inspiration.
Move parts of the computation to .py scripts that are then imported from the notebook when appropriate and that can be properly installed as seen during the course and in the group assignment (0.5 points)
Use of Dask-Yarn to deploy the analysis in a YARN/Spark/Amazon ElasticMapReduce cluster, and write accompanying documentation to describe the procedure for the deployment https://yarn.dask.org/ (0.5 points). See below for inspiration.
Useful links:

Putting everything in a pipeline https://tomaugspurger.github.io/scalable-ml-01.html
Why Dask-ML is faster than sklearn GridSearchCV for model selection https://jcrist.github.io/introducing-dask-searchcv.html
JupyterHub on Hadoop https://jcrist.github.io/jupyterhub-on-hadoop/index.html
As you can see, the assignment is more open ended. Use this as a opportunity to explore, and don't be afraid of recording failed experiments in the notebook, if they are properly explained and described.
