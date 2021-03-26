**Metis Data Science Bootcamp Project 5**

**Sentiment Analysis of Pharma Company Press Releases**

Companies in the pharma industry are doing amazing work, and this is especially apparent in the current COVID-19 pandemic. Laypeople who want to invest in pharma company stocks may have difficulty understanding the technology or the business. Analyzing pharma company press releases for topic (vocabulary words) and sentiment might help laypeople understand the business more, and also understand what constitutes positive versus negative company news.

Features and Target Variables: Text was analyzed, and the target variables were sentiment and change in stock price. The initial idea was to build a model using the text data and sentiment to try to predict movements in the stock prices in the days after the press release. However, the wide differences in date formats, plus the fact that there are not press releases every day, wheras the market is open every business day, results in mismatched data points--there is 'missing' press release data on some days, and marking those days as 'neutral' or zero is not a good solution.

Press releases of companies that had drugs approved by the US Food and Drug Administration (FDA) during that time period 2016-2019 were chosen for analysis. This time period was selected because it is recent, but does not overlap with the COVID-19 pandemic. Press release text was scraped from 10 companies; due to issues with website formatting and date format types, four companies were analyzed. Historical stock price data for these companies was collected using Tiingo.

Tools Used: SciKit-Learn, Pandas, Numpy, Tiingo, Pandas DataReader, NLTK, TextBlob, Seaborn, Matplotlib, Tableau.

Possible impacts: The goal of this project was to build something that might help make pharma press releases more understandable to the layperson. However, the sentiment analysis done using NLTK and TextBlob was not the right one for this use case. This type of highly specialized, technical literature require a tuned, specialized dictionary of words rated as having a positive or negative sentiment to be used as the basis for determining the sentiment of a press release. Further work will incorporate a more appropriate dictionary, and use context, when analyzing sentiment of press release texts.

# 
