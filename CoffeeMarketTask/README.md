# Pandas-Data-Science-Tasks

## Company Background

Caffeine Form is a company creating coffee cups from recycled material. Although they
started selling the products on their website last year, the results were not as good as they
expected. To better enter the market, they decided to collaborate with local coffee shops to
advertise and sell their coffee cups.

## Task

The marketing team is trying to come up with the best criteria to choose possible
collaborators by investigating the local market. They think focusing on the places with the
most reviews might have the biggest impact as more good reviews will create more
excitement for their cups.

## Customer Questions
* What is the most common place type in this local market?
* How does the range in number of reviews differ across all shops?
* How does the number of reviews vary across each place type?

## Data Validation
The original data is 200 rows and 9 columns. The first thing I did was to remove rows that should be excluded according to the data set description. I first removed rows where the Review value was missing. This was 2 rows, leaving 198 rows of data. I also switched missing values in the Dine in option and Takeaway option with False. There were no values that were false originally so this correctly made these columns True/False values.

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





