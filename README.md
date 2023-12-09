# Instagram-Engagement-Analysis

Project_link: https://prajivinn.github.io/2023/08/20/Instagram-Engagement-Analysis-Dashboard-Using-Excel.html

### Project Overview

Data Analyst Duo is an instagram community (@𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐) of ~104𝐤 data enthusiasts founded by two individuals Aditi & Kalpesh. They share content around statistics, data science & analytics with budding data aspirants.

The goal is to design a data-driven Instagram engagement analysis dashboard to gain insights into the performance of different post types on Data Analyst Duo’s Instagram account and provide recommendations to the duo.

### Data Dictionary

There are **7** separate spreadsheets of data which contains stats about the channel @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐

**Reach**

* Reach - It shows how many people did our account (@𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐) reached in that particular day.
* Date - It shows the date starting from September 1st 2022 till August 19th 2023.

**Profile Visits**

* Instagram Followers Visit - It shows how many people visited or checked our account (@𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐) in that particular day.
* Date - It shows the date starting from September 1st 2022 till August 19th 2023.

**New Followers**

* New Instagram Followers - It shows how many followers that we gained on this particular day.
* Date - This starts from 21st November 2022 till August 19th 2023.

**Content**

* Post_ID - It shows unique post ID for each instagram post.
* Account_ID - Shows the common ID of the account @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐.
* Account_Username - Shows the Account Name.
* Description - Shows the description of the post. It is basically the caption.
* Duration - Refers to the time in seconds of the post(Instagram Reels).
* Publish_Time - Shows the time when the post is published.
* PermaLink - Refers the Link to the instagram posts.
* Post_type - Refers to the type of the post. We have three types such as IG Carousel, IG Image, IG Reel.
* DATE - Refers to the validity of the post.
* COMMENT - This column is empty.
* Impressions - The number of times your post was viewed. It includes multiple views of your posts by the same accounts.
* Reach - The number of unique accounts that saw any of your posts or stories at least once.
* Shares - The number of times the post was shared.
* Follows - The number of new accounts that started following your Instagram account or the new followers we gained from that particular post.
* 3S Views - How many people watched atleast 3 seconds of the IG reels post. This is a new metric that has been introducted becasue it is a study on instagram that it takes 3 seconds 
  for people to decide whether they want to watch the video completely or not.
* Likes - The number of likes on the post.
* Comments - The number of comments on the post.
* Saves - How many people saved the post.

**Age_Gender**

* Age - Shows the Age of the people.
* Women - Number of Females who follow the instagram page @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐.
* Men - Number of Males who follow the instagram page @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐.

**Top_City**

* Top towns/cities - Shows the cities/towns where the followers are from.
* Value - Displays the total number of followers for each city.

**Top_Countries**

* Top Countries - Shows the country where the followers are from.
* Value - Displays the total number of followers from each country.

### Actions

We collected the data from the instagram page @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐. We have seven separate spreadsheets of data. We firstly needed to compile the necessary data from sevaral spreadsheets in the excel to a single worksheet. We joined all the necessary columns using VLOOKUP & INDEX-MATCH functions. We replaced the values which are missing aka “#N/A” as zero using IFERROR function.

Data is available from “01-Jan-2022” till “19th-Aug-2023”.The range of date values varies for few columns while the other columns have similar range of date values. So, in order to have everything in one particular scale we have started our analysis from 1st December 2022.

We calculated new metrics such as cumulative_followers which defines cumulative growth of followers each day starting from 1st December 2022 till 19th August 2023. Similarly, engagement_rate which defines how people are engaging with the content i.e. by liking, commenting, saving & sharing the posts. If the engagement_rate of the post is high, there are high chances that growth of followers increases, and it reaches to wider audience.

We compared the metric 3S_view which tells how many people watched IG_Reel for atleast 3 seconds with the metric Impressions which says how many people have watched the reels multiple times and calculated the average 3S_View/Impressions. It is found that more than 50% of the people skipped the content i.e. IG_Reels within 3 seconds. We identified the possible reasons behind it.

Computed the average* (reach, impressions, shares, likes, comments and saves) vs different post_types(IG_Reel, IG_Carousel, IG_Image) using pivot_table and we found the average reach and impression for IG_Reels was high. So, we checked for outliers in reach and impressions column because there could be some posts which would have outperformed others and removed those rows of data because it will inflate our observations.

We determined the average engagement metric(reach, impressions, shares, likes, comments and saves) based on the duration of the reel using pivot_table and found if the duration is less, there are high chances of reaching higher average engagement metrics which will be helpful in attracting wider audience.Lastly, we calculated the % of followers based on age-group,city and country to understand the audience.

Finally we estimated the metrics such as Total Followers, Total Post, Max of Cumulative Followers, Growth_Rate, Total Reach using pivot tables and along with the above calculated metrics we created pivot charts. Using bar chart, we have shown the % of followers based on age-group, city and country and also the average engagements metrics vs the duration of the reel. At last, using line chart we have shown the cumulative growth of followers and cumulative reach per month.

We re-arranged and adjusted the font size and color of all the text boxes, pivot bar/line charts to create a final dashboard. Then, we extracted insights and provided recommendations.

### Results

![1694512050561](https://github.com/prajivinn/Instagram-Engagement-Analysis/assets/108303914/14cafe7d-d42c-4b06-9c54-285244b9c48c)

Based on the observations from the dashboard, below are the recommendations suggested to the duo.

* Focus on Strengthening the hook i.e making it attractive or engaging the **IG-Video** reels at the start and also give weightage on the topics/content for the reels such as "Python", "Data Analytics", "SQl", "Statistics", "Interview preparation & questions for SQL/Python/Analyst roles" because as per the observations of the data, it is found that **58%** of the people skip the content within 3 seconds.
* Post **IG-Videos** consistently because it is found that it is performing well interms of engagement and also wider reach can be attained compared to IG Images & IG Carousel. With respect to **Reach and Impressions**, New followers can be gained if they put IG Videos but inorder to **engage the existing audience of the page, the duo should post IG carousel because of high number of Comments and Saves**. So go with IG Videos followed by IG Carousel by posting consistently.

### Growth/Next Steps

Social media feeds (specifically what people/posts you see when you log on) are driven by an algorithm but these can change from time to time. For example, on LinkedIn, there was a time when polls got a huge amount of reach, then it became sharing PDF documents. The algorithm was being changed behind the scenes to up-weight or down-weight certain types of post type.

As of now IG videos/reels, act as better engagement widely in general.

In future, there might be possibilities that they may change the algorithm to favor image posts or some newly discovered post type which can act as better engagement for the users

So keeping this analysis up to date would help the duo keep close to what was working now rather than what worked several months ago.

