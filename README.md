# me-in-texts

This project explores my digital footprint, attempting to better uncover who I am and what my relationships look like based on the largest digital repository of data I have on myself, my text messages.

The main question I am hoping to answer is:

- Has the nature of the communication I have with my online relationships changed over the past decade (ages 12 till 22)?

Some supporting questions that come up in the event to uncover the central answer include:

- Who are the top contacts I've communicated with throughout time?
- Has my communication style changed over the years?
- What individual and group communications drive the bulk of my online interactions?

**Visualization Takeaways**

I found the visualizations and associated analyses to be extremely insightful. It was very fun to work on this project because the dataset was actually just about me and the nature of my own online communications, so I found out more about myself in the process. I also found it to be fascinating how many of the trends and even the anomalies were highly explainable (i.e. differences and similarities across gender or sentiment), proving to be an exciting extension of the more declaratively statistical outcomes we quantified in Project 1 with the same data.

**ML Predictions Takeaways**

This was super fun to build. It is cool that given a particular message, we can now predict the types of reactions it will get. In a way, it's a more concrete addendum to natural language understanding (NLU) where apart from the message text itself, we see that certain factors can play a role in motivating the selection of reactions as qualifiers (i.e. a funny message gets a laugh, an intent for acknowledgement gets a like, etc).

In the future, I wish I was able to get the TF-IDF processing of the messaging that I did (see above) to work as features for the model. The way in which I structured the data (select top k words, have a structured array entry for salient word usage per message) was not a friendly format for BigQuery ML data ingestion, so I abandoned the effort for the sake of time and scope of the project. I think this could even further enhance the results. Something like Word2Vec embeddings would be similar on this front.

Nevertheless, with an AUROC of nearly 0.80, the performance far outdid my expectations, and was a very interesting quantity to predict after jumping through many hoops to wrangle this dataset into a format that enabled ML analyses.

**Overall Takeaways**

To answer my main question, it is clear that my nature of digital communication has indeed changed over time. This was heavily discussed throughout, and now with the ML model, we can almost forecast the future interactions and how they might be perceived even before others have the chance to react to it. I found this to be extremely fascinating, especially with texting to have been a tool and technology I've grown up with, and to this day drives such a large part of my overall interactions, extending the ones I otherwise would have IRL. There's a lot more work that can be done with quantifying nuance from things like inside jokes, deeper emotions like sarcasm or wit, or cleaning the dataset of junk/spam/out of context messages that would otherwise be detrimental to performance, but regardless, the outcome of this work was very interesting and rewarding!
