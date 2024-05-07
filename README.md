In this project, I analysed a kidney dataset obtained from Kaggle. The dataset (Kaggle: https://www.kaggle.com/datasets/mansoordaku/ckdisease) contains 25 features collected over a 2-month period in India.

I sought to understand the relationship between and among the features and used both supervised and unsupervised learning models to find which set of features (if any) can be successfully used to classify a patient as ckd or non-ckd.

I made the following observations in the course of my analysis:

- Age does not appear to be a determining factor of the following conditions: specific gravity, sugar, blood glucose random and blood urea.

- On average, people of different age groups have average levels of these conditions but in certain situations, they can be found to have higher or lower levels, depending on their lifestyle choices, pre-existing health conditions and/or genetic attributes.

Further, I observed the following from the cluster groups I generated:

- Younger and older people generally have higher bloood pressure than people of mid age

- People of mid-age generally have higher albumin levels than people of young age or older age

- Younger and mid-age people generally have higher red blood cells than older people

- Mid-age people have higher pus cells than younger and older people

- Younger people generally have lower pus cell clumps, but in few extreme situations, they can have higher pus cell clumps than the other age groups

- Younger people have lower bacteria levsls than mid-age or older people
