Short Answer Questions
1)
1.	What is the difference between stemming and lemmatization? Provide examples with the word “running.”
Stemming is the process of cutting off the end of a word to find its base or root form, often without considering grammar or context. It can sometimes produce incorrect or incomplete words.

Lemmatization, on the other hand, is a more accurate process that uses vocabulary and grammar rules to return the base (dictionary) form of a word, known as the lemma.

Example:
For the word "running":

Stemming gives "run" (correct in this case).

Lemmatization also gives "run", but it works based on grammatical context.

However, for a word like "better", stemming might give "bet", while lemmatization gives the correct lemma "good".

2. Why might removing stop words be useful in some NLP tasks, and when might it actually be harmful?
Removing stop words can be useful in tasks like topic modeling, document classification, or search indexing, where common words (e.g., "the", "is", "and") do not carry important meaning and only add noise to the data.

However, it can be harmful in tasks like sentiment analysis or question answering, where stop words such as "not", "never", or "no" are important for understanding the true meaning of the sentence.

Example:
In the sentence "I do not like this product", removing the word "not" would change the sentiment from negative to positive, which leads to wrong interpretation.


2)

1. How does NER differ from POS tagging in NLP?

Named Entity Recognition (NER)** identifies and classifies named entities in text into categories like PERSON, ORGANIZATION, LOCATION**, **DATE**, etc.

**Part-of-Speech (POS) tagging**, on the other hand, labels each word with its grammatical role in a sentence, such as **noun**, **verb**, **adjective**, **adverb**, etc.

**Example**:  
In the sentence *“Barack Obama was born in Hawaii.”*  
- **NER** tags:  
  - “Barack Obama” → PERSON  
  - “Hawaii” → LOCATION  
- **POS** tags:  
  - “Barack” → NNP (Proper Noun)  
  - “was” → VBD (Verb, past tense)  
  - “born” → VBN (Verb, past participle)

---

### **2. Describe two applications that use NER in the real world.**

**1. Financial News Analysis**:  
NER is used to identify companies, stock symbols, dates, and monetary amounts in financial news. This helps in automated trading and market sentiment analysis.

**2. Search Engines**:  
Search engines like Google use NER to better understand user queries and return more accurate results by recognizing named entities like people, places, or brands.

---

Let me know if you'd like this in Word or PDF format!
