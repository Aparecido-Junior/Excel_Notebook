# 📘 Excel Nootebook
This repository is a collection of the courses I have been doing since 2024, as well as some projects that I will continue to update. My goal is to share my steps toward becoming a Data Analyst or Data Scientist—or even something in between.

## 🔧 1. Data Cleaning Framework & Documentation
This project is a practical guide and framework for data cleaning in business analytics using Excel. The framework consists of a 5-step process:

- Conceptualize the data (identify granularity, metrics, and dimensions)
- Locate solvable issues
- Evaluate unsolvable problems
- Augment the data
- Note and documentation.


### 📋 Overview
This first Data Cleaning Framework project documents a comprehensive 5-step approach focused on preparing data to answer specific business questions rather than pursuing “perfect” data. The workflow simulates what a data analyst would do in a real business setting.

### 📊 Sample Context
Although the dataset is fictitious, it helps an aspiring data analyst practice real analytics tasks and build a showcase for future job applications. The data represents a tech company founded in 1999 that sells products online. Customers may purchase through the company’s website or through partner stores, and these channels are tracked in the dataset.

The dataset contains nine columns and over 20,000 rows—large enough to resemble a real dataset. From these nine columns, one represents a metric and the rest represent dimensions. The dataset is available on [Christine](https://www.youtube.com/watch?v=y9wFFD2bXQM&t=249s) Jiang’s YouTube channel.

### 🎯 Framework Steps

### 🧠 1. Conceptualize the Data
Before starting the analysis, it is necessary to know what questions the stakeholder is asking or what the analyst is trying to uncover. Without understanding the purpose, beginning the cleaning process is like driving without a destination.

Key questions to keep in mind:

- What is the granularity of the data?

- What are the metrics?

- What are the dimensions?
  
![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/5215fbc2c41e43688a05a320ea71217e2c1fe08a/imagens/1_cleaning.png)
  
### 🔍 Example Analysis:
> Customer 2c06175e placed order 0001328c3c220830 and made the purchase on 24/12/2020. The item, a Nintendo Switch, was shipped out on 13/12/2020. The item ID is e682, and the value was $168. The purchase took place on the website through an affiliate. The account creation date is unknown, and the country is USA.



From this information, it is concluded that the primary key in this data is ORDER_ID, the metric attribute is USD_PRICE, and the remaining attributes are dimensions.

### 🔎 2. Locate Solvable Issues
Four Categories:

During the cleaning phase, the analyst will often come across four types of solvable issues:

1. Inconsistent data format

2. Inconsistent categorizations

3. Null values (sometimes solvable)

4. Duplicates

The analyst begins by scanning the data visually to find obvious issues. After that, filters are applied column by column. As issues are identified, they are documented in a log sheet. Documentation is extremely important, and it will be revisited later in the process.

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/main/imagens/2_cleaning.png?raw=true)

TTo preserve the raw data, the dataset is duplicated into a new tab. The analyst then works on new columns rather than overwriting the original attributes.
![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/0d926ff99d5bb5113602a1afa70df2f528c4cd35/imagens/6_cleaning.png)

After the filter phase, the next step is to check for duplicate rows. There are multiple ways to do this; in this project, a Pivot Table was used.

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/0d926ff99d5bb5113602a1afa70df2f528c4cd35/imagens/3_cleaning.png)

  

### ⚠️ 3. Evaluate Unsolvable Problems
There are three types of “unsolvable” issues that a data analyst may come across:

1. Null values with no table of truth
2. Outliers and anomalies
3. Business logic violations.

Null values are difficult to solve when there is no table of truth. Since this is a data analytics project—not data science—filling missing values with averages, modes, or other estimates risks biasing the data. If the magnitude of missing values is large (e.g., more than 20%), the analyst may need to consult the stakeholder before making decisions.

Outliers and anomalies may represent mistakes or real events. The analyst must investigate the context before removing or modifying any data. If an outlier reflects a real business event, it cannot be removed, even if it skews the analysis.

Business logic violations occur when the data contradicts real-world logic. For example, in this dataset, some SHIPPED_OUT dates occur before PURCHASE_DATE, which should never happen. These issues must be documented clearly.

### ➕ 4. Augment the Data
In this phase, new attributes may be created from the existing ones. The purpose is not to perform advanced transformations, but simply to generate helpful fields based on the analysis needs. In this dataset, four new attributes were created to demonstrate the process.

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/0d926ff99d5bb5113602a1afa70df2f528c4cd35/imagens/4_cleaning.png)

### 📝 5. Note and Documentation
This is the final step of the framework. The analyst documents all the work performed so it can be presented to stakeholders, used by the team, or referenced in future analyses. 

![Image Alt](https://github.com/Aparecido-Junior/Excel_Notebook/blob/0d926ff99d5bb5113602a1afa70df2f528c4cd35/imagens/5_cleaning.png)

### 🏁 Conclusion
n this 5-step cleaning framework project, the CLEAN concept was introduced, explained, and demonstrated. Following this framework ensures that the analyst can deliver clear, structured work and that the next steps—Data Exploration, Transformation, and Sharing—will be achievable.





