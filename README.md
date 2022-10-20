# NLP
We are going to do the project on SMS SPAM data set from UCI reprository. In NLP we are going to follow the following steps
We use nltk which have all libraries for step1 preprocessing
>>import nltk
>>download()
# 1. TEXT PRE-PROCESSING: in this step we are going to do:
    - Tokenization: we basically divide the paragraph into sentences and then into words by using following statements in python
    >>nltk.sent_token(data_para)
    >>nltk.word_token(data_para)
    - Stopwords: these are those words that do not effect on results for example 'them','for','us',etc. Most of the time we remove these stopwords in preprocessing .In some cases it can be useful.for example Spam classification, Reviews
    >>from nltk.corpus importstopwords
    - Stemming: Process of reducing infected words to their stem words
    >>from nltk.stem.porter import PorterStemmer
    >> ps =PorterStemmer()
    >> [ps.stem(word) for word in review if **not word in stopwords.words('english')]**

- Lemmatization: process of reducing infected words into the meaningful root word. It takes time for exmple: chatbox
>>from nltk.stem import WordNetLemmatizer
>>lemmatizer=WordNetLemmatizer()
   
