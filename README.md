#   Airbnb-Host-Assistant
_____
![Airbnb](http://www.oliverandsons.com/wp-content/uploads/2014/08/Untitled-design-10.png)

# Table of contents
1. [Introduction](#Introduction)
2. [Goal](#paragraph1)
3. [Text-Processing](#paragraph2)
4. [Topic Modeling](#paragraph2)
5. [Supervised Learning Modeling](#paragraph2)

## Introduction
This project is about helping Airbnb host to estimate revenue for their listing based on the description of the listing. As you already know when booking a house on Airbnb what are the things you look at in the listing. We look at images of the house, listing price and read the description.

## Goal
While these are key elements of the listing. This project focuses on evaluating the list descriptionalong with few categorical values like roomtype,housetype to estimate revenue a host can make.

## DataSet
[Kaggle:facebook-recruiting-iv-human-or-bot/data](https://www.kaggle.com/c/facebook-recruiting-iv-human-or-bot/data)
I use the dataset provided by Inside Airbnb, where publicly available information about a city’s Airbnb’s listings have been scraped and released for independent, non-commercial use. This includes detailed listing information such as no. of rooms, location, text description, price.
I am foscusing on San Francisco city in United States so I used the detailed listings information for SF listings active from December 2017 to December 2018. After data cleaning, the dataset has 9722 rows and 16 columns.

## Text Processing
I  have a processed dataset and an understanding of what we are trying to predict, I focus on converting the description text into useful features for the machine learning model.
To reduce the number of terms and focus on the most important per document, non-english and stop words are removed. Words are also lemmatised and a RegEx tokeniser is used to ignore non-alphanumeric strings. The remaining words are then converted into a bag-of-words representation (a list of word_id, word_frequency 2-tuples) for the Document-Term-Matrix.
## Topic Modeling
1. Latent Dirichlet Allocation (LDA
2. Latent Semantic Analysis
3. Non-negative Matrix Factorization 

## Training Machine Learning Models 
1. Linear Regression
2. Decison Tree
3. Random Forest

## Score Table
| Model       | R2 Score        | RMSE  |
| ------------- |:-------------:| -----:|
| Logistic Regression    | 0.33 | 53167.27030 |
| Decision Tree      | 0.18      |   58631.09619 |
| Random Forest | are neat      |    $1 |

```


