import snscrape.modules.twitter as sntwitter

query = "象印 lang:ja"
tweets = []
for tweet in sntwitter.TwitterSearchScraper(query).get_items():
    tweets.append(tweet.content)
