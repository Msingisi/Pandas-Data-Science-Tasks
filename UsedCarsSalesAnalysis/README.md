# Pandas-Data-Science-Tasks

## Company Background

Discount Motors is a used car dealership in the UK. They want to lead the way in used cars.
Selling to customers who want the latest and greatest features, without the price tag of a
brand new car.

The UK Government has now announced that from 2030 all new cars will be required to be
zero emissions. Although this won’t impact the used car market, it is expected that buyers will
give more consideration to the future value of their cars. And petrol and diesel will likely have
a much lower value after 2030.

## Task

I am sure you have heard that by 2030 we are only going to be able to sell Electric vehicles
here in the UK. We want to run some campaigns to promote used Electric cars. We know
that in the last year we haven’t sold any electric cars, so we want to know about hybrids to
give us some ideas. We want to know anything you can tell us about how the sales differ
between hybrid and other types from sales over the last six months.

We know that there are less hybrid cars for sale. We think they are more expensive, so we
need to make them more appealing. We think hybrid could be a good way to get buyers to
think about more environmentally friendly cars.

Our goal is to increase the number of sales of hybrid and electric cars next year.
We want to get moving on this campaign as soon as possible to beat our competitors so
the sooner you can share some insights the better.

## Customer Questions
* What is the most common place type in this local market?
* How does the range in number of reviews differ across all shops?
* How does the number of reviews vary across each place type?

## Data Validation
The dataset contains 6738 rows and 9 columns before cleaning and validataion. I have validated all the columns against the criteria in the dataset table:
* model: 18 models without missing values, same as the description. No cleaning is needed.
* year: 23 unique values without missing values, from 1998 to 2020, same as the description. No cleaning is needed.
* price: numeric values without missing values, same as the description. No cleaning is needed.
* transmission: 4 categories without missing values, same as the description. No cleaning is needed.
* mileage: numeric values, same as the description. No cleaning is needed.
* fuelType: 4 categories without missing values, same as the description. No cleaning is needed.
* mpg: numeric values without missing values, same as the description. No cleaning is needed.
* engineSize: 16 possible values without missing values, same as the description. No cleaning is needed.
After the data validation, the dataset contains 6738 rows and 9 columns without missing values.

## Data Discovery and Visualization

# What is the most common place type in this local market?

the graph below shows that there are four possible types of coffee stores included in this data. The most common type listed is a coffee shop, with cafe being second although with half the number of locations. This would suggest that the team should focus on distributing their new cups in coffee shops as they are more common.

![alt text](https://github.com/Msingisi/Pandas-Data-Science-Tasks/blob/main/images/place_types.png)

# How does the range in number of reviews differ across all shops?

As the marketing team thinks that the number of reviews a place gets will be important, Looking at all reviews, we can see that most places have had less than 1000 reviews. There are some outliers that get more than 3000 reviews but this is very uncommon. When looking for places that have high reviews the team should aim for locations having over 1000 reviews, but be aware they may need to work with 500 reviews or more.

![alt text](https://github.com/Msingisi/Pandas-Data-Science-Tasks/blob/main/images/%23%20of%20reviews.png)

# How does the number of reviews vary across each place type?

Finally we want to combine the two pieces of information to see how the place type impacts number of reviews. So far coffee shops with over 1000 reviews would be ideal but we need to look at the two variables together to see if this is realistic.

When looking at just the reviews we excluded a single outlying value so that we could see the majority of the data. To show the impact, we can look at the range of number of reviews by place with this outlier in the data. In the graphic below you can see that this outlier is dominating the data and making comparison difficult. To make it easier to compare the rest of the data, we will remove this outlier.

![alt text](https://github.com/Msingisi/Pandas-Data-Science-Tasks/blob/main/images/plot_place_types.png)

After we remove the outlier we can focus on the main range of data. Although Coffee Shops do include the place types with the largest number of reviews, the interquartile range of the number of reviews is lower than Cafe and espresso bar types. This would suggest that the majority of the number of reviews may be lower than other types. However, this could also be an effect of having the largest number of locations, so the large number of low review locations brings the median down.

![alt text](https://github.com/Msingisi/Pandas-Data-Science-Tasks/blob/main/images/pllot_place_types_outliers.png)

## Recommendations

Based on all of the above, we would recommend that the team focus on coffee shops with reviews over 1000 to start, but also keeps an open mind to including cafes and espresso bars with high reviews. Further analysis should be done to understand if store type really does impact the number of reviews. The team should also consider including their cups in stores with lower reviews so that we can further analyze whether reviews has any impact over the popularity of the new cups.

## Resources

datacamp.com: https://app.datacamp.com/workspace/w/396b8323-75d7-4715-b390-fa43e386fb3c





