# Classification on Imbalanced Data
 This repository is dedicated to exploring various techniques and methodologies for dealing with imbalanced datasets in classification tasks. Imbalanced data is a common challenge in machine learning, where certain classes are underrepresented compared to others. This imbalance can lead to biased models that perform poorly on minority classes.

In real-world, when performing classification, the situation of having a imbalanced class is a very common situation. If we don't handle it and build the models to train on it, there will be bias and we will not be able to get an accurate and reliable outcome. 

The data is about an insurance claim frequency prediction. In total, there are 58,5892 samples and 41 features.

## Count difference in class:
Below we can clearly see the difference in the count of the classes, this is an example of Imbalanced data:
![alt text](image.png)

There is a huge difference between the ones who have claimed (1) against the people who haven't claimed their insurance (0).

If this data is directly used to train the model, the predictions it will make will be biased. So, challenges like these needs to be addressed before building the model.

## A heatmap to see the correlation:

To understand the relationship between the target class (claim_stauts) and independent features, we need to know how do they correlate. So, let's plot a heatmap that will show their relationship to better understand them.
![alt text](image-1.png)

It seems, subscription_length, vechicle_age, customer_age,and region_density are only correlated with the
claim_status. 

Let's see these features and try to understand their distribution.
