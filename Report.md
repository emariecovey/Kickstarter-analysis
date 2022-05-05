# Kickstarting with Excel

## Overview of Project

### This project was an analysis of kickstarter campaign data for Louise, who fundraised on kickstarter for her play. After her kickstarter was completed, she wanted to see how other campaigns turned out. Louise specifically was interested in theater campaign outcomes (successful, failed, etc) based on their launch dates (when the campaign began) and funding goals (amount of money each campaign wanted to raise).  

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

I created a pivot table with months in the rows and outcomes of campaigns in the columns. Then I filtered by theater campaigns, since Louise was interested in comparing other theater campaigns. I then created a line chart from the pivot table. 

![Theater_Outcomes_vs Launch](https://github.com/emariecovey/Kickstarter-analysis/blob/main/Theater_Outcomes_vs%20Launch.png)

### Analysis of Outcomes Based on Goals

I created another sheet to record the number and percentage of play outcomes (successful, failed, and canceled) grouped by goal amounts in categories (less than 1000, 1000-4999, etc.). I used the COUNTIFS() function in excel to filter the data into the numbers of outcomes columns in the new sheet based on the "outcome" column, the "goal" column, and the subcategory "plays" in the original sheet. I used the numbers of outcomes to calculate the percentage of successful, failed, or canceled plays per goal amount category. Then I created a line chart to display the data. 

![Outcomes_vs_Goals](https://github.com/emariecovey/Kickstarter-analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

I didn't have any challenges with the analysis of outcomes based on launch date. However, using the COUNTIFS() function for the analysis of outcomes based on goals did present a greater challenges. The main challenge for me was figuring out how to count in a range (for example, 1000-4999). I knew how to write <1000 and >5000, but I had to figure out how to put >=10000, <=4999. I tried a few more complicated ways of doing it before realizing that you tell excel to look for something greater than 1000 and also less than 4999. I was overthinking the syntax. Once I figured out that part, I was able to get the correct graph. 

## Results

Outcomes based on Launch Date: 

1. The most successful month to launch a campaign is in May. Many people attend theater productions in the summer months, and I would think that summer productions would be fundraising a few months ahead in the spring. Perhaps this is why May is particularly good for fundraising. 

2. The least successful month to launch a campaign is in December. December is a month where many people are purchasing holiday presents and focusing on the holidays in general, and may have less disposable income or time to donate to a kickstarter campaign. 

3. Failed outcomes have a much smaller range than successful campaigns. This lack of great variation over time perhaps indicates that factors other than time are more influential in causing a theater fundraising campaign to fail. There is some small variation, so time is still a factor, just not as influential of a factor as others. 

What can you conclude about the Outcomes based on Goals?

1. The most successful plays were less than $5000, and generally the lower the goal, the better chance for success. There is a chunk of plays with goals between $35,000-$45000 that were very successful as well. Perhaps these larger goal plays were from a few very prominent theaters that needed large budgets, and were well-known enough to get a lot of funding and not be subjected to the lower-the-better trend. 

2. No many plays in any category were canceled. According to [kickstarter.com](https://help.kickstarter.com/hc/en-us/articles/115005138393-How-can-I-cancel-my-project-), campaigns are usually canceled to make large changes to the project, such as the funding goal or campaign duration. Plays either were successful or unsuccessful, so people fundraising for plays must have not needed to rework their ideas after the launch of the campaign. 

Limitations

1. Donors could have theoretically donated outside of the kickstarter fundraiser (donated directly to the person fundraising?), resulting in the donation not being recorded in the dataset. Campaigners could have also lessened the budget for their project after the campaign if they got some, but not all, of the desired funding. Both of these would perhaps push some of the "failed" campaigns to the "successful" category. 

2. The data is from all over the world. There are many factors that result in a campaign being funded or not, and the factors likely change based on  geographic location. There could be outside forces acting in different locations that we aren't aware of. For example, theater is very important in New York City or London, and is likely funded more than other areas. 

What are some other possible tables and/or graphs that we could create? 

1. Do campaigns that have a longer duration have more success? Create a pivot table with length of duration and campaign outcome. This would help Louise see how long an idea campaign should be. 

2. Do campaigns with more backers have more success? Create a pivot table with number of backers and campaign outcome. This would help Louise see if she should focus on the masses or should zero in on a few wealthier backers. 


