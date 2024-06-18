# Cinema-Industry-Analysis
## Table Of Contents
- [Project overview](#project-overview)
- [Data Sources](#data-sources)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results of Findings](#results-of-findings)
- [Recommendations](#recommendations)
- [Limitations](limitations)

  ### Project Overview
  This Data Analysis Project aims to provide insights into  movie trends, audience preferences, box office performance and profitability in the cinema industry. By analyzing various aspects of cinema data, this project seeks to identify trends,make data-driven recommendations and gain a deeper understanding of the industry's performance.
  [Dashboard](Cinemadashboard.png)
  ![image](https://github.com/ChrisAnn609/Cinema-Industry-Analysis/assets/173093556/52fbe4cf-389f-4a9a-8248-1c7d573c8873)

 

  
  ### Data Sources
  The Primary Data set used for this analysis is the "Cinema Data Analysis.xlsx" file containing detailed information about
  - Audience Demographics
  - Box Office Revenue
  - Cast Members
  - Marketing and Prom Campaigns
  - Movie Production Budget and Costs
  - Movie Ratings and Reviews
  - Territory Table.
    
  #### The tools used were:
    - Excel- Data Entry and Collection
    - Power BI- Data Cleaning, transformation and Visualization

    ### Data Cleaning and Preparation
    In the initial data preparation phase, the following tasks were performed:
    - Data loading and inspection
    - Handling missing and duplicate values
    - Data cleaning and formatting

    ### Exploratory Data Analysis
  Exploratory Data Analysis involved exploring the Cinema Data Analysis data to answer key questions such as:
  - Box Office revenue trends over time and by genre?
  - Top rated movie genres and audience preferences?
  - Most popular booking channel per movie genre and age group?
  - Correlations between production budgets, marketing spend and box office performance.
    
  The visualizations used to answer this question included: Slicers, cards, Line charts, Bar charts, Scatter Plots and Pie Charts.
 
    ### Data Analysis
    The following metrics were calculated using DAX formulas:
  
  1- Return On Investment( ROI).
  
  2- Cost per Viewer
  
  3- Revenue per Screen- This formula divides the sum of the total box office revenue and the sum of the number of screens.
  
  #ROI Calculation

The formula used to calculate the Return on Investment (ROI) for movies is as follows:

```
ROI = DIVIDE(
    SUM('Box Office Revenue'[Total Box Office Revenue]) - SUM('Movie Production Budget & Costs'[Production Budget($)]), 
    SUM('Movie Production Budget & Costs'[Production Budget($)]),
    0
)
```
This formula divides the difference between the total box office revenue and the production budget by the production budget. If the production budget is zero, the formula returns zero to avoid division by zero errors.

Cost per Viewer Calculation

The formula used to calculate the Cost per Viewer for movies is as follows:

```
Cost per Viewer = 
  DIVIDE(
    SUM('Movie Production Budget & Costs'[Marketing Budget($)]),
    SUM('Box Office Revenue'[Total Viewers]),
    0
  )
```
This formula divides the marketing budget by the total number of viewers. If the total number of viewers is zero, the formula returns zero to avoid division by zero errors.

### Results Of Findings

- The overall Cost per Viewer is $40.38. This means that, on average, it costs $40.38 to attract one viewer to the cinema for a particular movie.
- The ROI Value for movies was 4, meaning the movie is generating four times the profit compared to its cost. This is a positive sign, indicating that the movie is profitable and has a healthy return on investment.
- For the various Marketing Channels- Billboards, Online Ads, Print Ads, Radio, Social Media and TV, the total marketing budget spent was 726 million dollars each whilst the corresponding Box Office Revenue was over 14 billion dollars.
- The age group 26-35 were the ones who spent majority of their time at the movies; with 23 of the customers being between this age range. 15 of the customers were between the age range 46-60; 14 customers were within the age group 36-45 and 12 customers were within the age group 19-25. The lowest number of audience members were seen from the age range 13-18; recording 5 persons; as these teenagers would more than likely watch movies on their devices at home.
- Customers preferred purchasing cinema tickets online as well as through the Box Office.
- The most profitable movie genre was Action and Adventure, which contributed $6.3 billion dollars to the total box office revenue and the least profitable genre was Comedy, which contributed $ 651 million dollars to total box office revenue.
- Comedy, the genre that contributed the least amount to total box revenue had a neutral sentiment.
- For the genre action and adventure, the sentiment analysis of the movies was mainly a positive one- with a positive sentiment analysis.


### Recommendations
Based on the analysis, the following actions are recommended:
- Focus on Audience Segmentation: Given the variations in audience demographics and preferences, movie offerings, marketing campaigns, and cinema experiences should be tailored to the different audience segments. For example, offer special screenings or promotions targeted at specific age groups or genres that are popular among certain demographics.
- Diversify Movie Offerings: Movie offerings must be diversified in order to appeal to a wider audience, thus can attract new viewers and increase the overall box office revenue.
- Enhance the Cinema Experience: Investing in improving the overall cinema experience to attract and retain audiences, which could include upgrading facilities, offering premium services and amenities.
- Engaging with the Community: Build a strong community presence by engaging with local audiences through promotions, partnerships and events. This will allow for a loyal customer base 
 to be created and will drive word-of-mouth marketing.
- Monitor Box Office Trends: Continuously monitor box office trends and adjust strategies accordingly in order to stay updated with industry trends and competitor activities , allowing one to remain competitive in the market.
- Maximize on ROI: Focus on channels that yield the highest return on investment and tailor campaigns based on audience demographics and preferences.

  ### Limitations
  Some records had to be excluded, as the accuracy of the analysis conclusion would have been affected.









    
 
