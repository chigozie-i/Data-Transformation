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

4. Remove top rows

During the process of shaping your data, it may become necessary to eliminate certain top rows. This could be due to various reasons such as blank rows or containing data irrelevant to your reports.

![ETL IMG 6](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%206.png)  

To eliminate these surplus rows, navigate to the Home tab and choose "Remove Rows" then "Remove Top Rows".  

![ETL IMG 7](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%207.png)   

5. Remove columns

An essential aspect of the data shaping process involves eliminating redundant columns. It's preferable to discard columns at the earliest stage feasible. One approach to achieving this is by restricting the columns during the data retrieval process from the data source.

There are two methods to remove columns. The initial method entails selecting the desired columns for removal, then navigating to the Home tab and selecting "Remove Columns.".  

![ETL IMG 8](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%208.png)  

Alternatively, you have the option to choose the columns you wish to retain and then, on the Home tab, select "Remove Columns" then "Remove Other Columns."  

6. Unpivot columns

Unpivoting proves to be a valuable feature within Power BI, applicable across various data sources. However, it finds frequent use particularly when importing data from Excel.

Consider the sample Excel document containing sales data below:

![ETL IMG 9](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%209.png)  

Generating a comprehensive total of all sales spanning 2018 and 2019 would pose a challenge. To facilitate the creation of total sales within Power BI, these three columns are required: Month, Year, and SalesAmount.  
  
Upon importing the data into Power Query, it will resemble the following image:

![ETL IMG 10](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2010.png)  

Following that, rename the initial column to "Month." Proceed by selecting the 2018 and 2019 columns, then navigate to the Transform tab within Power Query, and choose the "Unpivot" option.  

![ETL IMG 11](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2011.png)  

The outcome:  

![ETL IMG 12](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2012.png)  


You can rename the Attribute column to Year and the Value column to SalesAmount.  


7. Pivot Columns   
If your data lacks structure, meaning it's flat and lacks organization or grouping, it can hinder your ability to discern patterns within it.

To address this, you can utilize the Pivot Column feature to transform your flat data into a structured table containing aggregated values for each unique value in a column. This feature enables you to summarize data using various mathematical functions such as Count, Minimum, Maximum, Median, Average, or Sum.

For instance, in the SalesTarget example, you may pivot the columns to ascertain the quantity of product subcategories within each product category.

To access this feature, navigate to the Transform tab and select "Transform" then "Pivot Columns."

![ETL IMG 13](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2013.png)  

In the displayed Pivot Column window, choose a column from the Values Column list, such as Subcategory name. Expand the advanced options and pick an option from the Aggregate Value Function list, such as Count (All), then click OK.  

![ETL IMG 14](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2014.png)  

The subsequent image demonstrates the transformation brought about by the Pivot Column feature in reorganizing the data.  

![ETL IMG 15](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2015.png)  


**Step II:**  
### Simplify the Data Structure:

Upon importing data from various sources into Power BI Desktop, the data retains its predefined table and column names. You may find it necessary to modify some of these names to ensure consistency, enhance usability, and provide more meaningful insights to users. Power BI Desktop's Power Query Editor facilitates these name changes, simplifying your data structure in the process.  

1. Rename Query

Within Power Query Editor, navigate to the Queries pane situated to the left of your data. Select the query you wish to rename. Right-click on the query and opt for "Rename." Proceed to modify the existing name or input a new one, then press Enter.

![ETL IMG 16](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2016.png)  

While there is no set rule regarding naming conventions for tables, columns, and values, it is advisable to adhere to language and abbreviations commonly employed within your organization.  A consensus among team members on these conventions fosters uniformity and facilitates effective communication.
Best practice involves assigning descriptive business terms to tables, columns, and measures. Additionally, replacing underscores ("_") with spaces and maintaining consistency in abbreviations and prefixes further enhances clarity and understanding. 

2. Replace Values

The Replace Values feature in Power Query Editor enables you to substitute any value with another value within a designated column. In the example table provided below, within the Attribute column, the month "December" is misspelled. Correcting this error requires selecting the column containing the erroneous value (in this case, Attribute) and accessing the Replace Values option located on the Transform tab.  

![ETL IMG 17](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2017.png)  

Within the "Value to Find" box, input the name of the value you intend to replace. Subsequently, in the "Replace With" box, input the correct value name, and then proceed by selecting "OK."  

![ETL IMG 18](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2018.png)  

3. Replace Null Values

From time to time, you may encounter null values within your data sources. Should these values persist as null, the accuracy of calculated averages could be compromised. One approach to mitigate this issue involves replacing the null values with zero. Following the same procedure outlined for replacing values, you can substitute null values with zero.  

![ETL IMG 19](https://github.com/chigozie-i/Data-Transformation/blob/main/ETL%20IMG%2019.png)  

4. Remove Duplicates

Additionally, you have the option to eliminate duplicate entries from columns, retaining only unique names within a chosen column, by utilizing the Remove Duplicates feature in Power Query. This can be accomplished by selecting a column, right-clicking on its header, and selecting the Remove Duplicates option.
It is advisable to consider duplicating the table before removing duplicates. Doing so enables you to compare the tables and retain both versions if necessary.









## Conclusion:
enter a relevant text here...

## Reference:  
https://learn.microsoft.com  
https://docs.microsoft.com




## Help and Support

#### Did you find this document helpful? Leave a Star

[![GitHub stars](https://img.shields.io/github/stars/chigozie-i/Data-Transformation.svg?style=social)](https://github.com/chigozie-i/Data-Transformation/stargazers)

#### You may make a contribution to help us improve on our documentation by submitting a pull request.

