# Kickstarting with Excel
## An Analysis of a dataset of Kickstarter Fundraising Efforts.
### The purpose 
The purpose of the anaylsis was to determine how different factors contributed to the outcome of the fundraising campaign. The four different outcomes of the campaign were successful, failed, cancelled, and live.
## Two Different Analyses 
Louise wanted to know how **fundraiser launch date** and **fundraiser goal** impacted the outcome of the the fundraising campaign. Louise wants to take this information and apply it to her own play, *Fever.*
### Challenge 1: Analysis of Outcomes Based on Launch Date
The purpose of this analyis was to determine if the launch month of Theater fundraising campaigns has any impact on the outcome of the campaign. 

To perform this analysis I created a pivot table of the entire Kickstarter data sheet. In the fields, I filtered by Parent Category and Years, added outcomes to the columns, added Months to the rows (Months is a column that I made on the kickstarter sheet to better visualize the data), and added Count of outcomes to the values field.

Once I created the pivot table, I filtered the parent category to only show theater fundraising campaigns (subcatagories of theater include: plays, spaces, and musicals), filtered and sorted the outcomes in descending order to depict include successful, failed, and cancelled, and sort the Months in ascending order.

After the pivot table was filtered and sorted correctly, I added a pivot chart to visually display the data. I added a title to the chart to represent the data correctly. I saved that pivot chart as a .png file and added it to my Kickstarter-analysis repo. I then added the image to my readme.

![Theater_Outcomes_vs_Launch](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Theater_Outcomes_vs_Launch.png)

One of the biggest challanges I had with challenge number 1 was getting my pivot table to sort by months as opposed to the whole date of the fundraising campaign. I solved this issue by adding a "Months" column to the Kickstarter sheet. To find this I used the TEXT formula on the Date Created Conversion column to only depict the abbreviation of the month with "MMM". The formula can be seen in the image below.

![Months_Column](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Months_Column.png)

### Challenge 2: Analysis of Outcomes Based on Goals

![Outcomes_vs_Goals](https://github.com/jackogross123/Kickstarter-analysis/blob/main/Resources/Outcomes_vs_Goals.png)
