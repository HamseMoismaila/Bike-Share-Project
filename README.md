# Bike-Share-Project

## DATA OVERVIEW

BIKE SHARE ANALYSIS file contain all SQL queries that I use to Clean and EDA

READMe file contain all way process to answer this business case

### Objectives

In project I was assuming junior Data analysts in Bike share company . The director of marketing believes the company’s future success depends on maximizing the number of annual membership.

For main Business goal #was increase number subscribers . So, there was three main questions.

1.How do annual members and casual riders use Cyclistic bikes differently?

2.Why would casual riders buy Cyclistic annual memberships?

3.How can Cyclitic use digital media to influence casual riders to become members?

Director has assigned to me the first question to answer: How do annual members and casual riders use Cyclistic bikes differently?


I started with most important part of this Job which To understand business Task properly and Consider Key stakeholders Then, I heard to location of data which was company internal data to download, before that i had some questions about organization of data,is it reliable for analysis and credibility of this data??

I will trying to answer 

1. avg trip duration per usertype 
2. Total of each usertypes 
3. Age of our difference between cusomers 
4. Avg trip duration for each weekday and Month


I started to download the Dataset to start the Process from the Bike share company database link Download the previous 12 months of Cyclistic trip data.

### Preparing data

It contained four .CSV files which each one contained 4 months in Quarters. then, I dive into data to check it is format and how it organize. It was long format.![All Data colmuns](https://user-images.githubusercontent.com/122876767/226197358-0acc5a22-40f9-461b-a926-ca37cd230e53.PNG)

It different columns but most important column that I am going to use  is  the one that has  annual member and daily customer
Now, We going to through prepare of analysis our data set in order to answer the business case. This is Dataset contained more than 540000 Rows in each File 

### Cleaning Data 

1.  First, I am going to starting Cleaning data, And I used Excel. cheching for Duplicates 
![Duplicated](https://user-images.githubusercontent.com/122876767/226198643-3daa4724-c9e3-4697-b3ec-59ced92f5b5e.PNG)

2.After checking out for any blanks  and Errors in dataset It show that there some in gender column  and birthyear 
and Remmove 

3. Sorting and Filtering Data to check for any types of errors and 

### Process Data 

1. Adding new column to Table called weekday using TEXT FUNCTION 

![adding New Week day column](https://user-images.githubusercontent.com/122876767/226199058-f8a1f103-3ed1-40e5-86aa-40ecafe7612d.PNG)

2.Again, I dive down to data in trip duration which is time user was using the bike. I found some trip duration is way more that 24 hours , some other are less than  1 minute which is outlier to our data. So, I decided to remove all trip length greater than 24 hours and less 1 minute

![More Than 1440](https://user-images.githubusercontent.com/122876767/226199225-96d7efa2-2729-4c3e-baa3-0fe1092f2bf7.PNG)


### Analysing 

Now, it time  To analyze  and Import it Into SQL to do some Further analysis before that  I  did some calculation and descriptive analysis to get better understand about data.,and then start analysis  step  by step

I strted analysing using SQL Steps are in SQL BIKE SHARE ANALYSIS File to 

1.join all the Four  quarters in single Table name Full_Year

![Full_year](https://user-images.githubusercontent.com/122876767/226199628-24831db2-971e-40a7-8e62-656885e7b46b.PNG)


2.-Number of Customers Vs Subscribers in 2019

![Customer Vs ssubscribers](https://user-images.githubusercontent.com/122876767/226199667-3acd0ff4-5d82-4543-adfc-b726f68c3a6c.PNG)

3.Number Of minutes Per User

![Total Min Subscriber Vs Customers](https://user-images.githubusercontent.com/122876767/226199742-3a207867-0627-41ee-a8e5-837f4825903e.PNG)


4.Frequenccy Tripduration per Month as usertype

![Months Ananlysis](https://user-images.githubusercontent.com/122876767/226199791-8b75b7e2-5903-4b96-9932-ed8b45449edd.PNG)

5. Frequency Trip Duration per Weekday  and weekend as usertype.
![weekdays](https://user-images.githubusercontent.com/122876767/226199843-c6277a9c-0624-44e4-99f7-b9ac15648551.PNG)


### Sharing Insights through Viz


![Bike share project](https://user-images.githubusercontent.com/122876767/226199911-fdee2fe4-2a66-45da-876b-eee4009c02b1.PNG)

#### KEY INSIGHTS 

1. 87%  of user s are subscribers while only  13%  are  daily customer Customers

2. August, September and October are  Months with highest customer and subscriber.

3.During weekday is highest avg trip for subscribers   while weekend  is highest avg trip duration for daily customers.
Tuesday is day  with highest  avg trip for subscribers and lowest for customers 

4.People who are born in 1980 & after  are highest number of our users 


### Recommendation 

The most People that are using our services are 50 Years and younger so, we have target those people especially 
During August, September and October it is best time to make advertising to customers in order to make them annual because when usage of bikes is extremely high.















