# Data manipulation and assessment using Pandas

**Degree**: Data Science | **Class**: 815 | **Institution**: Let's Code | **Module**: IV - Programming Techniques - Final Project

## 👨‍🏫: Professor
[Pedro Gengo](https://github.com/pedrogengo)

## Peers of this assignment:
👩‍🎓: [Ana Gabriela de Castro Almeida](https://github.com/almeidacastrogabriela)
👨‍🎓: [Jeremias Diefenthaler](https://github.com/JeremiasDief)
👨‍🎓: [Daniel Aquino](https://github.com/DanWolks)

## 📍Files Info:
In this repository it's possible to find:
- English version of the project
- Portuguese version of the project

## 🖥️ Concepts:
- Setting up the analysis.
- Reading **three** databases with different delimiters
- Joining those dataframes into a **single one**.
- Data manipulation using Pandas.
- Numpy.
- Using an additional library to generate reports Pandas_Profiling.
- Generating graphs with Matplotlib and Seaborn.

## 📖 Description
The project consisted into answering the following questions:

Question 1. Using *shape* to determine the number of observations and columns of the entire dataset.
Question 2. Finding the number of **women amongst the ages of 26 and 35 years** in the dataset.
Question 3. Finding the number of unique users of the dataset.
Question 4. Record percentage (row percentage) with at least one null value (None, ǸaN, etc.)
Question 5. Quantity of null values in the variable (column) with the highest number of nulls
Question 6. Most frequent value (without nulls) at Product_Category_3
Question 7. True or False
Question 8. ID of the user who spent the most
Question 9. Determine which group (men or women) spent the most
Question 10. New table with the most purchased category by each customer.
Question 11. Normalize the Purchase column.
Question 12. **Marital Status Purchase Analysis. Explain**
Question 13. **Which variables had the most impact over the purchase price? Explain**.

## 📊 **Graphs and Detailed Analysis of Question 12 & 13.**

## Question 12

Does the marital status has an influence over the amount spent and at the product category bought? Demonstrate it.

In case the company wants to sell more products at the category 14, should it invest in advertisements to which marital status?

#### **For this analysis, it was assumed that "0" represents single customers while "1" stands for married customers*

<img src="images/Marital_Purchase.png" width="300">


According to the data seen above, it's possible to identify that there're more single customers making purchases during Black Friday; however, the group that had higher expenditures were the married customers.

This tends to happen due to the difference in lifestyle amongst single customers and married ones.

Meaning that having a carefree lifestyle, i.e, with less financial responsibilities than a married person, single people can afford to purchase more products than a married person who needs to take into account household budgets, financial commitments, debts, etc. before actually purchasing stuff online.
Nonetheless, even though the data exhibits that there are more single customers, the average of items purchased by married customers presents higher values.
For example, while a single customer can purchase 10 products varying amongst stationary and office supplies, a married customer can purchase a single product, like a laptop, which would therefore surpass the total amount of the purchase made by the single customer.

<img src="images/Marital_Stat_Cat_Purch.png" width="300">


Further analyzing the purchase behaviour of each marital status by category option, while verifying the expenditure percentage, more specifically looking at the data at the column "Percent_by_Category", it's possible to identify that the marital statues does not really influence the category of product purchase, since, proportionally, the amount of products purchased by category in each marital status it's almost equivalent.

<img src="images/Catg14_Marital.png" width="300">


### Prediction of advertisement budget for Category 14 analysing customer behaviour by marital status.

Defining to which Marital Status the advertisement budget needs to be invested in order to sell more Category 14 products will depend solely on the company's strategy.

Single customers are organically buying more products in this category than married ones; therefore, if the company wants to play safe and ensure its sales will go through the roof, it would be logical to invest the advertisement budget into this group and further push sales.

However, if the company wants to capture married customers in order to change their purchase behaviour in this product category, it would be a smart financial budget decision to bombard adds to this group to entice the customer to buy. 
Nonetheless, it's necessary to observe that investing all the advertisement budget into this strategy will not guarantee the married customers receiving the adds will actually purchase products in this category.

## Question 13

Which variables had the most impact over the purchase price? How did the team reach this conclusion?

Variables: Gender | Age | Marital_Status | Occupation | City_Category | Stay_In_Current_City_Years

### As previously seen at Question 09:

- Genre has a great influence over Purchase habits.
- Meaning "Male" users bought way more than the "Female" ones.
- Below there's again the data sampled to exhibit the importance of this variable to predict Customer Behaviour.

<img src="images/Gender_Purchase.png" width="300">


#### As Genre has an impact over Purchase amount, it's necessary to determine weather Age has an impact as well:

<img src="images/Age_Purchase.png" width="300">


#### Now that it was seen that both Genre and Age do impact how much a customer will spend while separately, grouping both data will present a much clearer view of the purchase habits:

<img src="images/GenAge_Purch.png" width="300">


From the previous graph, it can be seen that the average number of purchases made by "Women" remains very close regardless of age.

Furthermore, it's clear that not only "Male" users tend to spend most, but they also are the heaviest spenders when assessing Age Group.

Male customers amongst the ages of 51 to 55 represent the heaviest spenders.

#### After understanding consumer habits that are influenced by one's genre and age, it's necessary to determine wether the marital status can also play a big role into one's purchase habits.

<img src="images/Marital_Purchase.png" width="300">


As previously seen, it's possible to identify that there's more single customers making purchases during Black Friday; however, the group that had higher expenses was the one of married customers.
The average spending between both marital status is quite similar.

#### Not only one's genre, age and marital status can influence spending habits, one's occupation can also play a big role in it.¶
Looking at the data, a clearer understanding can be acquired:

<img src="images/Occupation_Purchase.png" width="300">

#### When assessing the Purchase behaviour according to one's "Occupation", it's possible to see that this data has also an impact, meaning that those whose professional occupation belongs to 12, 15 and 17 are the heaviest spenders during blackfriday.

- In the data presented below, there's an assessment of purchase behaviour taking into account one's Genre, Age and Professional Occupation.

### The city where one lives can also determine the purchase behaviour when it comes to shopping during Black Friday.

As the data is masked, it's not possible to determine each city nor to understand if it represents a countryside city or a capital.
Nonetheless, it's quite clear that those living at city with category C tend to spend the most during BF.

<img src="images/City_Purchase.png" width="300">

### City category somewhat has an impact into one's purchase behaviour; therefore, it's necessary to assess whether how many years one's been living in that specific city also portrays an impact at the purchase.

<img src="images/Years_Lived_Purchase.png" width="300">


Looking at the data above, it's possible to understand that those who have been living in a city for 2 years are likely to spend more at Black Friday purchases.

It's possible to make an inference that this is linked to the fact that a person living for 2 years in a certain city:
- Is in a comfortable and stable situation financially, and/or
- Has defined that particular city as a long-term home;

Therefore, it's possible to make decoration adjustments and/or furnish one's house; thus, Black Friday deals are a huge plus.

Based on the data, the average spending for the period the customer lives in the city is equivalent amongst the years 2 to 4+.

#### Assessing City Category and Years lived in it can also determine one's purchase behaviour, as not necessarily a person who's been living for 2 years in city C will have the same spending habits as a person living for 2 years in city A & B.


Further observing the data, through the information it's possible to verify that the city in category C remains as the city with the customers who spend the most and, besides that, they represent the group that spends the most when assessing how long one's been living in that particular city category.
