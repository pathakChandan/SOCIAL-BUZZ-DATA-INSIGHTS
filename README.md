# SOCIAL BUZZ DATA INSIGHTS

### INTRODUCTION
This is a job simulation project where I must pretend a data analyst role at a company, i.e. ACCENTURE. I work with a larger team, where each member has a different role and level of responsibility. Our team is assigned a new project for a client named Social Buzz. I get an opportunity to play as a data analyst in the company and showcase my data analysis and visualization skills.

### CLIENT AND BUSINESS PROBLEM
Social Buzz, a social media company, is the client. It is a social media platform to share various contents. Over the past 5 years, it has received unanticipated number of active user growth. Due to this, the amount of data that they create, collect and must analyse is huge. They are looking at bringing external expertise. Accenture is running a 3 month initial project in order to prove them that we are the best firm to work with. The objectives to meet:
- An audit of their big data practice,
- Recommendations for a successful IPO,
- **An analysis of their content categories that highlights the top 5 categories with the largest aggregate popularity.**

As a data analyst, I am given the task to meet the last objective.

### PROCESS
To tackle the problem, following five key steps are carried out.
1.	Obtaining Data and Understanding
2.	Data Scrubbing
3.	Data Modelling
4.	Data Analysis and Interpretation
5.	Findings and Recommendations

#### OBTAINING DATA AND UNDERSTANDING
The key to success on any data project is to understand the data in detail. The client sent 
- 7 datasets: Each data set contains different columns and values
- A data model: It shows the relationship between all the data sets and the links which can be used to merge the table
![image](https://github.com/user-attachments/assets/68c8bb07-9b2e-4010-800a-de9b20f00d22)

The domain of the client’s business and the data model is studied properly. The first step is to identify which datasets will be required to answer the business question, which is to figure out the top 5 categories with the largest popularity. Hence, Reaction, Content, and Reaction Types are selected as the relevant data sets.
- Popularity is quantified by the “Score” given to each reaction type.
- We therefore need data showing the content ID, category, content type, reaction type, and reaction score.
- To figure out popularity, we will have to add up which content categories have the largest score.

#### DATA SCRUBBING
The Data Exploration and Scrubbing is done in Microsoft EXCEL. We have three different relevant data sets, i.e Reactions, Contents and Reaction Types. The data is cleaned by:
- Removing columns which are not relevant.
- Removing rows that have values which are missing,
- Checking for duplicate rows,
- Changing the data type of some values within the column,
Three cleaned data sets are obtained undergoing data scrubbing.

#### DATA MODELING
First, all three tables are queried using Get Data. A final dataset is created by merging the three tables together from Query tab. Tables are merged according to the common columns, i.e Content ID column between Content table and Reactions table, likewise, Reaction Type column between intermediate merged table and Reaction Types table. The same thing could be obtained using EXCEL VLOOKUP as well.
![image](https://github.com/user-attachments/assets/dd97836f-57d4-40fc-b493-3fa6ed360527)

#### DATA ANALYSIS AND INTERPRETATION
By using pivot table, sum of scores per categories is obtained.
|Categories|SumOfScores|
|-------|-----------|
|Animals|74965|
|science|71168|
|healthy eating|69339|
|technology|68738|
|food|66676|
|culture|66579|
|travel|64880|
|cooking|64756|
|soccer|57783|
|education|57436|
|fitness|55323|
|Studying|54269|
|dogs|52511|
|tennis|50339|
|veganism|49619|
|public speaking|49264|

The same result could be obtained using “Sum If” formula. The result is the:
- Cleaned dataset
- The top 5 categories

  ![image](https://github.com/user-attachments/assets/c67ba400-62f8-4428-96e3-70c4175b0ead)

![image](https://github.com/user-attachments/assets/b6fc83ed-d2f3-40f7-96ee-1b95a53231b2)

![image](https://github.com/user-attachments/assets/4e365766-f331-47a0-bf82-b8ca3aaa62e1)

![image](https://github.com/user-attachments/assets/2cebbd2a-75df-4981-a2d5-0dd1c7442b43)

There are some other interesting insights that can be shared to the client.  For example, number of unique categories, total reactions per category and total content posts per category. 

### ANALYSIS
- Animals and science are the two the most popular categories of content, showing that people enjoy “real-life” and “factual” content the most.
- There are 16 unique categories.
- “Animals” category received 1897 reactions to the posts.
- The highest number of posts made was on the month of May 2021.

### INSIGHTS
Food is a common theme with the top 5 categories with “Healthy Eating” ranking the highest. This may give an indication to the audience within the user base. This insight could be used to create a campaign and work with heathy eating brands to boost user engagement.

### NEXT STEPS
This analysis is insightful, but it’s time to take this analysis into large scale production for real-time understanding of the business. We can show how to do this.





  


