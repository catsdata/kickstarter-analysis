# Kickstarting with Excel

## Overview of Project

### Purpose
Louise has recently had a kickstarter fundraiser for her play Fever, and would like to compare her results to other kickstarter campaigns.  She would like to see how those campaigns fared in relation to their launch dates and their funding goals. A data file has been provided with approximately 9 years of data on Kickstarter campaigns.  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
On the "Theater Outcomes by Launch Date" sheet, a pivot chart was created based on "Date Created" months; analyzing successful, failed, and canceled campaigns; and filtered down to theater campaigns only.   A filter on Years is also provided should it need to be further narrowed down.   A line chart has been created showing counts along the y axis and months along the x axis.   

![Theater Outcomes by Launch Date](https://github.com/catsdata/kickstarter-analysis/blob/main/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
On the "Outcomes Based on Goals" sheet, counts and percentages of Play only campaigns that were successful, failed or canceled were organized in a table based on Goal ranges in $5000 increments.  A line chart has been added to visualize the percentage of the outcomes along the y axus and monetary goal range along the x axis.  

![Outcomes Based on Goals](https://github.com/catsdata/kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
The following challenges were identified with the provided data file and requested output:  
1. Launch and Ended (Deadline) Dates were initially provided in Unix and had to be converted to standard dates. 
2. Multiple filters were needed within the count formulas requiring compunding countif's
	
The following difficulties were encountered:
1. Human error by inadvertantly creating data points on pledged financials versus goal financials in the goal table
2. Initial percentage formulas received a #DIV/0! error for items with zero counts, requiring the use of an IFERROR formula

## Results

###Outcomes Based on Launch Date conclusions:  
	Failure rates tend to be consistent month by month and not driven by launch date
	The most sucessful theater campaigns are launched between May and July.

###Outcomes Based on Goals conclusions:
	Successful "play" campaigns with less than a $5000 goal make up near half of all play kickstarters
	Goals of $45000 and greater have the highest chance of failure

###Limitations of the dataset:
	The provided dataset has only 4000+ campaigns.  Knowing the popularity of Kickstarter, and that this is global data, we have to 	assume we were provided only a sample dataset.  In the data provided, near 25% of the campaigns were plays.  This does not seem 	reasonable or logical for all global Kickstarters.  The 2009 & 2017 data provided are only a few months a piece and could skew 	monthly/annual results.  In outcomes based on goals - graphing by percentage - outliers are likely making a heavy impact as 	over 96% of plays analyzed are under $25000.  
	
###Other possible tables and/or graphs that may prove helpful:
	Lousie's campaign came close to goal fairly quickly; therefore comparing goals on campaigns with similar lengths of run time may paint a more accurate picture.  
Since we know that most successful play campaigns kicked off in May through July data on goals for plays, a further dive into the details on those campaigns may be needed.
All data is global and not filtered based on country applicable/comparable to Louise's campaign.  More details on her program would be needed to further analyze.
	Outliers in the main data are skewing information.  Statistical analysis to remove outliers in data would be more accurate.  
