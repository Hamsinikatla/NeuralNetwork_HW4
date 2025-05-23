# Short Answer Questions
# 1Q:

# 1.	What is the difference between stemming and lemmatization? Provide examples with the word “running.”
   
Stemming is the process of cutting off the end of a word to find its base or root form, often without considering grammar or context. It can sometimes produce incorrect or incomplete words.
Lemmatization, on the other hand, is a more accurate process that uses vocabulary and grammar rules to return the base (dictionary) form of a word, known as the lemma.

Example:
For the word "running":
Stemming gives "run" (correct in this case).
Lemmatization also gives "run", but it works based on grammatical context.
However, for a word like "better", stemming might give "bet", while lemmatization gives the correct lemma "good".

---

# 2. Why might removing stop words be useful in some NLP tasks, and when might it actually be harmful?
   
Removing stop words can be useful in tasks like topic modeling, document classification, or search indexing, where common words (e.g., "the", "is", "and") do not carry important meaning and only add noise to the data.
However, it can be harmful in tasks like sentiment analysis or question answering, where stop words such as "not", "never", or "no" are important for understanding the true meaning of the sentence.

Example:
In the sentence "I do not like this product", removing the word "not" would change the sentiment from negative to positive, which leads to wrong interpretation.

---
---
# 2Q:

# 1. How does NER differ from POS tagging in NLP?

Named Entity Recognition (NER)** identifies and classifies named entities in text into categories like PERSON, ORGANIZATION, LOCATION, DATE, etc.

Part-of-Speech (POS) tagging, on the other hand, labels each word with its grammatical role in a sentence, such as noun, verb, adjective, adverb, etc.

Example:  
In the sentence “Barack Obama was born in Hawaii.”  
- NER tags:  
  - “Barack Obama” → PERSON  
  - “Hawaii” → LOCATION  
- POS tags:  
  - “Barack” → NNP (Proper Noun)  
  - “was” → VBD (Verb, past tense)  
  - “born” → VBN (Verb, past participle)

---

# 2. Describe two applications that use NER in the real world.

1.FIinancial News Analysis:  
NER is used to identify companies, stock symbols, dates, and monetary amounts in financial news. This helps in automated trading and market sentiment analysis.

2. Search Engines:  
Search engines like Google use NER to better understand user queries and return more accurate results by recognizing named entities like people, places, or brands.

---
---

# 3Q:

# 1. Why do we divide the attention score by √d in the scaled dot-product attention formula?

We divide by √d (where d is the dimension of the key vectors) to prevent extremely large dot-product values when the dimensionality is high.  
Without this scaling, large values can push the softmax function into regions where it produces very small gradients, making the model harder to train.  
So, dividing by √d keeps the values in a stable range and improves training efficiency and numerical stability.

---

# 2. How does self-attention help the model understand relationships between words in a sentence?

Self-attention allows the model to compare each word with every other word in the sentence, assigning attention scores based on how related they are.
This helps the model:
- Understand context (e.g., in “bank of the river,” self-attention helps disambiguate “bank”).
- Capture long-range dependencies (e.g., connecting subjects and verbs that are far apart).
- Create richer word representations based on the entire sentence rather than just local surroundings.

In short, self-attention enables the model to focus on relevant words, no matter where they appear in the sentence.

---
---

# 4Q:

# 1. What is the main architectural difference between BERT and GPT? Which uses an encoder and which uses a decoder?

BERT (Bidirectional Encoder Representations from Transformers) uses only the encoder part of the Transformer architecture. It is bidirectional, meaning it looks at both the left and right context of a word.
GPT (Generative Pre-trained Transformer) uses only the decoder part of the Transformer. It is unidirectional, processing text from left to right, which is ideal for text generation.

BERT → Encoder-based (bidirectional, great for understanding)
GPT → Decoder-based (unidirectional, great for generating)

---

# 2. Explain why using pre-trained models (like BERT or GPT) is beneficial for NLP applications instead of training from scratch,

Using pre-trained models is beneficial because:

- Saves time and resources: Training from scratch requires massive data and computational power. Pre-trained models have already learned language patterns from large corpora.
- Improves performance: These models capture deep semantic and syntactic information, leading to better results on tasks like classification, translation, or question answering.
- Easy fine-tuning: You can adapt them to specific tasks with minimal data and training.

In short, pre-trained models provide a strong foundation and reduce the effort needed to build effective NLP systems.



