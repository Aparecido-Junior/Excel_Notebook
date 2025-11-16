# Excel Nootebook
This repository is a collection of the courses that I have been doing since 2024 as well as some projects that I will be updating. My goals is to share my steps towards my goal which is beccome a data analyst or data Scients or even something in between. 

## 1. Data Cleaning Framework & Documentation
A practical guide and framework for data cleaning processes in business analytics using excel.

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
  
![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/main/1_pic.png?raw=true)
  
### Example Analysis:

Customer 2c06175e places the order 0001328c3c220830 and made the purchase at 24/12/2020. The item was shipped out at 13/12/2020. It was a Nintendo Switch. The item ID was e682 with the value of $168. The purchase was in the website throughout an afiliate. The account creation is unkwon and the country is USA.

From this it is concluded that the primary key in this data is ORDER_ID, the metric attribute is USD_PRICE and the remains are the dimensions.

### Locate Solvable Issues
Four Categories:

1. Inconsistent data format

2. Inconsistent categorizations

3. Null values (sometimes solvable)

4. Duplicates

Process:

Quick scan of data

Attribute-by-attribute analysis using filters

Document all issues in an issue log

Prioritize by impact and solvability

### Evaluate Unsolvable Problems
Three Types:

1. Null values with no table of truth

2. Outliers and anomalies

3. Business logic violations

Approach:

Keep real outliers as they represent actual events

Validate business logic (e.g., ship date after purchase date)

Accept unsolvable nulls when no reference data exists

### Augment the Data
Create new attributes from existing data

Focus on columns useful for specific business questions

Avoid unnecessary complexity

### Note and Documentation
Maintain comprehensive documentation throughout the process

Track all changes and decisions

Create reproducible cleaning procedures

🔧 Implementation Strategy
Best Practices
Always duplicate original data before cleaning

Create new columns instead of overwriting original data

Use pivot tables or other methods to identify duplicates

Maintain an issue log for tracking problems

When is Data Ready?
"The data is ready when the modifications applied are enough to answer the business questions proposed."



Multiple sales channels and platforms

Diverse customer base and marketing approaches


