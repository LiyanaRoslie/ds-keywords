# Table of contents
- [Project overview](#project-overview)
- [Datasets](#datasets)

<div id="project-overview"></div>

## Project overview

` Project_EDA_TopicModelling_Overview.pptx ` contains the summarized version of the exploratory data analysis (EDA) and topic modelling evaluation. Source code for the scraping the articles' contents are divided into **two notebooks** and they are available in ` crawl_tds_part1.ipynb ` and ` crawl_tds_part2.ipynb `. 

After crawling process is completed, the data are sent to ` data_cleaning.ipynb ` notebook before they can be used for EDA or topic modelling. 

Next, the articles contents are analyzed to find some clues regarding the popular data science articles, etc, followed by the analysis for the Data Science job market in the ` eda.ipynb ` notebook. 

Finally topic modelling is done separately for the articles and jobs' listings in ` ML-TopicModelling-Articles.ipynb ` and ` ML-TopicModelling-JobsListings.ipynb ` respectively.

<div id="datasets"></div>

## Datasets

The data science datasets used in this project include those raw data that was retrieved during the scraping process and also data that has been cleaned before using it for EDA and topic modelling.  

All the datasets can be retrieved using the link below:
https://drive.google.com/drive/folders/16V2F0zCvEC2sgFsWtTSWDgYyy66IH4c_?usp=sharing
