![Hero IMG](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20HERO.png)

## INTRODUCTION:

With data analytics, the journey from raw data to actionable insights is often hindered by one crucial step: data cleaning and transformation. Power BI, Microsoft's powerful business analytics tool, is equipped with robust features to shape your data for effective and efficient analysis.  
In this article, we embark on a journey to demystify the art and science of cleaning and transforming data in Power BI. From tackling messy datasets to sculpting them into refined structures primed for analysis, we'll explore the tools, techniques, and best practices that empower data professionals to unleash the full potential of their data.  
Let’s delve into the intricacies of data cleaning and transformation in Power BI, equipping you with the knowledge and skills to navigate the twists and turns of data preparation with confidence and efficiency. 


## TABLE OF CONTENTS:

- [Overview](#Overview)
- [Data Sources](#Data-Sources)
- [Connecting To Files](#Connecting-To-Files)
- [How To Connect To Data In A File](#How-To-Connect-To-Data-In-A-File)
- [File Connection Path](#File-Connection-Path)
- [Data Storage Mode](#Data-Storage-Mode)
- [Lessons Learnt](#Lessons-Learnt)
- [Conclusion](#Conclusion)
- [Reference](#Reference)

##TRANSFORM DATA WITH POWER QUERY EDITOR:

After importing data into your Power BI model, a glance at it within Power BI Desktop reveals a disorganized state: certain data is irrelevant, while essential data is improperly formatted. To rectify this, leveraging Power Query Editor becomes imperative to cleanse and structure the dataset before proceeding with report creation.

![ETL IMG 1](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%201.png)  

To ensure trustworthy and dependable analytics, data necessitates thorough cleansing and preparation. Power Query Editor, integrated into Power BI Desktop, serves as the catalyst for transforming your imported data. With dedicated features geared towards data cleansing and preparation, Power Query equips you with the tools needed for effective analysis. In this article, we'll lead you through a comprehensive, step-by-step guide on shaping your data.  
  
Accessing Power Query Editor is straightforward: simply navigate to the Transform Data option located on the Home tab of Power BI Desktop.  

![ETL IMG 2](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%202.png)  

## STEPS TO SHAPING YOUR DATA:
**Step I:**  
### Columns and Headers  
1. Identify Column Headers and Names
The initial stage of shaping your data involves identifying the column headers and names within the dataset, followed by evaluating their positioning to confirm their correctness.  

![ETL IMG 3](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%203.png)  
The data depicted in the image did not import as anticipated. Upon locating the column headers and names, adjustments can be made to restructure the data accordingly.  

2. Promote headers

To promote headers, you select the "Use First Row as Headers" option on the Home tab.

![ETL IMG 4](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%204.png)  

![ETL IMG 5](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%205.png)  

3. Rename columns
The next step in refining your data involves inspecting the column headers. You may uncover instances where one or more columns possess incorrect headers, there are spelling errors in headers, or the header naming convention lacks consistency or user-friendliness.

There are two methods to rename column headers. One method involves right-clicking the header, selecting "Rename," editing the name, and then pressing Enter. Alternatively, you can double-click the column header and directly overwrite the name with the correct one.  

4. Remove top rows: 
During the process of shaping your data, it may become necessary to eliminate certain top rows. This could be due to various reasons such as blank rows or containing data irrelevant to your reports.

![ETL IMG 6](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%206.png)  

To eliminate these surplus rows, navigate to the Home tab and choose "Remove Rows" then "Remove Top Rows".  

![ETL IMG 7](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%207.png) 


## Conclusion:
enter a relevant text here...

## Reference:  
https://learn.microsoft.com  
https://docs.microsoft.com




## Help and Support

#### Did you find this document helpful? Leave a Star

[![GitHub stars](https://img.shields.io/github/stars/chigozie-i/Data-Transformation.svg?style=social)](https://github.com/chigozie-i/Data-Transformation/stargazers)

#### You may make a contribution to help us improve on our documentation by submitting a pull request.

