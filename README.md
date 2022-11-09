# CS6471_HateSpeechAnalysis
Course Project for CS 6471 : Computational Social Science. Project Title: Implicit and Explicit Hate Speech : An Empirical Analysis

Extension to work - ElSherief et al. (2021), "Latent Hatred: A Benchmark for Understanding Implicit Hate Speech" https://arxiv.org/abs/2109.05322

## Directory Structure - 

* Code : Contains the directory for the following python notebooks,
  * CSS_Data_Scraping.ipynb : Data scrapping and generation of word graphs for subreddits mentioned in the report.
  * CSS_Sentiment_Score.ipynb : Use of VADER for calculating sentiment score and analyse against the three hate categories.
  * FINAL_PRESENTATION_Copy_of_CSS_Project_Spring_2022.ipynb : Main notebook with the code to train the 2 way and 3 way classifier using latent hatred dataset.
          
* Data : This folder contains datasets that we used,
  * Training Dataset : 
    * implicit_explicit_nothate_classification.csv (3-way)
    * implicit_nothate_binary_full.csv (2-way)
  * Subsampled Training dataset : 
    * implicit_explicit_nothate_balanced.csv (3-way)
    * implicit_nothate_balanced.csv (2-way)
  * YoutubeReddit : Cross-Domain dataset for qualitative analysis.
  * SubReddit : Datasets collected for temporal analysis using PushShift API.
  
  Link to dataset - https://drive.google.com/drive/folders/1-Mq9Z0VRktgJlBkehEUCVthnxKy2obGU?usp=share_link


## Steps to RUN the code -

1. Paste the Data Folder in the google drive to be connected to the notebook.
2. Ensure the paths are in sync as mentioned in the notebook.
3. Notebook requires GPUs for faster performance. (can work without GPUs though)
4. To generate the models used for 3 way classifier, run the following cells in order -
    1. IMPORT STATEMENT
    2. DATA IMPORT
    3. FUNCTIONS
    4. Load Dataset
    5. Model - 3 labels balanced and tuned
5. To generate the models used for 2 way classifier, run the following cells in order -
    1. IMPORT STATEMENT
    2. DATA IMPORT
    3. FUNCTIONS
    4. Load Dataset
    5. Model Train and Test and Tune - 2 labels
6. To generate the annotations and results shared in the report, run the following cells in order-
    1. IMPORT STATEMENT
    2. DATA IMPORT
    3. FUNCTIONS
    4. Europe
    5. Politics
    6. Champions League
    7. ETHOS


