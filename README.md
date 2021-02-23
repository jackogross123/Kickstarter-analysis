# Kickstarting with Excel
## An Analysis of a dataset of Kickstarter Fundraising Efforts.
### The purpose 
The purpose of the anaylsis was to determine how different factors contributed to the outcome of the fundraising campaign. The four different outcomes of the campaign were successful, failed, cancelled, and live.

## Two Different Analyses 
Louise wanted to know how **fundraiser launch date** and **fundraiser goal** impacted the outcome of the the fundraising campaign. Louise wants to take this information and apply it to her own play, *Fever.*

### Challenge 1: Analysis of Outcomes Based on Launch Date
The purpose of this analyis was to determine if the launch month of Theater fundraising campaigns has any impact on the outcome of the campaign. 

#### Process

To perform this analysis I created a pivot table of the entire Kickstarter data sheet. In the fields, I filtered by Parent Category and Years, added outcomes to the columns, added Months to the rows (Months is a column that I made on the kickstarter sheet to better visualize the data), and added Count of outcomes to the values field.

Once I created the pivot table, I filtered the parent category to only show theater fundraising campaigns (subcatagories of theater include: plays, spaces, and musicals), filtered and sorted the outcomes in descending order to depict include successful, failed, and cancelled, and sort the Months in ascending order.

After the pivot table was filtered and sorted correctly, I added a pivot chart to visually display the data. I added a title to the chart to represent the data correctly. I saved that pivot chart as a .png file and added it to my Kickstarter-analysis repo. I then added the image to my readme.

![Theater_Outcomes_vs_Launch](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

#### Challenges

One of the biggest challanges I had with challenge number 1 was getting my pivot table to sort by months as opposed to the whole date of the fundraising campaign. I solved this issue by adding a "Months" column to the Kickstarter sheet. To find this I used the TEXT formula on the Date Created Conversion column to only depict the abbreviation of the month with "MMM". The formula can be seen in the image below.

![Months_Column_Formula](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Months_Column_Formula.png)

Another challenge I had with this project was figuring out how to upload photos to this readme file. By watching some videos and performing a couple of google searches I was able to solve my issue. As it can be seen in this file, I learned how to insert images.

### Challenge 2: Analysis of Outcomes Based on Goals

The purpose of this analysis was to determine in the goal of the fundraising campaign had any impact on the outcome of the campaign. 

#### Process

To perfrom this analysis I created a new sheet and added the following rows and columns:

![Rows_Columns](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Columns_Rows.png)

After I had my table formated properly, I wanted to count the number of successful, failed, and cancelled Play fundraiser campaigns. I inputted the formula: =COUNTIFS(Kickstarter!D:D,"<1000",Kickstarter!F:F,"Successful",Kickstarter!R:R,"plays").

![Countif_<1000](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Countif_%3C1000.png)

After that I changed the formula for every row to represent the goal range.

![Countif >1000_<4999](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Countif_%3E1000_%3C4999.png)

Once I completed the Number Succesful column, I moved to the number failed column. I had to tweek the formula a little to count the Failed campaigns. The formula for this reads: =COUNTIFS(Kickstarter!D:D,"<1000",Kickstarter!F:F,"Failed",Kickstarter!R:R,"plays"). 

![Countif_Failed](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Countif_Failed.png)

I changed this formula to fill the rest of the "Number Failed" column and then filled the "Number Cancelled" column. I then took the sum of each of the fundraising levels in the "Total Projects" column. Finally, I found the percentage of each of the outcomes for every fundraising level by dividing the the outcome number by the total projects. I then made a line graph with the percentage columns to show the percentage of succesful and failed outcomes at any given fundraising levels. 

![Outcomes_vs_Goals](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)

#### Challenges

The biggest challenge that I had with this challenge was creating the correct countif forumla. I have experience with countifs so I felt a little comfortable going into this part of the assignmen, but it took lots of trial and error. At first, I had troubles with narrowing down the formula to only include plays. Once I figured this out I was still having trouble matching my table with the one provided in the instructions. I then realized that I was only include ">" and "<" in the formulas and not =. I realized that I needed to include greater than or equal to and less than equal to get the correct information. Once I recognized this, I added equal signs to all of the forumals for all levels higher than "Less than 1000." With these corrections I finally matched my table and graph with the sample ones in the assignment instructions. 

## Results
### Theater Outcomes by Launch Date

The first conclusion that I drew from the 1st challenge (Theater Outcomes by Launch Date) is that the most amount of kickstarter campaigns are launched in May. The From the dataset, the most amount of Successful outcomes are seen in the month of May. At first look, I saw that in May the most amount of Successful campaigns were created. May also had the most amount of campaigns started, so I found the percentage of sucessful outcomes for each month and found that May had the highest. Approximently 67% of all campaigns started in May were successful. 

![Percentage_of_Successful_Campaigns](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Percentage_of_Successful_Campaigns.png)

As it can be see from this image, Louise has the best chance of running a successful campaign if she starts it in May. While May also has the highest amount of failed campaigns, the percentage of Successful outcomes out of the grand total is highest in May.

Another observation that can be made from the Theater Outcomes Based on Launch Date graph is that December is the worst month of the year to launch a kickstarter campaign for Theater project. Only 49% of the projects launched in December were Successful.

### Outcomes Based on Goal 

Lots of interesting conclusions can be drawn from the Outcomes Based on Goal chart. First, the highest percentage of successful outcomes fall in the "less than 1000" level. Approximently 76% of the play campaigns with goals less than 1000 were successful. Moreoever, 73% of campaigns with goals between 1000 and 4999 were successful. Following this, goals between 5000 and 34999 have lower success rates. At both the 35000 to 39999 and 40000 to 44999 levels 67% of the kickstarters were successful. 

The worst fundraising level for campaigns was 45000 to 50000 level where only 1 campaign was ran and it failed. The 1000 to 4999 level is interesting because this was the level that the most campaigns were ran. Out of the 534 projects at that level, 73% were successful and 27% failed. Louise should use this information to set her fundraising campaign for her play. I'd reccomend that she sets a goal between 1000 and 4999.

### Dataset Limitations

I think that one of the biggest limitations of the dataset is that there is no information on the fundraisers themselves. I also think that it may be valuable to see the ways that the fundraising was carried out. Data on points of contact as well as how the fundraising was conducted. This may be benefical for Lousie to run the most successful campaign. Lousie could take this information and apply it to her campaign to use the most successful tactics.

### Reccomendations 

I think another chart or graph that should be created in analyzing the amount of donors compared to amount pledged and raised. I believe that it may be beneficial to see this relationship, especially if Louise is interested in garndering wider support as opposed to just fundraising from a few individuals. It may be valuable to also show the average donations compared to the total amount raised. Observe what campaigns have the most successful campaigns based off of average contributions.

