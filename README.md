# Unit 12—Tales from the Crypto

![Stock Sentiment](Images/sentimental.jpeg)

## Background

There's been a lot of hype in the news lately about cryptocurrency, so we want to take stock, so to speak, of the latest news headlines regarding Bitcoin and Ethereum to get a better feel for the current public sentiment around each coin.

In this assignment, we will apply natural language processing to understand the sentiment in the latest news articles featuring Bitcoin and Ethereum. We will also apply fundamental NLP techniques to better understand the other factors involved with the coin prices such as common words and phrases and organizations and entities mentioned in the articles.


#### Sentiment Analysis

We used the [newsapi](https://newsapi.org/) to pull in the latest news articles for Bitcoin and Ethereum and created a DataFrame of sentiment scores for each coin.

Using descriptive statistics we wanted to answer the following questions:

> Which coin had the highest mean positive score?
>
> Which coin had the highest negative score?
>
> Which coin had the highest positive score?
> 
>And we found that:
>Bitcoin had a higher mean positive score 
>Ethereum had a higher max compound score of 0.817600
>Ethereum had a higher max positive score of 0.2100

Also while this program was being worked on over a week, Ethereum price was not shooting up in week 1 and sentiment analysis gave different sentiment where Bitcoin and Ethereum were considered about the same; but in week 2 when the ethereum price shot up to all time high of about $3400, it was noted that the ethereum max compound score and max positive score was higher.

#### Natural Language Processing

In this section, we will use NLTK and Python to tokenize the text for each coin. Be sure to:

We created a function to remove stop word, punctuations, including custom words that didn't seem necessary, and then tokenized (which converts a sentence into individual words, and lemmatized it, which gives us root words of the word in the articles. We then converted that to lower case so its easier for the program to understand.  

Next, we look at the ngrams and word frequency for each coin.

1. We used NLTK to produce the ngrams for N = 2.
2. Listed the top 20 words for each coin.

ngrams is combinations between adjacent words then we listed top 20 words
Finally, we generated word clouds for each coin to summarize the news for each coin.

#### Named Entity Recognition

In this section, we built a named entity recognition model for both coins and visualize the tags using SpaCy.

This categorizes words that show up in the article and list them.

---

### Resources

[Vader Sentiment Analysis](http://www.nltk.org/howto/sentiment.html)

---

### Hints and Considerations

The free developer version of the News API limits the total monthly requests, so be careful not to exceed the free limits.
---

© 2020 Trilogy Education Services, a 2U, Inc. brand. All Rights Reserved.
