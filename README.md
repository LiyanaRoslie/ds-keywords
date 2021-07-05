# Table of contents
- [Objective](#objective)
- [Project overview](#project-overview)
- [Datasets](#datasets)
- [Libraries used](#libraries-used)
- [Data preprocessing](#data-preprocessing)

<div id="objective"></div>

## Objective

Find what topics or keywords or domains that are relevant and important in the Data Science industry that could help someone to navigate their career in data science industry.

<div id="project-overview"></div>

## Project overview

` Project_EDA_TopicModelling_Overview.pptx ` contains the summarized version of the exploratory data analysis (EDA) and topic modelling evaluation. Source code for the scraping the articles' contents are divided into **two notebooks** and they are available in ` crawl_tds_part1.ipynb ` and ` crawl_tds_part2.ipynb `. 

After crawling process is completed, the data are sent to ` data_cleaning.ipynb ` notebook before they can be used for EDA or topic modelling. 

Next, the articles contents are analyzed to find some clues regarding the popular data science articles, etc, followed by the analysis for the Data Science job market in the ` eda.ipynb ` notebook. 

Finally topic modelling is done separately for the articles and jobs' listings in ` ML-TopicModelling-Articles.ipynb ` and ` ML-TopicModelling-JobsListings.ipynb ` in their respective Jupyter notebooks.

<div id="datasets"></div>

## Datasets

The data science datasets used in this project include those raw data that was retrieved during the scraping process and also data that has been cleaned before using it for EDA and topic modelling.  

All the datasets can be retrieved using the link below:
https://drive.google.com/drive/folders/16V2F0zCvEC2sgFsWtTSWDgYyy66IH4c_?usp=sharing

<div id="libraries-used"></div>

## Libraries used

Please have the following Python libraries installed to run the Jupyter Notebook
* pandas
* numpy
* requests
* random
* time
* BeautifulSoup
* emoji
* warnings
* seaborn
* wordcloud
* matplotlib
* nltk
* gensim
* pyLDAvis
* pyLDAvis.gensim_models

<div id="data-preprocessing"></div>

## Data preprocessing
Text data has to be cleaned before doing any EDA. The cleaned text data has to be transformed before doing topic modelling.

There are the methods employed to clean the text data:
* remove punctuation
* remove escape characters
* remove special characters
* remove duplicated data
* define stopwords for articles' contents and jobs' listings separately. Stopwords are frequently used words or holds not much meaning so they have to be removed.
* make all data to be in lowercase
* remove articles with missing content
* remove authors' names in articles
* remove reading time summary in articles' contents
* remove company name in jobs' listings
* extract company name in company column before “\n” appears

The methods below are employed to transform text data to fit for topic modelling:
* lemmatization - change words to noun
* stemming - reduce words to root form
* convert into list of tokens which are further transformed into ` bag-of-words ` and ` TF-IDF ` models
