# Evan Whittaker's Portfolio

# [Credit Card Clustering Analysis]([https://github.com/EvanWhittaker97/2023_NFL_Draft](https://github.com/EvanWhittaker97/banking_data)

**Tools Used**
1. R
2. Excel

**Clustering Algorithm Code:**

[Repository]([[https://github.com/EvanWhittaker97/2023_NFL_Draft/blob/main/Data_Manipulation_Cleaning](https://github.com/EvanWhittaker97/banking_data/blob/main/github_code.r](https://github.com/EvanWhittaker97/credit_card/blob/main/github_code.r)

**Data Source:**

https://www.kaggle.com/datasets/arjunbhasin2013/ccdata

**Project Scope**

The scope of this project was to perform a k-means clustering algorithm on the credit card data set to reveal trends in the data. The focus was

specifically on conducting exploratory data analysis, customer segmentation and potentially reveal cardholder behavior. 

**K-Means Output**

First, I determined the optimal number of clusters using the elbow method. As you can see below, the elbow indicated that 4 clusters appeard to be the most optimal number:

![](https://user-images.githubusercontent.com/64989275/233794078-4a66b2c6-cf6a-4cea-a5fa-27cae186a02f.png)

Then, after writing the k-means algorithm code, it unveiled the following clusters:

![](https://user-images.githubusercontent.com/64989275/233794078-4a66b2c6-cf6a-4cea-a5fa-27cae186a02f.png)

Once the clusters were determined, I added them back to the original dataset so I could conduct some basic exploratory analysis using Excel to demonstrate the power of clustering:

![](https://github.com/EvanWhittaker97/credit_card/blob/main/Average_Cash_Advance_Frequency.png)
![](https://github.com/EvanWhittaker97/credit_card/blob/main/average_balance.png)
![](https://github.com/EvanWhittaker97/credit_card/blob/main/average_tenure.png)

As you can see, it appears that the 3rd cluster has some concerning findings. The cardholders in the 3rd cluster have the highest frequency of cash advances by a significant margin. If there's one important thing to know, cash advances are detrimental to your credit!

Given this finding, I decided to look into the average balance outstanding for each cluster. Unsurprisingly, the 3rd cluster has the largest outstanding balance on their cards by nearly $1000.00. Finally, I wanted to determine the loyalty of these cardholders. Often times,

cardholders with these financial habits won't spend a ton of time with a single provider. I decided to visualize the average tenure by cluster. Although the 3rd cluster did have the shortest tenure with the card provider, it appears that the tenure wasn't short enough

for the findings to be conclusive. Nontheless, further exploratory data analysis on the 3rd cluster would certainly shed light on their lacklustre creditworthiness. 

# [Creating 2023 NFL Draft Rookie Grades Based on Measurables ](https://github.com/EvanWhittaker97/2023_NFL_Draft)

**Tools Used**
1. Python
2. Power BI
3. Power Query

**Cleaning/Manipulation Code:**

[Repository](https://github.com/EvanWhittaker97/2023_NFL_Draft/blob/main/Data_Manipulation_Cleaning)

**Project Scope**

The goal of this project was to analyze the athleticism of NFL rookies in this upcoming 2023 draft. 

To accomplish this, I started by gathering data for different positions such as DL, EDGE, LB, OL, QB, RB, S, TE, and WR, and stored them in CSV files. Then, I used the Pandas library in Python to read the data from each CSV file into a DataFrame.

There wasn't a lot to clean in this data. However, I removed the players who didn't test in 3 or more of the athletic testing fields so an accurate grade could be determined. Furthermore, I wanted the height field to be something easier to quantify, so I converted the height from inches to feet. 

Next, I calculated the percentiles for each player's performance in the athletic tests, such as the 40-yard dash, vertical jump, and cone drill. The challenge was creating percentile grades by position. It was imperitive that I only compare apples to apples. For example, it wouldn't be fair to compare speed of a WR to the speed to an OL. 

I then combined each position's CSV into one and loaded it into Power BI.

The Power BI dashboard was designed to be both appealing and interative. The goal was to create a dashboard that someone with no football knowledge could look at and understand exactly how athletic the prospect was. The user has the ability to filter players by position then select the specific player they want to see metrics and the final grade for. 

**Dashboard**

![](https://user-images.githubusercontent.com/64989275/233794078-4a66b2c6-cf6a-4cea-a5fa-27cae186a02f.png)
