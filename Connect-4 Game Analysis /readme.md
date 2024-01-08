# Connect-4 Outcome Analysis Project
## Abstract
This project applies various supervised and unsupervised machine learning algorithms to analyze legal game positions in Connect-4. It explores the efficacy of different techniques such as Logistic Regression, Decision Trees, SVMs, Neural Networks, and K-means clustering, aiming to predict outcomes and provide insights into the Connect-4 dataset.

## Introduction
Connect-4 is a two-player board game with a simple objective: connect four discs of the same color in a row, column, or diagonal. This project investigates the Connect-4 game dataset, comprising legal game positions where victory is not yet achieved, and the next move is not forced.

### Goals
- Examine the effectiveness of various analytical techniques.
- Utilize supervised algorithms for outcome prediction.
- Employ unsupervised learning for pattern discovery.

## Theoretical Background
A detailed discussion of each algorithm's theory and application is provided, encompassing topics like Logistic Regression, Decision Trees, SVMs, Neural Networks, PCA, SVD, and Clustering.

## Methodology
The project includes data visualization, preprocessing with one-hot encoding, training various models, and evaluating them based on accuracy, silhouette score, and completeness score. 

## Computational Results
The Random Forest model achieved the highest accuracy at 81.94%, while the clustering algorithm had low performance metrics, indicating a lack of clear clustering patterns in the dataset.

## Discussion
Insights into feature importance, model accuracy, and the visualizations of the game board positions are discussed. The findings suggest particular game positions that can influence the game outcome.

## Conclusion
The project demonstrates the effectiveness of machine learning models like Random Forest and Neural Networks in predicting Connect-4 outcomes. It also highlights the limitations of certain models and clustering techniques in the context of the dataset.

## Requirements
List of libraries and versions used, e.g., scikit-learn, TensorFlow, Pandas, NumPy, etc.
