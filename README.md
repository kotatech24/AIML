# AIML
ML
65000 libraries in python
syntax is easy to understand
number of lines of code is 1/3 lines of code we write in Java or C++
open source 
big community to help

Artificial intelligence is possible because of libraries in python

what is AI 
intelligence - anything which learns and improves over time
Artificial intellegence - intelligence mimicing by machine

Machine learning - end goal of machine learning - predictive analytics
subset of AI and its goal is predictive analytics 
eg weather forecasting
ML is good of 2d data - like in excel, RDBMS - Oracle, SQL 

Deep learning - subset of ML
ML has 2 drawbacks - 1. curse of dimentionality - images (RGB pixels 0-255), unstructured data
                     2. feature selection is manual in ML
                        20 yrs data of Haryana in India - humidity, rainfall, temp -> CY
                        number of ph calls farmer made
expensive way - uses GPU

Generative AI
Agentic AI 


NLP
-------------------------------
encompass techniques to analyse human language
this field includes
1. sentiment analysis - positive, negative, neutral 
2. summarization - summarise long text 
3. Keyword extraction - SEO - search engine optimization
                      - social media monitoring

Real time NLP applications 
- chat bots
- text summarization
- text categorization
- parts of speech tagging
- machine translation


Benifits of NLP
--------------------
1. the ability to analyze both structured and unstructured data like speech, emails, social media post
2. improve customer satisfaction
3. understand target market
4. reduce cost - using AI to answer queries

limitations of NLP
-----------------
Ambiguity 
struggle to interpret sarcsam, emotions, context, slang, errors etc
struggle to understand ambiguous 
cultural differences

basic file handling using python
open()

read
write
append 





What is NLP 
==============
Encompasses wide range of techniques to analyse human language.
- sentiment analysis - positive, negative or neutral
- summarization - summarize long texts
- keyword extraction - search engine optimization (SEO)
- tokenization -- break sentence into words so that system can understand vocbulary

NLP benifits
-------------
improve customer satisfaction
reduce cost - automated chatbots
better understand the market
anaylse bith structured and unstructured data

Limitations of NLP
===================
1. Lexical Ambiguity - Single word can mean different things
eg I deposited money in the bank
   I sat by the bank of the river

   The bat flew out of the cave
   he hit the ball with a bat

2. Syntactic Ambiguity - sentence can be parsed in multiple ways
sentence structure allows more than one interpretation

eg I saw the man with a telescope
- I used a telescope to see the man
- I saw a man whi had a telescope

visiting relatives can be annoying
- going to visit relatives is annoying
- Relatives who visit can be annoying


3. Semantic Ambiguity - sentence meaning is unclear due to relationships between concepts
eg Every student read a book

- all the students read the same book
- each student read a different book

4. Pragmatic Ambiguity - (contexts creates multiple interpretation)
eg can you open the window ?
Literal meaning - Asking about the ability
pragmatic meaning - request to open the window

Its cold here
Literal meaning - statement about temperature
pragmatic meaning - turn on the heater/ close the window
-----------------------------------------------------------------------------------------

Install a library called nltk

! pip install nltk
import nltk
nltk.download()

in NLP - Corpus - (Plural is corpora) - is a large collection of text data used to train, test or analyse language

Guterberg - contains books - used for text analysis
- shakespear-caesar.txt
used for word frequency
sentence anlysis
language patters


Stopwords - contain common words - used for cleaning text
WordNet - contains word meanings - used for semantics
Brown - contains tagged text - POS tagging, grammar
- one of the oldest corpus
- contains news, fiction, religion, govt

Movie Reviews - contains reviews - used for sentiment analysis


why corpus are important
---------------------------
1. to train NLP models
2. test algorithms
3. study language patters
4. build chatbots
5. perform setiment analysis
6. do tokenization, stemming, POS tagging


What is tokenization
-----------------------
It is a process of breaking text into smaller meaningful units called tokens such as words, sentences, characters or subwords for NLP processing

tokenization - means breaking text into smaller pieces called tokens

token can be 
- a word
- a sentence
- a character
- a subword (part of word)

I love learning NLP 
["I", "love", "learning", 'NLP']

Why tokenization is needed
----------------------
- count words
- remove stopwords
- find sentiments
- do POS tagging
- train machine learning models

N Grams
-------------
An ngram is a group of consecutive words

Uni-gram - 1 word
bi-gram - 2 words
tri-gram - 3 words
n-gram - N words

google search autocompletion

I want  to drink ........

water - high probability
laptop - low probability

if sentence have m words - total number of n-grams are = m - n + 1

if sentence has 6 words how many bi-grams = 6 - 2 + 1 = 5
tri-grams = 6 - 3 + 1 = 4

------------------------------------------------
stemming
------------------------------------------------
stemming means reduce words to their root/ base form (called a stem)

we replace suffix/ prefix to get root word

playing
played
player
plays

-----> stem - play

connected
connectivity
connection

what humans interpret - connect


why it is helpful
---------------------
1. search engines
2. text classification
3. sentiment analysis
4. Information retrival
5. reduces volcabulary size

3 types of stemmers
-------------------
1. Porter stemmer - balanced (not strict as well not too agressive), most famous commonly used
it can create fake words

2. Lancaster - much more agressive, cuts words harder, fast, strong reduction. problem of overstemming

3. Snowball - improved porter. It is balanced. supports multiple languages


Lemmatization 
----------------
both stemming and lemmatization techniques are used in NLP to reduce
words to a common base form

lemmatization reduces a word to its lemma (dictionary base form) by considering
- meaning
- context
- part of speech (POS)

it uses vocabulary + linguistic Rules

eg running -> run
   better -> good (this answer is aware of context and not just chopping letters)
   studies -> study
   went -> go

how lemmatization works
-------------------------
1. identify part of speech (noun, verb, adjective)
2. uses lexicon/ dictionary
3. Apply morphological analysis

meeting -> noun
meet -> verb

this lemma depends on context


we use lemmatization (understand the tree before trimming ) when
- we need more accuracy
- chatbots, question answering, search engines, sentiment analysis

we use stemming (cutting branches blindly) when
- we need speed
- for large scale systems like  information retrival, search indexing

stop words
-----------
are common words that usually dont carry much meaning 
eg the, is, in, at, and, a, an

why do we need to remove stop words
-----------------------------------
reduce noise
speed up the processing
focus more on meaningful words

eg the cat is sitting on the mat - sentence with stop words
   cat sitting mat -> sentence without stop words

import nltk
nltk.download('stopwords')


NER - Name Entity Recognition
------------------------------
NER is a task in Natural Language Processing where we identify and classify
entities in text into categories like person name, locations, organisation, dates etc

NLTK performs NER in these steps
1. tokenization - splitting text into words
2. POS tagging - identify grammatical roles
3. Chunking (NER) - group words into names entities


what is chunking
------------------
in NLP we group words into meaningful phrases (chunks) like
Noun Phrases (NP)
Verb Phrases (VP)
Prepositional Phrases (PP)

What chunking is not
- it does not understand the full sentence meaning
- it does not find relationship between chunks
- it is not deep parsing

Why chunking is important
----------------------------
to extract key phrases
for chatbots
information extraction
resume parsing











































































































































































































































