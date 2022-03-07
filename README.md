# imdb-analysis

## Dataset

This analysis was performed on the IMDB datasets found here: [dataset](https://www.imdb.com/interfaces/)

In this dataset we can find the following tables:

- title.akas.tsv.gz: This table gives us a list of regions that a movie was featured in. The worldwide appeal of a movie can indicate how popular it is and can also correlate with its quality.
- title.basics.tsv.gz: Gives basic information like runtime, number of votes etx. This table will form the basis of our dataset.
- title.crew.tsv.gz: Gives the directors and writers that have worked on a title.
- title.episode.tsv.gz: this table is irrelevant for us since we are only considering movies
- title.principals.tsv.gz: This gives us an ordered list of actors, directors and other crew members who have worked on a film
- title.ratings.tsv.gz: This table maps a titles to its imdb rating.
- name.basics.tsv.gz: Gives the names of actors and some titles that they are known for. This data will be used later for imputation.

## Notebooks

This repository contains the following notebooks

- [Data Sampling](Data%20Imputation%20and%20Feature%20Engineering.ipynb): This notebook features a first look at the data and subsamples the data for the movie and TVMovie categories
- [Data Imputaion and Feature Engineering](Data%20Imputation%20and%20Feature%20Engineering.ipynb): This notebook attemps to impute any missing features and created a new set of features that can be used in the dataset
- [EDA](EDA.ipynb): This performs explorartory analysis on our created dataset. Here we explore the relationship of our features with our target variable 
- [Modeling](Modeling.ipynb): This notebook features data preprocesing, model building and model tuning.

## Key Insights



## Future Scope

Given more time, we can improve and augment this dataset to produce better predictions. These are the few ideas that can be implemented in the future.

### Dataset

- Augment the dataset with external sources like the TMDB dataset. I did use the TMDB dataset for data imputation, but due to its rate limiter for the free tier, I wasn;t able to use it to enrich the entire dataset within the same timeframe.
- We can see that the model's predictions heavily depends on the performance of the cast and crew. Finding a way to better define the perfomrace inex of the cast and the crew may impact the model's predictive power.
- Adding temporal features for the cast and the crew may aid in the model's performace. How well a movie does doesn't necessarily depend only on the cast's and crew's past performances but also on their performance trajectory. Having a feature which encodes this temporal aspect may help in increasing predictive capability.
- Film budgets are also a strong indicator or quality. Finding a way to add in the budget could help imporve the model's predictive performance. This information was available on the TMDB API, but I couldn't incorporate it due to the rate limiting constraints

### Models
- More hyper-parameter tuning to gain better model performance.
- More model analysis to understand which what distribution of features have the lowest predictive power




