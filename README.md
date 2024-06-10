
# Oasis Infobyte Data Analytics Internship
As a part of my Data Analytics Internship at Oasis Infobyte spanning 1st May,2024 till 5th June,2024, I completed 3 projects :

1. Exploratory Data Analysis (EDA) on Retail Sales Data
2. Data Cleaning on New York City Airbnb Listings
3. Analyzing Google Play Store Data


## EDA ON Retail Sales Data
![image](https://github.com/AmruhaAhmed/OIBSIP/assets/98407069/0b325e2a-2f9e-438e-8090-d40d4f9853d6)


As a part of my Data Analytics Internship at Oasis Infobyte, I have used a dataset from Kaggle (public domain) related to the Retail Sales Data collected from 10 different shopping malls in Istanbul, Turkey.

### Columns in the dataset

Link to the dataset: https://www.kaggle.com/datasets/mehmettahiraslan/customer-shopping-dataset

1. invoice_no: invoice number
2. customer_id
3. gender: either male or female
4. age
5. category: such as clothing,shoes, cosmetics, et cetera
6. quantity
7. price: this is price per unit item
8. payment method: either cash or debit card or credit card
9. shopping_mall: name of the mall

### Project Structure

1. Data Loading and Cleaning
2. Feature Engineering
3. Descriptive Statistics
4. Data Visualization
5. Data Analysis
6. Recommendations

### Data Loading and Cleaning

This step involved:
1. Loading the dataset into a Pandas dataframe
2. handling missing values
3. removing duplicates
4. correcting data types 
5. formatting the dates 

### Feature Engineering

This step involved creating columns based on:
1. categorization of malls such as Luxury mall, mega mall, mixed-use mall and outlet mall
2. location of mall -  whether the mall is located on the European side of Istanbul or on the Asian side of Istanbul.
3. total price of items
4. categorization of ages into different age groups of baby, young adult, middle aged adult and old adults.
5. total price of items purchased by each gender
6. total price of items purchased by each age group
7. total price of items purchased in each category of items
8. total price of items purchased through each payment method
9. total price of items purchased in each shopping mall
10. total price of items purchased in each mall location
10. total price of items purchased in each type of mall
11. unit price of items purchased by each gender
12. total quantity of items purchased by each gender
13. total quantity of items purchased from each category
14. total quantity of items purchased through each payment method
15. total quantity of items purchased in each shopping mall
16. total quantity of items purchased in each type of mall
17. total quantity of items purchased in each mall location
18. total quantity of items purchased by each age group

### Descriptive Statistics

This step involved getting KPI's from the crucial columns using measures of central tendency. Here are a few important bits of information derived from this step:
1. The average age of a person shopping in the malls is 43 years
2. On an average, a customer buys about 3 items of any type from the shopping mall
3. On an average, a person spends 689.26 Turkish Liras per item in a shopping mall
4. The number of purchases done by females are higher than those of males.
5. The payment method for most invoices is Cash
6. Majority of the invoices come from malls located on the European side of Istanbul

### Data Visualization
In this step, I utilized many different types of graphs such as bar charts and pie charts using matplotlib and seaborn libraries to explore and understand the data.

Few of the most pivotal graphs I made at this stage were:

1. Comparison of Payment Methods
2. Total Amount spent
3. Purchase trends in each month

### Data Analysis
In this stage, I analyzed the graphs and descriptive statistics to make the following inferences about the data:

1. Customers of age 37 years have the most invoices in shopping malls
2. On an average, a customer buys about 3 items of any type from the shopping mall
3. On an average, a person spends 689.26 Turkish Liras per item in a shopping mall
4. The maximum number of invoices are from the Mall of Istanbul
5. More invoices have been issued to females than to males thereby more amount of money is spent and more quantity of items are purchased by female customers.
6. Both male and female customers visit Luxury and Mega Malls, and the malls in European part of Istanbul more often.
7. Young adults ( 3 years to 39 years) have more invoices as compared to middle aged and old adults hence the total price and quantity of items purchased is higher.
8. Clothing emerges as the most popular category among all the invoices, followed by cosmetics and food/beverages.
9. Clothing and shoes, followed by technology items have the highest total price.
10. Price per item is the highest for technology category , followed by shoes and clothing.
11. Customers spend more in the month of October. There is a sharp decrease in the total price in November followed by a slight increase in December. A rough estimation can be made that males shop the most in September, whereas female customers shop more in July and October
12. Most of the payments have been done in cash followed by credit card.
13. More number of invoices have been issued by Kanyon and Mall of Istanbul than other malls.
14. The invoices are dominated by purchases from mega malls
15. Most of the invoices are from malls located in the European part of Istanbul

### Recommendations

Here are my top recommendations based on the insights gathered:

1. Malls should locate themselves in the European part of Istanbul and update their infrastructure to become Luxury or Mega Malls.
2. Malls should focus more on their young adult(3 years to 39 years) customers.
3. Malls should also focus more on their female customers as the number of invoices billed by females, the total price and quantity of items purchased by females is higher than that of males.
4. Malls should make adequate arrangements during the month of October as it is the highest billing month.
5. Malls should make sure that a customer can easily purchase items using cash.
6. Malls should focus more on selling clothing items to customers.

LinkedIn : https://www.linkedin.com/posts/amruha-ahmed_oasisinfobyte-intern-internship-activity-7194752879071571969-efTM?utm_source=share&utm_medium=member_desktop

## Data Cleaning on New York City Airbnb Listings

![image](https://github.com/AmruhaAhmed/OIBSIP/assets/98407069/aed915f2-eb16-4459-b440-95ae5401ef49)

As a part of my Data Analytics Internship at Oasis Infobyte, I have used a dataset from Kaggle (public domain) related to the AirBnB listings and metrics in New York City in the year 2019 to perform extensive data cleaning.

### Columns in the dataset

Link to the dataset: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data/data

1. id: Listing ID
2. name: name/description of the airbnb listing
3. host_id
4. host_name
5. neighbourhood_group: location of the listing
6. neighbourhood: area
7. latitude
8. longitude
9. room_type: listing space type
10. price: in US dollars

### Project Structure

I have performed data cleaning in the following steps:

1. Initial Data Exploration
2. Imputation
3. Date Parsing
4. Outlier Detection and Handling
5. Text preprocessing
6. Label Encoding
7. Column Removal
8. Min Max Scaling

### Initial Data Exploration

From this section of initial data exploration , I imported all the necessary libraries and  observed the following points:

1. name, neighbourhood group, last_review and reviews_per_month columns have NaN values.
2. There are no duplicate values in the dataset

### Imputation

In the dataset, name, neighbourhood_group, last_review and reviews_per_month column had several NaN values before this section
I imputed the NaN values in these columns by making use of statistical functions such as mean and mode.

### Date Parsing

As a precaution, I brought the dates contained in the last_review column into a common format

### Outlier Detection and Handling

Here are a few points I noted in this section:
1. Outliers can cause problems in model building so I decided to remove them from the dataset
2. I utilized z score technique to detect outliers in latitude, longitude and price columns as they are the most crucial columns to the analysis.
3. If z score lies between -3 and +3 then the data point is not an outlier otherwise it is classified as an outlier.
4. I created columns of z_latitude and z_longitude to store the z-scores of latitude and longitude columns respectively.
5. I removed the rows containing z_latitude > 3 and z_latitude<-3
6. There were no rows for z_longitude<-3.
7. I removed the rows where z_longitude>3
8. I created columns of z_price to store the z-scores of price column .
9. Since most of the outliers detected through the price column have names such as "luxury" and "trendy" and might have a reason for their high price, I will be keeping the outliers in the price columns as it is and not deal with them.
10. There were no rows for z_price<-3

### Text preprocessing

In this section, I have dealth with cleaning the text based columns such as name, host_name, neighbourhood_group and neighbourhood in the following manner:

1. I removed stopwords from the columns to concentrate on the more important words
2. I also included a punctuation removal function
3. I converted all these textual columns into lower case for easy handling.

### Column Removal

In this section, I removed some columns of id, host_name, z_latitude, z_longitude and z_price as they dont play a major role in the upcoming cleaning process and have less contribution in the visualization process.

### Label Encoding

In this section, I focussed on converting many of the text based columns into numeric type using label encoding method to help in easy handling.

### Min Max Scaling

In the final section, I performed min max scaling on numeric columns to prevent any column from dominating the machine learning algorithm.
1. I had initially divided the dataset into scaling and non-scaling features.
2. Then I performed min max scaling on scaling features and stored it in scaled features
3. I created new data frames from scaled features and non-scaling features then concatenated them into the final cleaned dataset 'df'.

LinkedIn : https://www.linkedin.com/posts/amruha-ahmed_data-oasisinfobyte-intern-activity-7194780743552679936-T5Am?utm_source=share&utm_medium=member_desktop


## Analyzing Google Play Store Data 

![image](https://github.com/AmruhaAhmed/OIBSIP/assets/98407069/490a2efc-1f04-4f6e-ba82-c838f2732891)

In this project done as a part of my Data Analytics Internship at Oasis Infobyte, I have performed an in-depth analysis of Google Play Store data. This analysis aims to understand the factors that contribute to an app's success, such as user ratings, number of installs, and category trends. By uncovering these insights, developers and businesses can optimize their app offerings.

### Datasets used 

Link to the datasets: https://www.kaggle.com/datasets/utshabkumarghosh/android-app-market-on-google-play

I have used two datasets from Kaggle related to over 9000 apps from 20+ categories, along with the reviews of apps for this analysis. The datasets I have used are :

1. apps.csv: It contains 14 columns pertaining to the apps listed on Google Play Store

2. user_reviews.csv: It contains 5 columns pertaining to the reviews received by each app and the corresponding sentiment.

### Columns in the Datasets

The columns present in apps.csv are as follows:

1. Unnamed: 0
2. App
3. Category
4. Rating
5. Reviews
6. Size
7. Installs
8. Type
9. Price
10. Content Rating
11. Genres
12. Last Updated
13. Current Ver
14. Android Ver

The columns present in user_reviews.csv are as follows:

1. App
2. Translated_Review
3. Sentiment
4. Sentiment_Polarity
5. Sentiment_Subjectivity

### Project Structure

I have followed the steps given below to analyze this data:

1. Initial Data Exploration
2. Data Cleaning
3. Feature Engineering
4. Descriptive Statistics
5. Data Visualization
6. Data Analysis

### Initial Data Exploration

I loaded the two datasets under consideration and stored them in pandas dataframes .  I also imported the necessary libraries.

### Data Cleaning

In this section, I implemented the following steps :
1. Handled missing values in critical columns like Rating and Reviews.
2. Converted data types for columns like Installs and Price.
3. Removed punctuation from text based columns such as category and Genres
4. Removed stopwords from text based columns such as Translated Reviews

### Feature Engineering

In this section, I created new columns in both the dataframes such as opinion type, average price of apps per category , average number of reviews per category and so on.

### Descriptive Statistics

This step involved getting KPI's from the crucial columns using measures of central tendency. Here are a few important bits of information derived from this step:

1. Most of the apps belong to the "free" category
2. The average rating of apps is 4.17
3. The average size of each app listed is 20.41 MB
4. Most of the reviews are positive


### Data Visualization

In this step, I utilized many different types of graphs using matplotlib , seaborn and wordcloud libraries to explore and understand the data.

Few of the most pivotal graphs I made at this stage were:

1. Distribution of ratings
2. Count of Categories of apps
3. Content Ratings of apps

### Data Analysis

Here are the top 15 insights I have gathered from the visualizations:

1. Majority of the apps belong to the "family" category followed by games and tools.
2. The average rating of apps is 4.17
3. The average size of each app listed is 20.41 MB
4. Finance, followed by lifestyle apps had the highest average prices among all categories
5. Art and design and education categories have the highest average ratings among all categories
6. Gaming apps, followed by family apps have the highest average size per category.
7. Communication, followed by video players category has the highest average number of installations among all categories
8. Majority of the apps listed are free to use
9. Free apps occupy slightly more size on an average as compared to paid apps
10. Average number of installations for free apps is far greater than the number of installations of paid apps
11. Most apps have "everyone" or suitable for all ages rating.
12. Tools, education and entertainment are the most commonly used words to describe the genre of apps
13. Most of the reviews evoke a positive sentiment
14. Most of the reviews are subjective in nature
15. Good, game, great are some of the most commonly used words in the reviews of apps

LinkedIn : https://www.linkedin.com/posts/amruha-ahmed_oasisinfobyte-intern-internship-activity-7194788290175115264-cego?utm_source=share&utm_medium=member_desktop

