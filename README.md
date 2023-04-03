# Thesis
codes and datasets for thesis project


###
Each of the folders in this repository contains the relevant code files and data to replicate all figures and graphs in the thesis paper. To run the code
snippets and reproduce the thesis plots:
1) Clone the repository from Github
2) Install miniconda from https://docs.conda.io/en/latest/miniconda.html
3) Preferebly create a conda virtual environment. Install the required packages using the requirements.txt file in the environment. 
4) Follow these instructions to properly setup Jupyter Notebook using conda environments. 
https://towardsdatascience.com/get-your-conda-environment-to-show-in-jupyter-notebooks-the-easy-way-17010b76e874
https://stackoverflow.com/questions/58068818/how-to-use-jupyter-notebooks-in-a-conda-environment (I used option 3)
5) Navigate to the main folder using the miniconda prompt, and then run jupyter notebook from within the folder. The code and relevant data files will be visible.

###
To create the graphs used in the contextual analysis, you must download and use the software gephi from https://gephi.org/
###
https://drive.google.com/drive/folders/1qHlJvMTXaYPhAIPsUiYDr_zcnu9ukmeq?usp=share_link
The Drive link contains 4 folders.
1) Download the "Raw Data".rar file from the "Tweet Data" folder on the Drive into the "Raw Data" subfolder if you want to begin the thesis workflow from
the beginning. Download the "Cleaned Data".rar file into the "Cleaned Data" subfolder if you want to skip the preprocessing stage.
2) Download the "wv_model.pkl" from the "Sentiment Analysis" folder on the Drive link to create feature vectors for the model training, cross validation 
and testing in the "sentiment analysis" notebook. The "classifier.pkl" file can be downloaded into the main folder for the "running sentiment analysis on
all cleaned tweets" notebook.
3) Extract all the models in the "word2vec models" folder(in the "Contextual Analysis" folder on the Drive) into the "weekly word2vec models" subfolder
to create the networks used for contextual analysis.
4) Download and extract the "word2vec".rar file if you want to train the word2vec model used for the sentiment 
analysis.
###
To reproduce the sentiment analysis section:
1) Download the "wv_model.pkl" into the main folder and run the "sentiment analysis" notebook.
###
To reproduce the institutional settings section:
1) Extract the "owid-covid".rar file in the main folder.
2) Run the createing plots for India's covid preparedness notebook.
###
To reproduce the changepoint analysis section:
1) Download the "national tweet_details.pkl" file from the Drive into the main folder.
2) Run the "descriptive statstics" notebook for the descriptive statstics section and the "changepoint identification" notebook for the changepoint detection
###
To reproduce the contextual analysis section:
1) Download the "weekly word2vec models" folder from the Drive link, and extract the files into the "weekly word2vec models" subfolder.
4) Run the "creating networks for contextual analysis" notebook.
###
If you are running through the entire thesis workflow on your own:
1) Download the "Raw Data" into the "Raw Data" subfolder.
2) Run the "tweets preprocesing" notebook to clean the tweets.
3) Train the word2vec model using the "training word2vec" notebook.
4) Run the "sentiment analysis" notebook to run train, cross validate and test the classifier.
5) Run the "sentiment analysis on all cleaned tweets" notebook to tag all tweets with their sentiment value.
6) Run the "identifying tweets about Muslims" notebook to tag Muslim related tweets and create the dataset for the changepoint detection.
7) Run the "creating corpus of tweets for every week and training word2vec models" notebook to train the word2vec models used in the contextual analysis
section.
9) Follow the steps listed above in the reproducing section to reproduce the respective thesis sections.
###
IMPORTANT: Delete the Notes.txt files from all the subfolders after cloning/downloading the git repo. 
