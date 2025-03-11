# zomato_resto_sentiment_analysis_-_clustering
## PROBLEM STATEMENT
The Project focuses on Customers and Company, you have to analyze the sentiments of the reviews given by the customer in the data and make some useful conclusions in the form of Visualizations. Also, cluster the zomato restaurants into different segments. The data is visualized as it becomes easy to analyze data at instant. The Analysis also solve some of the business cases that can directly help the customers finding the best restaurant in their locality and for the company to grow up and work on the fields they are currently lagging in. This could help in clustering the restaurants into segments. Also, the data has valuable information around cuisine and costing which can be used in cost vs. benefit analysis
---
## Attribute Information

**Zomato Restaurant names and Metadata**

**Name** : Name of Restaurants
**Links**: URL Links of Restaurants
**Cost** : Per person estimated Cost of dining
**Collection** : Tagging of Restaurants w.r.t. Zomato categories
**Cuisines** : Cuisines served by Restaurants
**Timings** : Restaurant Timings
---
**Zomato Restaurant reviews**

**Restaurant** : Name of the Restaurant
**Reviewer** : Name of the Reviewer
**Review** : Review Text
**Rating** : Rating Provided by Reviewer
**MetaData** : Reviewer Metadata - No. of Reviews and followers
**Time**: Date and Time of Review
**Pictures** : No. of pictures posted with review
---
## EDA Summary:
• College Hyatt Gachibowli is most expensive restaurant with cost more than 2500. rupees
• Mohammedia Shawarma is the cheapest restaurant with average cost of 150 rupees.
• North Indian cuisine is the most served cuisine in the restaurants followed by Chinese and South Indian
• Most of the rating given by the customers are above 3
• Maximum review and orders are coming between the time (12pm - 3pm) and (8pm - 11pm)

## Text Preprocessing
---
Data Preprocessing is the most essential step for any Machine Learning model. How well the raw data has been cleaned and preprocessed plays a major role in the performance of the model. Likewise in the case of NLP, the very first step is Text Processing.

The various preprocessing steps that are involved are:

• Lower Casing

• Tokenization

• Punctuation Mark Removal

• Stop Word Removal

• Stemming

• Lemmatization

● Lower Casing: Converting a word to lowercase (NLP -> nlp). Words like Book and book mean the same but when not converted to the lower case those two are represented as two different words in the vector space model (resulting in more dimensions).

● Tokenization: It is the process of tokenizing or splitting a string, text into a list of tokens. One can think of a token as parts like a word is a token in a sentence, and a sentence is a token in a paragraph.

● Punctuation Mark Removal: The punctuation removal process will help to treat each text equally. For example, the word data and data! are treated equally after the process of removal of punctuations.

● Stop Word Removal: The idea is simply removing the words that occur commonly across all the documents in the corpus. Typically, articles and pronouns are generally classified as stop words.

● Stemming: This is the process of reducing a word to its word stem that affixes to suffixes and prefixes.

● Lemmatization: This is the process of the grouping together of different forms of the same word and converting words into base or root form.

## Sentiment Analysis
---
Sentiment analysis (or opinion mining) is a natural language processing (NLP) technique used to determine whether data is positive, negative or neutral. Sentiment analysis is often performed on textual data to help businesses monitor brand and product sentiment in customer feedback, and understand customer needs. In this project we will try to see the sentiment of the review given by the customers.

Subjectivity: Subjectivity quantifies the amount of personal opinion and factual information contained in the text. Subjectivity lies between [0,1]. The higher subjectivity means that the text contains personal opinion rather than factual information.

Polarity: Polarity score tells us how positive or negative the text is, it ranges between (- 1 to +1) if the score is negative it means sentiment is negative, if score is positive, it means sentiment is positive. If the Polarity score is 0, it means the text is neither positive nor negative but neutral.

## Summary
---

Out of 9,954 reviews:

• 7,478 reviews are Positive (i.e., 75% of total review are Positive)

• 1,887 reviews are Negative (i.e., 19% of total reviews are Negative)

• 589 reviews are Neutral (i.e., 6% total reviews are Neutral)


## Clustering
---
K- Means Clustering:

• The optimal number of clusters were built after visualizing the elbow curve i.e., 5
• Cluster were segmented in terms of the cost and ratings.
