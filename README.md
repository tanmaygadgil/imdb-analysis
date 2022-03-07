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
- [Data Imputaion and Feature Engineering](Data%20Imputation%20and%20Feature%20Engineering.ipynb)
- [EDA][EDA.ipynb]
- [Modeling][Modeling.ipynb]
