# Kickstarting with Excel
## Overview of Project
### Purpose
The data presented in the Kickstarter challenge compared products across the world that were hoping to successfully enter the market. Analyzing the outcomes, deadlines, and donations allowed for a more in depth understanding of each product. In order to do so, graphs and formulas were utilized to portray extrapolations from the data.
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
In this section, a new sheet with a chart and corresponding graph were made. My first attempt at this graph was unsuccessful. I had not properly filtered the data to only include the theater category. I also incorrectly placed some fields in the axis rather than the filter. The trouble I had creating this chart allowed me to experiment with the placement of fields in the PivotChart and how it would affect the outcome. Once I cleared the existing filters on the Kickstarter I was able to focus on the theater category. Below is the original chart created that was unfiltered.
![Version 1 - Outcomes based on Launch](https://user-images.githubusercontent.com/71112430/94349891-dc890f00-fffd-11ea-8a2f-20eb905aa787.png)
### Analysis of Outcomes Based on Goals
Forming this new sheet took a lot of careful consideration of the countifs code. There were multiple conditions that had to be met to get the correct number from the code. Since this was one of the longer codes performed in the challenge, my knowledge of the syntax was put to the test. At first attempt, I had difficulties figuring out how to find the numbers between 2 limitations. I thought that there was a maximum amount of three conditions we could put in a countif. I tried to put >=5000 and <=9000 within the same quotations (=COUNTIFS(Kickstarter!$D:$D,">=5000,<=9000",Kickstarter!$F:$F, "failed",Kickstarter!$R:$R, "plays")). This led to an error message that I had to experiment with until finding the correct code. Having the correct code allowed me to quite easily get the data I needed to perform the tasks.
### Challenges and Difficulties Encountered
The primary difficulty with this challenge was with organization. There were many filters that had to be placed in a specific order and if they were done differently the outcome would be significantly changed. The syntax was also important to follow correctly. The error codes could be difficult to understand without having experience with excel codes. There was a lot of trial and error that took up time.
## Results
The outcomes based on launch date chart shows a really big difference between the success and failure in the Summer months. There is a clear peak in success in May and June specifically. The success rates dwindle down during the winter. However, the fail and success rates both spiked in October. It seems that there will always be a percentage of failed shows. While the success rates go up, the failure rates will correspond. This just means that the failures and successes proportionally increase with the total amount of shows launching that month. 

The outcomes based on goals sheet allowed for a clear look at the relationship between the two fields. It showed that the higher the monetary goal, the lower the percentage successful was. The projects that had goals exceeding $10,000 were very minimal. Therefore, the percentage of success or failure was very sensitive to change. While analyzing the data it was very important that I look at all the information rather than just focusing on the percentage failing. If there was a 100% failure rate for a project with a goal between $45,000 and $49,000, I had to make sure to take into consideration that there was only one project that met that criteria. So even if the rate was 100% failure, that does not guarantee that any project that would later on meet that criteria would fail. 

A limitation of this dataset that stands out is the inability to see the big picture. There are so many factors in this sheet that it is difficult to take all of them into consideration. Creating charts and graphs with a narrower goal was the most effective way to come to any conclusions. Another limitation lies in the success and fail labels. The data does not show what conditions have to be met for a product to be considered successful. While analyzing, we have to come up with our own idea of success and that becomes a very subjective analysis.

Creating a chart that compares successful project categories versus countries would be an interesting way to see which industries thrive internationally. This chart could take data from the country, outcome, and parent category fields. From this chart, I could continue analyzing international products by further examining the failing products and compare it to the date it was launched and try to find out why these products didn’t succeed. 
