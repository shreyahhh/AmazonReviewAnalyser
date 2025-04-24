LINK TO THE PUBLISHED PAPER:
https://link.springer.com/chapter/10.1007/978-981-97-8946-7_24

The attached 201 pdf file is the paper I wrote along with my team on this project which got accepted in Springer Conference.

Objective:
This project aims to analyze Amazon product reviews to assess the quality of each review using various metrics and methods to gain a comprehensive understanding of customer sentiments.

Methodology and Key Features:

1. Data Handling:
Loading and Parsing: Reviews are loaded from a JSON file and parsed to extract reviewText, reviewerID, and helpful votes.

2. Metrics Calculation:
Helpfulness Score: Calculated as the ratio of helpful votes to total votes.
Spelling Error Score: Ratio of misspelled words to the total word count using the spellchecker library.
Readability Score: Flesch Reading Ease score scaled to a range of 0 to 1 using the textstat library.
Review Quality: Difference between scaled readability score and spelling error score.

3. Advanced Techniques:
Finding Latest Review: Identifies the most recent review based on reviewTime.
Graph Construction: NetworkX library creates a graph of reviews based on cosine similarity calculated by TfidfVectorizer from sklearn, with edges added above a similarity threshold.
Centrality Measures: Eigenvector centrality, PageRank, and betweenness centrality determine the influence and information flow control of reviews in the graph.

4. Ordered Weighted Averaging (OWA) Scores:
Metrics: OWA at least half normalized, OWA at most half normalized, and OWA as many as possible normalized analyze the central tendency and variability of review sentiments.
Correlation Insights: High correlation between some OWA metrics suggests redundancy, while weak correlation with others indicates unique value.

This project offers a robust approach to analyzing Amazon product reviews by integrating traditional sentiment analysis with supplementary metrics. The multi-metric model provides detailed insights into customer sentiments, aiding businesses in making data-driven decisions based on comprehensive customer feedback.
