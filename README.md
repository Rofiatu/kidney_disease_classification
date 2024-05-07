This project was part of a learning assessment at GoMyCode.

It involved the analysis of a kidney dataset obtained from Kaggle. The dataset (Kaggle: https://www.kaggle.com/datasets/mansoordaku/ckdisease) contains 25 features collected over a 2-month period in India.

I sought to understand the relationship between and among the features and used both supervised and unsupervised learning models to find which set of features (if any) can be successfully used to classify a patient as ckd or non-ckd.

The following specific tasks were assigned to us by the tutor:

Section A: Supervised Learning

- Task 1: Load the dataset of kidney disease.
- Task 2: Rename the columns
- Task 3: Apply logistic regression, and print the confusion matrix to validate your model.
- Task 4: Apply KNN and choose the optimal number of neighbors
- Task 5: Apply decision tree, plot it and calculate the accuracy.
- Task 6: Apply random forest, calculate the new accuracy and compare it with the previous results.

Section B: Unsupervised Learning
- Task 1: Drop out the target variable (named “classification”)
- Task 2:
  * Use hierarchical clustering to identify the inherent groupings within your data
  * Plot the clusters
  * Plot the dendrogram
- Task 3:
  * Use k-means clustering and select the optimal k
  * Plot the clusters

**Implementation**

My independent variable was the classification of features into ckd and non-ckd.

After cleaning and standardising my data, I used XGBoost and Select K Best, to identify the most relevant features for my supervised modelling. The following features yielded the most significant scores: haemoglobin, specific gravity, hypertension, red blood cell count, albumin, blood glucose random and packed cell volume.

After my modelling, Logistic regression, KNN and Random Forest returned the same accuracy score of 98.75%; while Decision Tree returned an accuracy score of 97.50%

The unsupervised learning, on the other hand, did not yield useful or distinct clusters across the available features. However, age seemed to provide some classification prospect, so I plotted age against some of the other individual variables for further investigation.

I made the following observations from my further analysis:

- Age does not appear to be a determining factor of the following conditions: specific gravity, sugar, blood glucose random and blood urea.

- On average, people of different age groups have average levels of these conditions but in certain situations, they can be found to have higher or lower levels, depending on their lifestyle choices, pre-existing health conditions and/or genetic attributes.

Further, I observed the following from the cluster groups I generated:

- Younger and older people generally have higher bloood pressure than people of mid age

- People of mid-age generally have higher albumin levels than people of young age or older age

- Younger and mid-age people generally have higher red blood cells than older people

- Mid-age people have higher pus cells than younger and older people

- Younger people generally have lower pus cell clumps, but in few extreme situations, they can have higher pus cell clumps than the other age groups

- Younger people have lower bacteria levsls than mid-age or older people
