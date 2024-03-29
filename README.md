# Module 5 Project: Qualities of A Higher-Rated App
## Overview
This project was for The Flatiron School, Inc.'s Data Science bootcamp, and was put together by Bronwen C.
The dataset was information on strategy game apps provided by a Kaggle user. The analysis found 11 important features that account for whether an app has a higher rating or a lower rating.
A higher-rated app was defined as having an average user rating of 4.5 or higher and a lower-rated app was defined as having an average rating of 4 or under.
The apps' average ratings were provided at halves, so there are no apps in the dataset with an average rating between 4 and 4.5.

I wrote a [blog post](https://bronwencc.github.io/a_higher_rated_strategy_game_app) that goes into more detail about this project. [Another blog post](https://bronwencc.github.io/two_experiences_with_feature_engineering_using_pandas) goes into more detail specifically about engineering a feature I did not end up using.

### 5 significant features with highest importance:
* The number of ratings: Apps with more ratings had higher average user ratings
* Whether the app has a Subtitle: Apps with a Subtitle had higher average user ratings
* The size of the application: Larger apps had higher average user ratings
* The length of Description text: Apps with a longer Description had higher average user ratings
* Whether the application is in the Simulation genre: More apps in the simulation genre than not in that genre had lower average user ratings

## Repository contains folders and files:

* 17k-apple-app-store-strategy-games.zip is a compressed file of the [dataset from Kaggle](https://www.kaggle.com/tristan581/17k-apple-app-store-strategy-games), created by Kaggle user Tristan

* appstore-games.csv is the unzipped file of the original dataset

* [final.ipynb](https://github.com/bronwencc/Module-5-Project/blob/master/final.ipynb) is a Jupyter notebook containing all the code for this project: analyzing the dataset, creating a model, and plotting information

* [LICENSE.md](https://github.com/bronwencc/Module-5-Project/blob/master/LICENSE.md) is the license detailing under what circumstances the code and its derivatives, and the files contained in this repository may be used

* [presentation.pdf](https://github.com/bronwencc/Module-5-Project/blob/master/presentation.pdf) is a PDF for a business audience presenting the results, recommendations and future ideas

### The [files folder](https://github.com/bronwencc/Module-5-Project/tree/master/files/) contains CSV files saved from various points of working on the project:

* binsiap7464.csv is the data from the In-app Purchases feature sorted based on whether the record has one or more in-app purchases falling into one of six bins, except if there are no in-app purchases or only those that cost 0, they have a 1 in iapb_none and 0 in all other columns
* iap7464.csv is similar to above, except without bins, for every price in In-app Purchases
* final7464.csv contains 15 important features and the Target, all int or float variables
* finalbins7464.csv similarly contains 15 important features, except they were determined with the binned version of In-app Purchases
* temp7464.csv contains the dataset with all relevant numerical features, creating dummy columns or simple counts of characters from an original text column
* tempbins7464.csv similarly contains all numerical versions of features, except with bins for the In-app Purchases column

### The [images folder](https://github.com/bronwencc/Module-5-Project/tree/master/images/) contains plots of various features as .PNG files:

* Several display percentages of binary categorical features comparing the records that have the feature to those without by looking at stacked bar chart percentages of whether they have the target variable or not (1 for Average User Ratings 4.5 or 5, 0 for Average User Ratings 4 and under)

* Two plots are scatter plots looking at continuous features compared to Average User Rating (the latter on a scale from 1 to 5). One of them is of app size:

![Scatter plot of App Size (in Gibibytes) compared to Average User Rating with most points being small app size at all ratings; no app rated 2 or lower has size larger than ~0.5 GiB; with sparse scattering for sizes larger than ~2.5 GiB, all of those have 3.5 rating or higher](https://raw.githubusercontent.com/bronwencc/Module-5-Project/master/images/Distribution%20of%20Size.png)

* One image is two box plots comparing the length of the Description text in number of characters for higher- and lower-rated records:

![Pair of box plots without outliers showing higher-rated apps have higher values for the median, the third quartile and the upper extreme](https://raw.githubusercontent.com/bronwencc/Module-5-Project/master/images/Description%20Box-Plots.png)
