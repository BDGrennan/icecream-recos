# **Business Fundamentals Project Write-up**
## **Ice Cream Flavor Recommendations**
#### *by William Grennan*


## Abstract
The primary goal of this project is to create a simple recommendation engine to help people find a flavor of ice cream they would enjoy. The model is built off four product review datasets from major ice cream manufacturers, leveraging the out-of-5 star rating provided. Included is an interactive Tableau dashboard that will recommend a flavor to try based on simple preference selections.


## Design
This project model utilizes the 5 star system to generate an Net Promoter Score (NPS) for each flavor. A rating between 1 and 3 is a negative "detractor" reviewer, a score of 4 is a "passive" reviewer, and a perfect 5 star rating is a "promoter". These scores are averaged across all the reviews of a product to give the final rating. In the Tableau dashboard, a user can specify whether they want the ice cream flavor to include nuts or not. Additionally, they can choose if they prefer a chocolate flavor, or an alternative. The recommender can return up to 15 different flavors ranked by their NPS, but it is limited to flavors with a minimum of 10 reviews.

## Data
Data for the project was obtained from Kaggle as a pre-scraped dataset. The data includes 241 flavors from Ben and Jerry’s, Häagen-Dazs, Breyers, and Talenti. Included is an ingredient list; which is parsed to see if chocolate or nuts are included, and an out-of-5 star rating given by reviewers. 

The data also includes 21,674 individual reviews for those flavors. The review data includes an author, which allows us to track a reviewers likes and dislikes and enables further modeling. The review data also includes the out-of-5 star rating that contributes to the rating from product data. 


[Kaggle Ice Cream Data](https://www.kaggle.com/datasets/tysonpo/ice-cream-dataset)

## Algorithms
#### Data Processing
1. NPS was generated from 5 star reviews
1. Authors are tracked and their individual favorite flavor is used to recommend a flavor to the user


## Tools
- Microsoft Excel is used to store data and create new features such as NPS and the chocolate or nuts flags.
- Tableau is used to build the primary recommender and as a visualization tool

## Communications
This work along with the slides and python script has been uploaded to my Github. The working Tableau dashboard is available on Tableau Public [here](https://public.tableau.com/app/profile/william.grennan/viz/EveryonesFavoriteIceCream/Dashboard1)
