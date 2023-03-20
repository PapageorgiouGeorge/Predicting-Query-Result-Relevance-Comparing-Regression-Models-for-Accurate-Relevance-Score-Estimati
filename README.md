# Predicting-Query-Result-Relevance-Comparing-Regression-Models-for-Accurate-Relevance-Score-Estimati
This project's objective is to predict the relevance of a result corresponding to a query, where each query is represented by search term(s) and the result by a specific product. A relevance score is assigned based on the congruity between the query and the answer, with higher scores indicating better relevance. Relevance scores are real numbers within the range of [1,3] (in increments of 0.5), where 1 signifies minimum relevance and 3 the maximum. Our task is to accurately predict the relevance score for an unknown query-result combination, utilizing the Root-Mean-Square Error (RMSE) as the evaluation metric.

To accomplish this, we will utilize train.csv, which contains query-answer pairs and their associated relevance scores; product_descriptions.csv, offering textual descriptions for each distinct product; and attributes.csv, comprising additional attributes for certain products, although some products may lack such supplementary information.

The technical approach includes importing necessary packages, loading the datasets, fixing typos, merging dataframes, performing stemming, generating numerical features, and applying various regression models. The models used for prediction are Random Forest, Ridge Regression, Gradient Boosting, XGBoosting, and Multi-layer Perceptron.

The final results show that XGBoost Regression provided the best performance with an RMSE of 0.4768. The most important features in predicting relevance were the length of words for the description, the ratio of product description word length to search term word length, and the length of words of the title.


## Contact Information

If you require access to the code in this repository, please reach out to me at g.papageorgiou.contact@gmail.com or on [LinkedIn](https://www.linkedin.com/in/giorgos-papageorgiou-3b27a9221), and I will be happy to assist you.
