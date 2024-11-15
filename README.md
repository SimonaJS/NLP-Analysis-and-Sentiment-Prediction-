# Customer Sentiment Analysis for Hospitality Insights Group

## Overview
This repository contains the code and resources for a natural language processing (NLP)-driven sentiment analysis project. The project is designed to predict customer satisfaction from hotel reviews by leveraging machine learning techniques. By identifying key factors influencing customer sentiment, this project enables Hospitality Insights Group to better understand guest feedback and implement data-driven improvements.

## Problem Statement
In the competitive hospitality industry, understanding guest sentiment is crucial for enhancing service quality and improving customer experience. Manual review analysis is impractical for large datasets, leading to potential missed insights. This project addresses this challenge by developing a predictive model that analyzes guest reviews, classifying them as positive or negative, and identifying the main factors driving satisfaction.

## Impact
This project aims to:
- **Enhance Customer Experience**: By identifying sentiment drivers, hotel managers can make targeted improvements.
- **Enable Informed Decision-Making**: The model supports data-driven strategies based on customer feedback.
- **Streamline Feedback Processing**: Automating sentiment analysis reduces time and resources required to analyze guest feedback.

## Dataset
The dataset includes structured and unstructured data from Hospitality Insights Group, consisting of review text, stay details, and a `reviewer_score` target variable indicating overall sentiment (1 for positive, 0 for negative). This dataset enables the development of models that capture nuanced sentiment patterns across different aspects of the guest experience.

### Data Dictionary
| Variable Name                                 | Description                                                                                   |
|-----------------------------------------------|-----------------------------------------------------------------------------------------------|
| `additional_number_of_scoring`                | The number of additional scores given for the hotel.                                          |
| `average_score`                               | The average score of the hotel based on reviews.                                              |
| `days_since_review`                           | The number of days since the review was posted.                                               |
| `day`                                         | Day of the review.                                                                            |
| `hotel_address_amsterdam`                     | Binary variable indicating if the hotel is located in Amsterdam.                              |
| `hotel_address_barcelona`                     | Binary variable indicating if the hotel is located in Barcelona.                              |
| `hotel_address_london`                        | Binary variable indicating if the hotel is located in London.                                 |
| `hotel_address_milan`                         | Binary variable indicating if the hotel is located in Milan.                                  |
| `hotel_address_paris`                         | Binary variable indicating if the hotel is located in Paris.                                  |
| `hotel_address_vienna`                        | Binary variable indicating if the hotel is located in Vienna.                                 |
| `latitude`                                    | Latitude coordinate of the hotel's location.                                                  |
| `leisure_trip`                                | Binary variable indicating if the trip was for leisure or not.                                |
| `longitude`                                   | Longitude coordinate of the hotel's location.                                                 |
| `month`                                       | Month of the review.                                                                          |
| `negative_review`                             | Textual field containing negative comments from the reviewer.                                 |
| `nights_stayed`                               | The number of nights the reviewer stayed at the hotel.                                        |
| `positive_review`                             | Textual field containing positive comments from the reviewer.                                 |
| `review_total_negative_word_counts`           | Total count of negative words in the negative review.                                         |
| `review_total_positive_word_counts`           | Total count of positive words in the positive review.                                         |
| `reviewer_nationality_australia`              | Binary variable indicating if the reviewer is from Australia.                                 |
| `reviewer_nationality_ireland`                | Binary variable indicating if the reviewer is from Ireland.                                   |
| `reviewer_nationality_other`                  | Binary variable indicating if the reviewer is from a nationality other than the specified ones.|
| `reviewer_nationality_uae`                    | Binary variable indicating if the reviewer is from the UAE (United Arab Emirates).            |
| `reviewer_nationality_uk`                     | Binary variable indicating if the reviewer is from the UK (United Kingdom).                   |
| `reviewer_nationality_usa`                    | Binary variable indicating if the reviewer is from the USA (United States of America).        |
| `reviewer_score`                              | The score given by the reviewer, where positive sentiment is encoded as 1 and negative as 0.  |
| `total_number_of_reviews`                     | The total number of reviews for the hotel.                                                    |
| `total_number_of_reviews_reviewer_has_given`  | The total number of reviews the reviewer has given.                                           |
| `year`                                        | Year of the review.                                                                           |

## Exploratory Data Analysis (EDA)
The EDA process included analyzing patterns and distributions within the dataset to identify key trends related to guest sentiment. Techniques included:
- **Descriptive Statistics**: Summarized numerical and categorical features.
- **Geospatial Analysis**: Examined location-based trends in sentiment.
- **Correlation and Multicollinearity Checks**: Used statistical metrics to assess feature relationships and redundancies.
- **Sentiment Analysis**: Preprocessed and extracted n-gram and TF-IDF features for enhanced text representation.

## Predictive Modeling
The project used various machine learning models to predict reviewer sentiment, including logistic regression, decision trees, random forests, and gradient boosting models. Feature selection and dimensionality reduction were applied to enhance model performance and interpretability.

### Key Models
- **Logistic Regression Models**: Baseline, N-gram (1,3), and TF-IDF variants were used for sentiment prediction.
- **Tree-Based Models**: Decision trees and random forests provided insights into feature importance and model robustness.
- **Gradient Boosting**: Achieved the highest accuracy, identifying crucial sentiment-related features.

## Key Findings and Recommendations
### Positive Sentiment Drivers
- **Location and Accessibility**: Terms related to convenience and location quality emerged as major contributors to positive reviews.
- **Room Comfort and Amenities**: Features related to bedding and room quality influenced positive sentiment significantly.
- **Service Quality**: High scores were associated with positive service experiences.

### Negative Sentiment Drivers
- **Service Gaps**: Common complaints centered on inconsistent service quality.
- **Value for Money**: Terms related to pricing and amenities indicated that guests' value perceptions are crucial.
- **Comfort Issues**: Negative reviews often referenced room quality issues.

### Recommendations
- Enhance service quality across locations.
- Emphasize convenience and amenities in marketing materials.
- Regularly review pricing strategies and align them with service quality.

## Future Work
To further develop this project, consider:
- **Scaling for Larger Datasets**: Enhance model performance for large datasets.
- **Advanced NLP Techniques**: Integrate models like BERT for improved text analysis.
- **Demographic Segmentation**: Tailor sentiment analysis by guest demographics for targeted insights.

## Usage
1. **Clone the Repository**: Clone this repository to your local machine.
2. **Install Dependencies**: Use `requirements.txt` to install necessary libraries.
3. **Explore Jupyter Notebooks**: The notebooks in the `notebooks` folder contain EDA and modeling steps.
4. **Run Scripts**: The `scripts` directory contains code for data processing and model training.

## License
This project is licensed under the MIT License.
---
