# Weekly Market Direction Prediction

## Overview
This project involves the analysis of weekly market data with the goal of predicting market direction ('Up' or 'Down'). The data spans from 1990 to 2010 and includes various lag variables, volume, and the direction of the market.

## Data Description
The dataset contains the following columns:
- **Year**: The year of the observation.
- **Lag1** to **Lag5**: The percentage returns for each of the five previous weeks.
- **Volume**: The number of shares traded (in billions).
- **Today**: The percentage return for this week.
- **Direction**: The direction of the market movement, either 'Up' or 'Down'.

## Objective
The primary objective is to build models that can predict the weekly direction of the market ('Up' or 'Down') using various statistical and machine learning techniques.

## Methodology
We employed several methods to achieve our objective:
1. **Logistic Regression**
2. **Linear Discriminant Analysis (LDA)**
3. **Quadratic Discriminant Analysis (QDA)**
4. **K-Nearest Neighbors (KNN) with k=1**

The models were trained using the data from 1990 to 2008 and tested on the held-out data from 2009 and 2010.

## Results
The performance of the models was evaluated based on the accuracy and the confusion matrix. The key findings are:

- **Logistic Regression and LDA** both achieved the highest accuracy of **62.50%**.
- **QDA** showed a lower accuracy of **58.65%**, with a tendency to predict 'Up' movements.
- **KNN (k=1)** had the lowest accuracy of **49.04%**, indicating less effectiveness in this scenario.

## Conclusion
Linear Discriminant Analysis (LDA) appears to provide the best results on this data, closely followed by logistic regression. Both QDA and KNN (k=1) showed lower effectiveness. The modest accuracy of the best models suggests that predicting market direction might be inherently challenging with the given variables, or additional predictors and more complex models might be necessary for improved performance.

## Future Work
Further analysis could explore:
- The inclusion of additional predictors.
- More complex models or ensemble techniques.
- A deeper analysis of market conditions and external factors that might influence the market direction.
