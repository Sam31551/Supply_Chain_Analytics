

# Sentiment Analysis of Ben & Jerry's Ice Cream Reviews

This project performs a sentiment analysis of Ben & Jerry's ice cream reviews to understand the relationship between user-provided star ratings and sentiment scores derived from review texts. The goal is to assess how well sentiment aligns with star ratings and identify products that might require attention.

## Dataset Overview

The analysis uses two primary datasets:

### Products Data

The `products.csv` file includes:

- `key`: Unique identifier for the product
- `name`: Name of the product
- `subhead`: Subheading describing the product
- `description`: Detailed description of the product
- `rating`: Average star rating from Ben & Jerry's
- `rating_count`: Number of ratings
- `ingredients`: List of ingredients

### Reviews Data

The `reviews.csv` file includes:

- `key`: Unique identifier matching the product
- `author`: Reviewer’s username
- `date`: Date of the review
- `stars`: Star rating given by the reviewer
- `title`: Title of the review
- `helpful_yes`: Number of people who found the review helpful
- `helpful_no`: Number of people who did not find the review helpful
- `text`: Text content of the review


## Steps and Methodology

1. **Data Preparation**:
   - The data is loaded and cleaned by removing irrelevant columns from the reviews dataset. This prepares the data for sentiment analysis.

2. **Sentiment Analysis**:
   - Sentiment analysis is performed on the text of each review to derive a sentiment score, which indicates the positive or negative tone of the review. This score is added to the reviews dataset.

3. **Rating Analysis**:
   - The average star ratings and sentiment scores are computed for each product. These scores are then normalized to a range of 0 to 1 for consistency.

4. **Comparison and Visualization**:
   - The discrepancy between star ratings and sentiment scores is analyzed. A comparison plot is generated to visualize how star ratings and sentiment scores relate to each other.

5. **Results**:
   - The top and bottom performing products are identified based on their combined star ratings and sentiment scores. This helps in understanding which products are well-received or poorly received by customers.

## Results

### Key Metrics

- **Average Stars Rating vs. Review Text Score**:
  - Reviews with positive sentiment generally have higher star ratings. The average sentiment score for reviews is approximately 0.603.

- **Discrepancy Between Stars and Reviews**:
  - On average, the ratio of star rating to review sentiment is around 1.465. This indicates that users tend to rate products higher in stars compared to their sentiment score from review text.

### Best and Worst Performing Products

- **Top 5 Products**:
  1. Ice Cream Sammie
  2. Cold Brew Caramel
  3. Sweet like Sugar Cookie Dough Core
  4. Glampfire Trail Mix
  5. Americone Dream

- **Bottom 5 Products**:
  1. Chocolate Cookie Dough Core
  2. Coffee Toffee Bar Crunch
  3. Chocolate Fudge Brownie
  4. Red, White & Blueberry
  5. Chillin’ the Roast

## Conclusion

The analysis shows that while higher star ratings are often associated with more positive text reviews, there is a notable discrepancy between star ratings and sentiment scores. This suggests that Ben & Jerry's should consider both star ratings and sentiment analysis of reviews for a more comprehensive evaluation of product performance.

## Recommendations

1. **Product Evaluation**:
   - Combine star ratings with sentiment analysis to better understand customer satisfaction.
   - Address products with low combined scores to improve their market performance.

2. **Product Improvements**:
   - Focus on reformulating or discontinuing products with consistently poor sentiment and star ratings.

3. **Continuous Monitoring**:
   - Regularly update sentiment analysis to keep track of changing customer opinions and adapt strategies accordingly.
