# world-happiness-analysis

This is my analysis of [this](https://www.kaggle.com/unsdsn/world-happiness) Kaggle dataset. 

My aim was to try and create a model that could accurately predict whether a country would be in the top 20 happiest countries based on its scores
and region, agnostic of the scoring criterion already in place, and see if the decision rules would prove interesting. 

# About the decision tree

This is not the only decision tree that can describe this data. There are several ones that can predict high ranking happiness with high accuracy. I just chose one with 
small maximal depth so it wasn't too daunting to read. There are numerous different decision trees (some with even smaller depth than this) that can predict with high
accuracy as well, but any with high accuracy can provide interesting insights. Indeed, each time I run this data, there's a chance it comes up with a different decision tree,
as it is shuffled each time, and each one that it comes up with is equally valid as long as it is a good predictor. I liked this one because it highlighted a perhaps unique
ability for Australia and New Zealand to be in the top 20 in happiness invariably of it having a low or high score in GDP.  I will also say that I've never come across a tree
whose root node wasn't this GDP <= 1.3 rule. 
