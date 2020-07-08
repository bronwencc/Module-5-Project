This repository contains two folders (files and images) along with several files:

17k-apple-app-store-strategy-games.zip is a compressed file of the dataset from https://www.kaggle.com/tristan581/17k-apple-app-store-strategy-games, created by Kaggle user Tristan

appstore-games.csv is the unzipped file of the original dataset

final-draft.ipynb is a Jupyter notebook containing all the code for this project: analyzing the dataset, creating a model, and plotting information

LICENSE.md is the license detailing under what circumstances the code and its derivatives, and the files contained in this repository may be used

README.md is this file explaining the contents of this repository

presentation.pdf is a PDF for a business audience presenting the results, recommendations and future ideas

files contains CSV files saved from various points of working on the project:

binsiap7464.csv is the data from the In-app Purchases feature sorted based on whether the record has one or more in-app purchases falling into one of six bins, except if there are no in-app purchases or only those that cost 0, they have a 1 in iapb_none and 0 in all other columns

iap7464.csv is similar, except without bins, for every price in In-app Purchases

final7464.csv contains 15 important features and the Target, all int or float variables
finalbins7464.csv similarly contains 15 important features, except they were determined with the binned version of In-app Purchases

temp7464.csv contains the dataset with all relevant numerical features, creating dummy columns or simple counts of characters from an original text column

tempbins7464.csv similarly contains all numerical versions of features, except with bins for the In-app Purchases column

images contains plots of various features as .PNG files:

Several display percentages of binary categorical features comparing the records that have the feature to those without by looking at stacked bar chart percentages of whether they have the target variable or not (1 for Average User Ratings 4.5 or 5, 0 for Average User Ratings 4 and under)

two plots are scatter plots looking at continuous features compared to Average User Rating (the latter on a scale from 1 to 5)

one plot is a box plot comparing the length of the Description text for higher- and lower-rated records