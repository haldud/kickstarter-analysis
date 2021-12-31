# Kickstarting with Excel

## Overview of Project
Louise is fundraising for her play titled *Fever*. We have been analyzing data from several thousand other crowdfunding projects to find trends and to identify usefult insights. The analysis will be provided to Louise to help her make decisions in her quest to reach her fundraising goals.

### Purpose
The most recent update we have from Louise is that her play *Fever* came close reaching the goals in a short amount of time. We will be comparing how other campaigns performed relative to the following two factors:
1. Launch date - can we uncover any trends as it relates to a launch date of a kickstarter?
2. Funding goals - does the fundrasing goal seem to have an impact on the success of a campaign?

## Analysis and Challenges
We performed our analysis with Microsoft Excel. Excel is an extremely powerful tool for analyzing data containing approximately less than one million rows. Our data set of kickstarter data contained just over 4,000 rows so Excel was the perfect tool to find valuable information for Louise.

The kickstarter spreadsheet that we have been analyzing can be downloaded from here: [Kickstarter](https://github.com/haldud/kickstarter-analysis/blob/main/Kickstarter_Challenge.zip)

Below are charts that we created in Excel that show trends related to launch date and funding goals.

### Analysis of Outcomes Based on Launch Date
![Theater Outcomes based on Launch Date](https://github.com/haldud/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals
![Theater Outcomes based on Goals](https://github.com/haldud/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered
Overall this project went very smoothly. One of the stumbling blocks that I encountered was understanding the parameters for the COUNTIFS function in Excel. I did not include the second parameter in double quotes initially. For example, I was attempting to use:

  =COUNTIFS(Kickstarter!$D:$D, <1000, Kickstarter!$F:$F, "successful", Kickstarter!$R:$R, "plays")

The <1000 needed to be in quotes like this: "<1000"

## Results
Here are our conclusions that we have been tasked to answer according to the launch date and funding goals.

1. May significantly stands out as the month with the most successful campaigns (111). May is also tied with October for the most failed campaigns (52). We need to pay a little closer attention to determine if May is the ideal month to launch a campaign. May does turn out to have the highest chance of a successful campaing with 67%. The months of June and July have the second and third highest chances of succeeding with 65% and 63%, respectively. The month of December has the worst chances with 49% succeeding. All of the other months have at least a 57% chance of succeeding.

2. When first looking at the outcomes based on goals chart it seems somewhat challenging to make definite conclusions as to how fundraising goals affect affect the percentage of succeeding due to the seemingly good outcomes for campaings in the $35K to $45K range. Overall, the outcomes seem to be much better for campaings with very small goals. About 75% of campaings are succeeding with campaigns whose goals are less than $5,000. On the spectrum, campaings with very large goals ($45K or more) look to have the worst chance of succeeding with about a 13% success rate.

One of the limitations that I encountered when analyzing the outcomes based on goal data was the lack of campaings with fundraising goals over $25K. It would have been good to see more examples in that range in order confirm that campaigns with smaller goals have a better chance of succeeding. One of the other dataset issues that we did not address was the matter of currency conversion. The spreadsheet contains data with multiple currencies and we treated all of the goals in US dollars instead of converting the goal in the local currency to US dollars.

There are a few other columns in the kickstarter dataset that we did not focus on, but could perhaps also provide some insights. We could have drawn a line char to determine if the campaign duration affects the chance of succeeding. Also, can we find any insight based on country? If Louise is flexible in where she launches her campaign then generating a bar graph to show successful vs unsuccessful campaigns by country could also be beneficial. In addition, there are some other columns that were not discussed such as "staff_pick" and "spotlight". It would have been important to identify what those represented and if they impact the chance of success.
