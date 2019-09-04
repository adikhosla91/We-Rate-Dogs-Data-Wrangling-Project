
# Data Wrangling/Analysis(We Rate Dogs Twitter Data Set) 

## Packages Required
* Numpy
* Pandas
* Seaborn
* Matplotlib
* glob
* json
* requests
* json
* tweepy (for twitter api)
* timeit


## System and Software Requirement
* Python Version--> 3
* Ram : 2GB
* Notebook: Jupyter Notebook

## File Format
* twitter-archive-enhanced.csv --> comma seperated file
* image-predictions.tsv --> tab seperated file
* Using twitter api to create twitter_json.txt file

## Data Wrangling 

### Introduction
In this report we will be describing about the Data wrangling process and we will showcase the wrangling steps on WeRateDogs dataset.  The data wrangling process can be divided into three parts:
* Gathering of data --> Gathering date from different sources
* Assessing of data -->  Checking the data visually and programmatically to identify any abnormalities in the data
* Cleaning--> Removing the abnormalities from the data and make it clean for data analysis or to apply machine learning algorithms


### Gathering Data
In this report we have gathered data from three different sources and programmatically we have uploaded it into Jupyter notebook. Data Sources of data gathering:
1.	CSV File(twitter_archive_enhnaced.csv)
2.	TSV File(image_predictions.tsv) downloaded from url :https://d17h27t6h515a5.cloudfront.net/topher/2017/August/599fd2ad_image-predictions/image-predictions.tsv
3.	Accessing twitter api using the api key and secret details. Gathering data and writing it to tweet_json.txt file. These files were loaded into Jupyter notebook using pandas’ libraries functionality and we made three dataframes for storing the files above into Jupyter notebook
   For accessing the twitter api we used library known tweepy. We then queried the tweeter data and extracted information such tweet_id ,favourite_count, retweet_count


### Assessing Data
Data assessing can be done in two ways a.) Visual Assessment   b.) Programmatic Assessment.  For assessing the dataframes in we did both visual and programmatic assessment. For Visual assessment I used Excel. For image_predictions.tsv; I downloaded the file and then performed visual assessment on it. For Programmatic assessment I used pandas and python’s in-built functions such as 1.) Head 2.) Tail
3.) value_counts(),4. Nunique()5. Info(), 6. Describe() and other string functions
The dirty and messy data usually are divided into three buckets such as 1.) Completeness, 2.) Tidiness 3.) Quality, but for this project we only addressed 
Tidiness and Quality issues
![image.png](attachment:image.png)

### Cleaning Data
In cleaning process, we tackle the completeness issue first, then the tidiness issue and then the quality issues. But for this project we will be tackling the tidiness issues first and then we would be improving the quality issues. The cleaning process is intensive, so we should always Define the cleaning step, code the cleaning step and then test it. So, while performing the cleaning process I followed this approach. So that I can track what changes I made and what was the cleaning code; when I want to run the code again

### Conclusion
To conclude, the data wrangling process of gathering, assessing, cleaning is important part; because if we have unclean and messy data the conclusion and the results that we make from it will be incorrect. The incorrect information provided to senior management will cause in taking incorrect business decisions. We can also say that the data wrangling process is an iterative process and we can perform it as soon as we see if something is missing or if we missed something during the data analysis process

## Data Analysis and Visualization


### Introduction
This report focuses on data analysis of WeRateDogs twitter_archive_master dataset. The twitter_archive_master is the cleaned csv file that was stored after the cleaning process. The report below will have some basic visualizations that uses matplotlib and seaborn libraries such as barplot , distplot, piechart , scatterplots 

### Analysis Result
* BarPlot between Source and it's count
![image.png](attachment:image.png)


In the count plot above we can see that most the twitter updates on WeRateDogs page was done using the twitter app on Iphone, the updates using the web-client and twitter deck are very low. We can say that majority of the users like to use twitter app on I phone because it is easy and convenient
* Barplot between breed and it's popularity rating
![image.png](attachment:image.png)
The bar plot is between the dog_breeds in type 1 prediction analysis and their popularity. For the analysis purpose I have taken the sample data to plot the bar-plot so that we can see the range of the ratings. The ratings go as high as 1.4 to as low as approx.  0.1

* Scatter plot retweet count and favourite_count over years
![image.png](attachment:image.png)
Here we can see relationship between favourite_count and retweet_Count. The relationship is positive. We can also see that most of the values are for all the years are 20000. The maximum value for retweets is 80,000 and maximum value for favourite_count is around 130000.This tells us over the years with increase in favourite_count the retweet_count has also increased
 distribution. That also could suggest that the model is not good enough

* Line chart of Users tweeting over years
![image.png](attachment:image.png)
Here we can see the trend of the line graph with counts and the month. We can see that in latter part of 2015 the user count tweeting started increasing and then we can see that in 2016 user count decreased and then in May it started increasing and slowing decreasing again. In 2017 we can see the users that tweeting is reducing.

* Bar plot of Dog_Stages
![image.png](attachment:image.png)
Here, we can see the distribution of dog stages. It shows that ‘pupper’ (a small doggo, usually younger) is the most popular dog stage, followed by ‘doggo’ and ‘puppo’. It could be due to the young and unmatured dog is usually cuter than the adult dog. It should also be noticed that there’s huge amount missing data in dog stage, hence the distribution might not be true.


```python

```
