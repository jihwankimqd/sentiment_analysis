# Edit 25/08/2020
Upon more thought, there seemed to be no meaningful value in continuing this project. The project delivers no value and the methods in sampling and processing data is flawed along with the model training part. On the bright side, I learnt a lot regarding project development from this project.

# News Scraper and Sentiment Analysis of News Headlines

Headlines of news articles from Google News are scraped and analysed using VADER. The sentiment scores for individual articles for a single date is then averaged to give
an average score for the respective date. The average score for each dates are then compared with the price change of the stock and a classification model (SVM) is trained.
In the first attempt, the score of the model was only 22.2%. 

SK Innovation (096770) is used as a reference, and the date range for the stock and news collection is from 01/07/2020 to Today (live date using Python datetime lib). 
The reason SK Innovation was chosen as a reference is because of its sudden fluctuation (increase) in price on early August, and a few articles implicitly indicated that the company's
stock price would rise due to a rise in the EV market (and to my surprise, the price jumped (very high) a few days later), which inspired me to create this program.

# Running the code

Download the repo and run the ipynb file step by step from the top. It may take a long time to scrape the news articles if the date range is large. 
