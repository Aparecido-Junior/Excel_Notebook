# Excel Nootebook
This repository is a collection of the courses that I have been doing since 2024 as well as some projects that I will be updating. My goals is to share my steps towards my goal which is beccome a data analyst or data Scients or even something in between. 

## 1. Data Cleaning Framework & Documentation
A practical guide and framework for data cleaning processes in business analytics using excel. THe framework consist of 5 steps project:

- Conceptualize the data (identify granularity, metrics and dimensions);
- Locate solvable issues;
- Evaluate unsolvable problems;
- Augment the data;
- Note and documentation.


### 📋 Overview
This first Data Cleaning Framework project documents a comprehensive 5-step framework for data cleaning with business applications. The methodology focuses on preparing data to answer specific business questions rather than pursuing "perfect" data.

### 📊 Sample Context
This data is ficticous, however it does help an inspiring data analyst practice and apply business analytics concepts to practice as well as showcase for future jobs application that one is capable of work as data analyst.

This data represetn a tech company found in 1999 focussed on selling tech products online. Customer may buy its products in its own store or by partiners store, which is followed up in this data base.

The data base has nine columns and over 20k lines, which is verry representative of a real world dataset. From this nine columns one represent a metric as the other represent dimensions. 


### 🎯 Framework Steps

### Conceptualize the Data
Before even starting the analysis, it is necessary to know what are the answers that the analyst are looking for or what are the questions that the stakeholder asked and now the analyst are trying to find out. Without knowing this, start the cleaning project is like drive without any destination.

KeyQuestions to keep in mind:

- What is the granularity of the data?

- What are the metrics?

- What are the dimensions?
  
![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/main/imagens/1_cleaning.png?raw=true)
  
### Example Analysis:

Customer 2c06175e places the order 0001328c3c220830 and made the purchase at 24/12/2020. The item was shipped out at 13/12/2020. It was a Nintendo Switch. The item ID was e682 with the value of $168. The purchase was in the website throughout an afiliate. The account creation is unkwon and the country is USA.

From this it is concluded that the primary key in this data is ORDER_ID, the metric attribute is USD_PRICE and the remains are the dimensions.

### 🎯 Locate Solvable Issues
Four Categories:

Often times, during the cleaning phase, the analist will come across four types of issues:

1. Inconsistent data format

2. Inconsistent categorizations

3. Null values (sometimes solvable)

4. Duplicates

### Process:

Here the analyst will first glance throughout the data to check whether there are issues that is visible only by looking. After that, the analyst must apply filter in each column as the column is analyzed. As the analyst find a issue, one must document it in a log tab, documentatios of the process is very important and in the end we gona talk about it too.

The following picture show the issue log tab that was used.

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/main/imagens/2_cleaning.png?raw=true)

After dealing with the filter phase, it is time to check for duplicates rows. There are more than one way to do it, for this I used pivot table:

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/main/imagens/3_cleaning.png?raw=true)

  

### 🎯 Evaluate Unsolvable Problems
Three are three types of "unsolvable" issues that a data analyst myght come across:

1. Null values with no table of truth;

2. Outliers and anomalies;

3. Business logic violations.

Null values is difficult the solve when one does not have a table of truth if the missing information. Note that this is a data analytics cleaning project, therefore imput the missing values with mean, average, mode, or anyother value may bised the data and skew the analysis. Unless it is really necessary to fulfill the missing value is is not up to the analyst to do so. It case likes this what the analyst should check is the magnetude of the missing values. Is it more the 20% of the data? If yes, maybe report it to the stakeholder and wait for feedback.
Outliers as well as anomalies maybe a misstype error or an real event that happened and now is skewed the analysis. Here the analyst must analyze the situation, understand what is going on and work on it. Even if the values is skewing the analysis, if it represent a real world event, the analyst can't remove it.
Finally, the busines logic violation. Here the analyst is better having some background to understand the busines and then check if what is going on on the data makes sense. For example, in this dataset some SHIPPED_OUT values happened before the PURCHASED_DATA. It should never happen, thefore the analyst must document this as well.

### Augment the Data
In this phase new attributes may be create based on the existing attributes of the data. Again, the intention here is not to be fancy on analysis, only to generate columns that may be handy according to the business questions in the particular situation. For this data was created four attribubes to demostrate how it may be done.



### Note and Documentation
Here is the final step of the framework. Here the analyst documents all his work to present to the stakeholder, team or just for future analysis since with this he or she can always come back. 
