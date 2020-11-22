# Kickstarting with Excel

## Overview of Project

### Purpose

The purpose of this analysis is to understand how different components can affect a Kickstarter campaign. With the given information, we can assess how goals, category type, and time can help predict if a Kickstarter will be successful. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

Using the master Kickstarter Excel sheet, I created a Pivot Table to compare outcomes to Launch dates. For the most concise and important data, I used outcomes as the columns and the count of each possible outcome, successful, fauled, canceled, and live, as the values. The months of the launch dates are then used as the rows, and the information is filtered by the category theater and all years. 

Since we are looking at outcomes over months, a line graph is used to compare the different types of outcomes. 

[Outcomes vs Launch Graph](https://github.com/ajg318/kickstarter-analysis/blob/main/resources/Theater_Outcomes_vs_Launch.png)

### Analysis of Outcomes Based on Goals

Along with Launch Date, The size of the goal can potentially play a factor to the success of a Kickstarter. Breaking the goals into buckets ranging from $0 to greater than $50,000, I analyzed the data to see if there is any correlation between the goal amount and outcome for plays. To do so, the function COUNTIFS() was used to determine the percentage of plays were successful, failed, or canceled based on 12 goal buckets. 

Line graphs were again used to compare the percentages for each bucket, as shown in the graph below.

[Outcome vs Goals Graph](https://github.com/ajg318/kickstarter-analysis/blob/main/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

The dataset used was clean before needing any attention. This limited the challenges faced when using it. One challenge I did face was validating the formulas I used. For example, when I was comparing the goals to outcomes, all the buckets had 0% for canceled. I wanted to double check if that was true, so I had to user the master data and filter. It may be difficult to spot check with larger datasets, so I had to go through and make sure the results made sense.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

Two conclusions that can be made about the Outcomes based on Launch Dates are:

1. Spring, particularly in May, appears to be best time to launch a play based on successful data. May does have the most entries out of all the months which can possibly be a reason for the spike. 

2. The winter, most notably December, appears to be the least successful time to launch a Kickstarter. This is based on the successful outcomes data. There is a spike of failed outcomes in October. Once again, this can be in relation to less Kickstarters

- What can you conclude about the Outcomes based on Goals?

According to the outcomes based on goals, campaigns under $20,000 are most likely to be successful based on the percentages. The percentages are also positive from $35,000 to $45,0000, but there are only 9 projects as opposed to the 985 under $20,000.

- What are some limitations of this dataset?

A few limitations to this dataset are:

* The data is already clean, so it is unclear how it was affected.
* The number of projects decrease immensely after about $30,000. This makes projects above that amount less certain than under. 
* This only checks Kickstarter. Louise may have success on another platform or with more information.
* The data only drills down to a certain level. Perhaps knowing different genres of plays can be helpful.

- What are some other possible tables and/or graphs that we could create?

Some more tables and graphs that may be helpful for Louise are:

* Outcome vs. Length of campaign (Deadline - Launch). This can help see how long it may take for a campaign to become successful
* Outcome vs. Average Pledge from each backer or Category vs. Average by Backer. Knowing how many backers are needed or if there are ways to get more out of each backer can help pick demographic to market to.
* Outcome vs. Staff pick. This can help see if it is necessary to become a staff pick to be successful.


