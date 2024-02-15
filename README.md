# Yelp-Review-Analysis

## Description:
This project utilizes PySpark, a powerful framework for large-scale data processing, to analyze Yelp restaurant reviews and predict restaurant ratings based on various features. The dataset contains a vast amount of information about restaurants, including reviews, ratings, locations, and more.

## Objective:
The primary objective of this project is to develop a predictive model that can accurately predict restaurant ratings based on the textual content of reviews and other relevant features. By leveraging PySpark's distributed computing capabilities, we aim to efficiently handle large volumes of data and extract valuable insights to enhance decision-making processes for restaurant owners and potential customers.

## Key Features:

Data Preprocessing: The dataset undergoes extensive preprocessing to clean and transform the data into a suitable format for analysis. This includes handling missing values, text normalization, tokenization, and more.

Feature Engineering: We extract relevant features from the dataset, such as review text, restaurant location, sentiment analysis scores, and other metadata, to build a comprehensive feature set for model training.

Model Training: PySpark's machine learning library is employed to train predictive models, such as regression or classification algorithms, to predict restaurant ratings. Various models are explored and evaluated to identify the most accurate one.

Evaluation and Validation: The trained models are evaluated using appropriate performance metrics to assess their accuracy and effectiveness in predicting restaurant ratings. Cross-validation techniques may be employed to ensure robustness and generalization of the models.

Deployment: Once a satisfactory model is developed, it can be deployed to predict restaurant ratings in real-time or batch processing scenarios. This can be achieved using PySpark's deployment capabilities or integrating the model into other applications or platforms.

The Yelp dataset is downloaded from Kaggle website. In total, there are 5,200,000 user reviews, information on 174,000 business. we will focus on two tables which are business table and review table. Attributes of business table are as following:

* business_id: ID of the business 
* name: name of the business
* neighborhood 
* address: address of the business
* city: city of the business
* state: state of the business
* postal_code: postal code of the business
* latitude: latitude of the business
* longitude: longitude of the business
* stars: average rating of the business
* review_count: number of reviews received
* is_open: 1 if the business is open, 0 therwise
* categories: multiple categories of the business

Attribues of review table are as following:
* review_id: ID of the review
* user_id: ID of the user
* business_id: ID of the business
* stars: ratings of the business
* date: review date
* text: review from the user
* useful: number of users who vote a review as usefull
* funny: number of users who vote a review as funny
* cool: number of users who vote a review as cool
