# NLP-Sentiment analysis
This is an sentiment analysis repository for hotel reviews(English txt).

Sentiment polarity analysis is a process of analyzing and processing emotional texts. According to the kinds of processed texts, it can be divided into sentiment analysis based on news commentary and sentiment analysis based on product reviews. Among them, the former is mostly used for public opinion monitoring and information prediction, and the latter can help users understand the reputation of a certain product.
At present, there are two main methods of sentiment polarity analysis: sentiment dictionary-based methods and machine learning-based methods.For dictionary-based method, we usually need the following data: sent dictionary and score(Boson NLP), Negative word dictionary, Degree adverb dictionary, Stop word dictionary. The process is very simple, here is an example:
eg： 我非常讨厌害说谎
seg --> 我/非常/讨厌/说谎
非常 adv word ， 讨厌 Negative Word,  说谎 sentiment word

finalSentiScore = (-1) ^ (num of NegativeWords) * degreeword Num * senti word Score
finalScore = sum(finalSentiScore)

In this repository, I choosed the machine learning-based method. The data you need is only the hotel reviews txt.The process is divided into three steps. Simply put, the first: Organize, clean the data, and make a neat format（sent_tag --- review text）, second: Processing text with word2vec(or other word embedding method), finnaly: Reduce dimensionality and choose a machine learning model to fit.


