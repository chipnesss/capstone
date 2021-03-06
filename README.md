# Tableau Public Link
## [Risk Analysis Dashboard](https://public.tableau.com/views/RiskAnalysisDashboard_16196460921210/PortfolioAnalysisDashboard?:language=en&:display_count=y&publish=yes&:toolbar=n&:origin=viz_share_link)  
  --- 
# Building risk analysis systems for portfolio management

While it is currently a WIP, feel free to take a look at the projects tab to see how far into the project I am.

# Portfolio risk analysis script and dashboard.

This project was sparked from a need to be able to analyze investment assets at a glance, in order to identify potential situations where a portfolio may be taking on too much downside risk according to the portfolio’s goals. Can I create a system that can run with up to the minute data in order to give me the overall health of my portfolio? If I were to do that, it would be in a dashboard format that I could run indefinitely. It would automatically update based on trades and changes to the portfolio that I make within TD Ameritrade, and give me information to help me make informed decisions without having to manually run complex calculations. The data would be from the TD Ameritrade API, and so it would be constantly updated, but not live streamed data. Potential issues would be accessing the API, potentially delayed data, TD Ameritrade’s services not operating as anticipated on their end, and getting the application to run autonomously. 

### Over all view of the dashboard
![Base Design](assets/image.png)

### Tooltip: Account Balance and Account Beta
![Account Total and Beta Tool Tip](assets/image3.png)

### Filter by and analyze Beta.  These data points show additional bits of info needed for quickly making decisions
![Beta Tool Tip](assets/image2.png)

### Tooltip: Scrolling over news summaries will give you a quick and easily consumable version of the article
![News Tool Tip](assets/image4.png)

### Quickly change the chart and select which stock you are analyzing based on the symbol
![Symbol Search](assets/image5.png)

### Tooltip: Hovering over the 1 Minute chart will show more information about the time, stock price, and percent change.
![1 Minute Chart](assets/image6.png)

### Review the weight and beta of flagged positions
![Weight & Risk](assets/image7.png)

### Filter by and analyze the % P/L Day.
![% P/L Day](assets/image8.png)

# Motivation

My motivation for this project stems from a drive to be able to quickly and accurately analyze my family’s assets in order to protect from accidentally taking on an unreasonable amount of downside risk, based on the portfolio’s goals.

# Answering the Questions
 
Can I develop a program that will identify elevated risk levels across my portfolio?
If so, can that same program convey that information to me in a concise and meaningful way?

# Minimum Viable Product

#### The Minimum Viable Product required to answer this question would have the following elements:
- Ability to contact and pull data from the TD Ameritrade API
- Ability to pull up to date account data to identify positions, quantities, and data on those positions
- Calculations to analyze both individual account positions and the portfolio risk as a whole. 
- Ability to update based on trades and new equity positions
- Dashboard displaying:
  - Account Value
  - Individual Position Risk Levels
  - Overall Portfolio Risk Levels
  - Perhaps a sliding scale chart or number system
  - Top 3 Daily Gainers
  - Top 3 Daily Losers

# Stretch Goals
- Pulling news articles based on current portfolio holdings
- Morning/Evening email updates regarding any known risk issues
- Live stream data flow

# Data Sources
This project will pull data from the [TD Ameritrade API](https://developer.tdameritrade.com/apis) service, along with the [Yahoo Finance API](https://rapidapi.com/apidojo/api/yahoo-finance1)

# Known Issues and Challenges
- Working with TD Ameritrade API to pull up to the minute data. 
- Ideally getting the data to automatically propagate on a timer/constant basis so it feels like live data.
