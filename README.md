# Instagram-Engagement-Analysis

### Context

Data Analyst Duo is an instagram community (@𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐) of ~104𝐤 data enthusiasts founded by two individuals Aditi & Kalpesh. They share content around statistics, data science & analytics with budding data aspirants.

The goal is to design a data-driven Instagram engagement analysis dashboard to gain insights into the performance of different post types on Data Analyst Duo’s Instagram account and provide recommendations to the duo.

### Actions

We collected the data from the instagram page @𝒅𝒂𝒕𝒂𝒂𝒏𝒂𝒍𝒚𝒔𝒕𝒅𝒖𝒐. We have seven separate spreadsheets of data. We firstly needed to compile the necessary data from sevaral spreadsheets in the excel to a single worksheet. We joined all the necessary columns using VLOOKUP & INDEX-MATCH functions. We replaced the values which are missing aka “#N/A” as zero using IFERROR function.

Data is available from “01-Jan-2022” till “19th-Aug-2023”.The range of date values varies for few columns while the other columns have similar range of date values. So, in order to have everything in one particular scale we have started our analysis from 1st December 2022.

We calculated new metrics such as cumulative_followers which defines cumulative growth of followers each day starting from 1st December 2022 till 19th August 2023. Similarly, engagement_rate which defines how people are engaging with the content i.e. by liking, commenting, saving & sharing the posts. If the engagement_rate of the post is high, there are high chances that growth of followers increases, and it reaches to wider audience.

We compared the metric 3S_view which tells how many people watched IG_Reel for atleast 3 seconds with the metric Impressions which says how many people have watched the reels multiple times and calculated the average 3S_View/Impressions. It is found that more than 50% of the people skipped the content i.e. IG_Reels within 3 seconds. We identified the possible reasons behind it.

Computed the average* (reach, impressions, shares, likes, comments and saves) vs different post_types(IG_Reel, IG_Carousel, IG_Image) using pivot_table and we found the average reach and impression for IG_Reels was high. So, we checked for outliers in reach and impressions column because there could be some posts which would have outperformed others and removed those rows of data because it will inflate our observations.

We determined the average engagement metric(reach, impressions, shares, likes, comments and saves) based on the duration of the reel using pivot_table and found if the duration is less, there are high chances of reaching higher average engagement metrics which will be helpful in attracting wider audience.Lastly, we calculated the % of followers based on age-group,city and country to understand the audience.

Finally we estimated the metrics such as Total Followers, Total Post, Max of Cumulative Followers, Growth_Rate, Total Reach using pivot tables and along with the above calculated metrics we created pivot charts. Using bar chart, we have shown the % of followers based on age-group, city and country and also the average engagements metrics vs the duration of the reel. At last, using line chart we have shown the cumulative growth of followers and cumulative reach per month.

We re-arranged and adjusted the font size and color of all the text boxes, pivot bar/line charts to create a final dashboard. Then, we extracted insights and provided few recommendations.

### Results

