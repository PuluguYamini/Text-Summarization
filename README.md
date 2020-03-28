# Text-Summarization

Automatic Text Summarization is one of the most challenging and interesting problems in the field of Natural Language Processing (NLP). It is a process of generating a concise and meaningful summary of text from multiple text resources such as books, news articles, blog posts, research papers, emails, and tweets.

The demand for automatic text summarization systems is spiking these days thanks to the availability of large amounts of textual data.

Through this article, we will explore the realms of text summarization. We will understand how the Text Rank algorithm works, and will also implement it in Python. Strap in, this is going to be a fun ride!

Text Summarization is one of those applications of Natural Language Processing (NLP) which is bound to have a huge impact on our lives. The demand for automatic text summarization systems is spiking these days thanks to the availability of large amounts of textual data. In this project we take a dataset with the interview articles of sportspersons and summarize the big articles into small paragraphs.

The algorithm we use is Text Ranking. We use Extractive Summarization, this relies on extracting several parts, such as phrases and sentences, from a piece of text and stack them together to create a summary. 

Therefore, identifying the right sentences for summarization is of utmost importance in an extractive method.

# ALGORITHM

TEXT RANK ALGORITHM

Let’s understand the Text Rank algorithm, now that we have a grasp on PageRank. I have listed the similarities between these two algorithms below:

In place of web pages, we use sentences
Similarity between any two sentences is used as an equivalent to the web page transition probability
The similarity scores are stored in a square matrix, similar to the matrix M used for PageRank

The first step would be to concatenate all the text contained in the articles
Then split the text into individual sentences
In the next step, we will find vector representation (word embeddings) for each and every sentence
Similarities between sentence vectors are then calculated and stored in a matrix
The similarity matrix is then converted into a graph, with sentences as vertices and similarity scores as edges, for sentence rank calculation
Finally, a certain number of top-ranked sentences form the final summary

