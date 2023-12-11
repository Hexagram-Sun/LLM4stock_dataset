## URL
+ https://www.kaggle.com/datasets/miguelaenlle/massive-stock-news-analysis-db-for-nlpbacktests

## Content

+ raw_analyst_ratings.csv

    - Directly-scraped raw analyst ratings

    - Columns are as follows: index, headline, URL, article author (publisher is always benzinga), publication timestamp, stock ticker symbol.

    - Note that all dates on this CSV file don't contain exact hour-minute-second information. If you plan on using this file to backtest (analyst_ratings_processed.csv is better), assume that the article was published the next day instead of the day shown on the current article.

+ raw_partner_headlines.csv

    - Directly-scraped raw news headlines

    - Columns go as follows: index, headline, URL, publisher (NOT benzinga), date, stock ticker. For this CSV, it isn't possible to get exact dates

    - For this CSV, it isn't possible to get precise hour-minute-second timestamps for the dates. Do what is stated for backtesting in the previous note for this CSV too.

+ analyst_ratings_processed.csv

    - Processed analyst ratings

    - Columns go as follows: article title, date, stock

    - Timezone is UTC-4. The difference between this and raw_analyst_headlines is that this has exact dates to the minute vs. raw_analyst_ratings which is only the day without hour or minutes.