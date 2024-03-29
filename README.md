# Pandas-Data-Science-Tasks

## Company Background

Caffeine Form is a company creating coffee cups from recycled material. Although they
started selling the products on their website last year, the results were not as good as they
expected. To better enter the market, they decided to collaborate with local coffee shops to
advertise and sell their coffee cups.

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

![alt text](https://github.com/Msingisi/Pandas-Data-Science-Tasks/blob/main/images/%23%20of%20reviews.png)



