**Financial News**: In this project, I scraped financial news websites from CNBC using  BeautifulSoup to collect all the headlines on the page at the moment of performing the requests. I Saved the timestamp of my extraction
**Stock Market Data**: I also used Alpha Vantage API to extract stock market data to get historical stock prices for the following companies:
•	Apple
•	Microsoft
•	Google
•	Amazon
•	Meta
I have removed the Alpha Vantage API I used for security and privacy reasons.
**Transformations:** I performed sentiment analysis on the headlines from CNBC using Spacy and saved the polarity scores in a new column called sentiment_scores. I created a new column called sentiment and classify the sentiment scores as positive, negative and neutral:
The sentiment scores between -1 and -0.2 were classified as negative, those between -0.2 and 0.2 were classified as neutral, and else positive.

**Relevant Words**: I used word tokenizer from nltk.tokenize library to find the relevant words in each headline and stored them in a column named relevant_words
**Save and Loading Data in SQLite**: I saved the data from the scrapped headlines into csv files called headlines_data.csv and stocks_data.csv. I created two tables for loading the headlines and stocks data. Wrote sqlite code to store the data from the CSV files into created tables in the SQLite database
