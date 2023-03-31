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
  https://stackoverflow.com/questions/58068818/how-to-use-jupyter-notebooks-in-a-conda-environment
5) Navigate to the folder that you want to run the code of using the miniconda prompt, and then run jupyter notebook from within the folder. The code and relevant data files will be visible.

###
If you want to replicate the entire thesis workflow or train the word2vec models for the sentiment analysis or the weekly ego networks
then you must download the compressed data files from the Google Drive link and save them in the main folder specific to the task you are attempting

###
To create the graphs used in the contextual analysis, you must download and use the software gephi from https://gephi.org/
###
https://drive.google.com/drive/folders/1qHlJvMTXaYPhAIPsUiYDr_zcnu9ukmeq?usp=share_link
The Drive link contains 4 folders.
1) The "word2vec" folder contains the compressed txt file containing all tweets for training the word2vec model. Download and extract it into the "Tweets Preprocessing" folder. Use it to train the word2vec model.
2) The "Tweet Data" folder contains the compressed raw and cleaned tweets. Download and extract them into the "Raw Data" and "Cleaned Data" folders in the "Tweets Preprocessing". Keep in mind if you start the preprocessing from the Raw Data, the output of that will get saved in "Cleaned Data"
3) The "Sentiment Analysis" folder contains the trained word2vec model and the sentiment classifier pipeline. Both can be downloaded into the "Tweets Preprocessing" folder to facilitate the sentiment prediction of all the cleaned tweets. Or the word2vec model can be downloaded into the "Sentiment analysis" folder of the Github repository to run the grid-search CV to train the classifier.
4) The "contextual analysis" folder contains two folders. The first contains the training tweets for each of the weekly word2vec models (these are in the other folder). Use the tweets txt files to train the weekly word2vec models yourself or use the trained models to create the network. 
