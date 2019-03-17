# WeRateDogs
Wrangle and Analyze the data from the Twitter WeRateDogs

2019-03-10 In the Udacity Data Analytics Nanodegree, I'm working on a Data Wrangling Project with information from the twitter WeRateDogs. Hopefully I can upload the first ipynb tomorrow.

2019-03-11: I will upload an ipynb and html, what reflects the project status. More information will follow soon.

2019-03-12: Solved the following issues:
* Not every value of the column 'rating_denominator' has value 10
* each variable forms a column: rating_numerator and rating_denominator are actually one variable but separated in two columns (should be merged, ideally e.g. 8/10)

2019-03-13: Solved the following issues:
* datatype of p1, p2 and p3 is object and not category
* data type of column 'timestamp' is object and not datetime

2019-03-14: work in progress:
* dogs sometimes are in two dog stages
* each variable forms a column: for dog stage, there are four columns, they should be merged to one column called 'dog_stage' (datatype: category with values: None, doggo, floofer, pupper, puppo)

2019-03-15: Solved the following issues:
* dogs sometimes are in two dog stages
* each variable forms a column: for dog stage, there are four columns, they should be merged to one column called 'dog_stage' (datatype: category with values: None, doggo, floofer, pupper, puppo)

2019-03-16: Solved the following issues:
* changed datatype of 'dog_stage' to category
* conducted data analytics and visualizations
