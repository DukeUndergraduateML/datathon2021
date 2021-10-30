# datathon2021: Asian Barometer Survey (ABS)

This repository contains information for Datathon2021, which is on the Asian Barometer Survey (ABS), where extensive information can be found here at 
http://asianbarometer.org/

## Instructions

Welcome to Datathon 2021! 

1. The dataset can be found at dukeml.org/dataset and the password to the file will be provided at 10:30am on Saturday, November 6, 2021 via email and Slack. Please download the dataset as soon as possible to prevent potential network issues on Duke’s wifi!

2. Submissions will be due at 10:30 AM on Sunday, November 7, 2020 at Microsoft CMT (https://cmt3.research.microsoft.com/User/Login), and projects will be judged on the rubric that is found in the documentation folder. Specifically, we are looking for high quality submissions that answer the challenge question provided below, which are presented in a clear, statistical correct and sound manner (with support via vizualizations and citations from books or literature). 

3. In your submission, you have four pages to present the most important findings to the reviewers, with an optional two page appendix. Your submissions will be reviewed by at least two reviewers of either faculty/graduate students who will asess the quality of your work through peer review and provide constructive comments back to you. You must submit reproducible code in order for your submission to be considered. Please submit just on zip file to the CMT webpage, and have your group leader submit this on behalf of your group (up to four individuals). 

4. Top submissions will receive recogition from the Duke Undergraduate Machine Learning Board as well as a prize. These will be decided upon by the reviewers as well as area chairs that will also review the work. 

5. You are welcome to get help from mentors at the event and ask questions of the organizers. You are encouraged to talk to other groups as well. The overall goal of this event is to learn how to analyze data in a fun setting and hopefully make friends. There are workshops that will be held in case you are new to statistical machine learning, so please check these out. 

Finally, the event is hybrid this year in case you don't feel comfortable being around others. If you do come to the event, please rememeber to follow all Duke COVID-19 protocols and mask up, Duke. We have reserved space around campus so that students can work in small groups as well. 

## Components of Submission

Teams must write a report that describes the steps taken to answer their proposed question/prompt. There is no set format for how the report should be written, but example sections of the report can include, but are not limited to, the following:

1. Introduction: What question are you answering with the data, and why is it important?
2. Prior Work/Literature Review: What is the current literature in this area in a few sentences regarding references that you're utilizing. It's important to cite any work that you are using if it's not your own proposal as this is best practice. 
3. EDA: How did your EDA help motivate your proposed methods? (This could be put in the appendix and be referenced in the main document). 
4. Proposed Methodology: What are the main method(s) that you are using and why? Be sure to choose methods that are appropriate for the data. State any assumptions and why they are valid. 
5. Analysis: Analyze your data and provide evaluations. What do you find (include visualization if helpful). 
6. Conclusion: What can you conclude from your analysis and how is this useful regarding the motivating question. 
work?

At minimum, the report must include the question being answered, findings and visualizations, and a conclusion. Your report may not be longer than 4 pages in length. You may have an optional appendix (maximum 2 pages), however, this may not be read by the reviewers. From the report, it should be clear as to how you approached your analysis. Do not include any identifying information about the members of your group in the submission. Please submit your written report as a .pdf document.

## What is the mission of the ABS?

The ABS has three main objectives, which we repeat exactly from their webpage to help student understand their mission.

1. ``To generate a region-wide base of scientifically reliable and comparable data."

``Public opinion data on issues such as political values, democracy, governance, human security, and economic reforms were gathered through face-to-face interviews with randomly-selected pools of respondents that represent the adult population of the country in question. By insisting on strict research standards, we seek to ensure that are data is trustworthy and accurate."

2. ``To strengthen intellectual and institutional capacity for research on democracy."

``The network fosters mutual exchange of expertise by bringing partners and scholars together for planning and analysis at the national, continental, and global levels."


3. ``To disseminate survey results to academics and policy circles."

``We continually strive for the consistent presentation of our survey results. Using the Globalbarometer Survey (GBS) report as our model, we distribute our data to a wide variety of individuals and organizations, including decision makers in legislative and executive branches of government, policy advocates and civic educators, journalists, academic researchers, international investors, and NGOs concerned with democratic development."

- Reference: http://asianbarometer.org/

## Question of Interest: ABS, Waves 1 and Waves 2

Given one of the motivating questions of interest, build a predictive model for at least one wave to help the ABS' objective. Be sure to conduct an exploratory data analysis, choose a model that is appropriate for the data at hand, and explain any assumptions that you make. In building your model, be sure to pay attention to the priority variables in the documentation folders. 

Suggestions regarding talking points and plans of work:

0. Choose a group leader, especially that might have experience with this type of data. 
1. Perform an exploratory data analysis such that you understand what type of data you have. Is it continuous, discrete, categorical, or mixed? Given the data, what types of models are appropriate? 
2. Start out in a simple way. For example, start with wave 1 and with one country to get a feel for the data set before generalizing. 
3. Choose simple models before overly complex models (and make sure that these models are appropriate for the data). Be sure to account for missingness of any data in a statistically sound way. 
4. What conclusions and guidance can you provide to the ABS for future guidance? 
5. Be sure to include your code in your report. 

Remark: If you can build a predictive model across both waves for all countries, this would be a top-notch project! 

## Getting started in R 

The code below illustrates how to load in the wave 1 dataset from Thailand using R.

```
data <- read.spss("data/Wave.1_Data/Thailand/thailand v4.2.sav", 
                  to.data.frame=TRUE)
attach(data)
data %>%
inspect_types()
```

### :card_index_dividers: Folder descriptions

- **key-variables**: This is a folder describing key varaibles of the first two waves.
- **documentation**: This is a document provided by the ABS regarding the survey/questionaire.
- **rubric**: This is a document that provides the rubric for the event 






