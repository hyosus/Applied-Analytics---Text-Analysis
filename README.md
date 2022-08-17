# Applied-Analytics - Text Analysis
The objective of this assignment is to extract and associate various meaningful keywords in the provided dataset of news stories using Bag-of-Word and TF-IDF methods, then analyse them using association rule mining. The text analytic model will be created in Python, and the model will be able to correlate the retrieved keywords from each text to one of the five categories.

### Summary of findings
During the data pre-processing, it was found that the number of documents was not too far off from one another, with ‘sport’ having the most at 511 and ‘entertainment’ having the least at 386.

Bag-of-Words (BoW) and TF-IDF were the two main methods used for transforming of texts. From using BoW, it was discovered that the highest frequency of words were ‘people’, ‘time’, ‘world’, ‘government’ and ‘uk’. And using WordCloud on TF-IDF matrix, it was discovered that the most keywords also include ‘people’, ‘government’ and ‘uk’.

Because of the terms "people" and "government," it is most likely that these keywords fall into the "politics" category. This would imply that in addition to appearing frequently, these terms are also the most significant in their category.

Using association rule mining, it was determined that the keywords 'phone' and ‘mobile,' as well as 'chancellor', 'labour', and 'brown' have a very high confidence and lift, indicating a high possibility of them appearing together as well as a strong significance to the relationship.

### Possible further improvements
Utilizing stemming and lemmatization of the text data prior to the analytics could be an improvement. These text normalization approaches are used in NLP with the aim of reducing word inflectional forms and occasionally derivationally related forms to a single base form.

The words "phone" and "phones", which can be seen in Figure 17 above, were discovered as a result of association mining. These two terms should be considered as one word, ‘phone’, which is the root form of both words, rather than two as it is recognized that they have the same meaning—just one in plural tense. The results of the entire text analysis can then be seen to have significantly improved as a result of doing this.

Another possible improvement is to experiment with more threshold values for association rules such as the Support value. Using a smaller value for Support would allow me to view more keywords and discover interesting relationship between variables.
