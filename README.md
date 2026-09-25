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



Machine learning - is all about predictive analytics
we must have data in 2 Dimention (rows Vs columns)

- feature selection is manual - we need to select columns manually

humidity/ rainfall/temp/ farmer ph calls -> crop yield


Deep learning  - can predict on multi dimentional data
image (RGB) , video, audio, text

feature selection is automatic


=======================================>

Image Augmentation
===================
Image augmentation is the process of creating new training image from existing 
images by applying transformation while preserving the original class label

eg imagine we have one image of cat
from the same image we can create multiple images of cat by
- rotate - rotating by certain degrees
- flip - horizontal flip (left right orientation)
- zoom - zoom in zoom out
- Brightness - introduce cloudy theme, night
- Noise
- crop
- shift - move image to left/ right/ up/ down in same frame
- shear - rectangle and parallelogram -simulates viewing onbject from different angles

why augmentation is needed 
---------------------------
suppose we have only 100 images of dogs
without augmentation 
100 images -> CNN -> learn only those 100 images

in the testing dataset - if we rotate dog image by 30 degree
model will fail as it have never learnt from that kind of image

Benifits of image augmentation
------------------------------
create additional training examples
reduces overfitting
better generalization - improves performance on unseen images
handles real world variations
better accuracy


when to use augmentation
-------------------
1. small datasets
2. medical imaging where we need more accuracy
3. sattelite images
4. face recognition
5. object detection
6. image classification

when should we avoid augmentation
----------------------
handwritten digits - 6 if you rotate to 180 degree it becomes 9

CIFAR 10 Dataset
-----------------
total images - 60,000
training images - 50,000
testing images - 10,000
number of classes - 10
image per class - 6000
training images per class - 5000
testing images per class - 1000
image size - 32 X 32 pixels
color - RGB

labels 
0 - Airplane
1 - Automobile
2 - Bird
3 - cat
4 - Deer
5 - Dog
6 - Frog
7 - horse
8 - ship
9 - truck

per image size is (32 X 32 X 3)

-------------------------------------

R-CNN (Region Based Convolutional Neural Network)

a deep learning algorithm used for object detection. Unlike image classification (which predicts one lable for entire image)

this answers - where object is present, where they are located

imagine image has Dog, car and a person

R-CNN first finds possible regions that might contain objects

Region 1 - person
Region 2 - dog
Region 3 - Cat
..
...
2000 regions

each region is then passed to CNN seperately 

steps of R-CNN
----------------
1. input image
2. Region proposal - An algorithm called selective search proposes approx 2000 regions
3. Resize every region - CNN requires fixed size inputs therefore each region is resized
4. CNN feature extraction - each resized region is passed to CNN and features are created
5. Classification - A classifier predicts the object category 

Man - 99%
dog - 0.2%
..
...
6. Boundary box regression - The proposed box may not fit the object precisely, boundary box
regression adjusts it


complete pipeline
-------------------
image -> selective search -> Resize -> CNN ->feature extraction -> SVM Classifier ->Boundary box regression -> final detection

Advantages of RCNN
----------------------
very accurate compared to earlier object detection methods
determine multiple objects in one image
can locate objects with boundary boxes


Disadvantages 
-------------
approx 2000 regions - on those CNN works - computationaly expensive
that a a reason more advanced model came - 
Fast RCNN - Runs CNN once on the whole image and shares features for all the regions
Faster RCNN - replaces selective search with RPN (Region proposed Network)
Mask RCNN - add pixel level object segmentation in addition to boundaries - highly accurate





GST payers data of last 5 years of certain state
columns like KYC details, amount of GST due, paid, defaulter (Y/N)
you have 30 columns

aim - predict next GST payers is defaulter  or not

what are pre processing steps
which algorithm you use (ML or DL what you will use and why)
what you will do to find important columns for prediction

- check the columns df.columns
- check df.shape (rows Vs Col)
- df.dtypes (obj - contains string)
- remove duplicates
- impute missing values if they are not high in any column
  if missing vals are very high - we delete that col
- variance in a col - Age - all age is 25
  if var is low - delete that col
- correlation between vars - heat maps
  if multiple vars are correlated we keep 1 and delete others
- data visualization and check if we have outlier
- basic ML algo - Logistic reg, decision trees, random forest, naive bayes classifier
- decision trees, random forest - feature impotances tells which column is 
  contributing to result
-----------------------------------------------------------------------

Autoencoders 
-------------
Netflix - has millions of users and they have their own behaviours
can we compress the important information into smaller meaningful patters ?

or

how does your phone reduce image size but still the image recognizable ?

Autoencoders - learns
how to compress data
then reconstruct it again


like Zip files, Human memory, summaries, data compression

autoencoders learns the most important features automatically

Definition of autoencoders - An autoencoder is a neural network that
1. takes the input data
2. compress it
3. Tries to recreate the same data

What is the Architecture of autoencoder
Input -> encoder -> Bottleneck -> Decoder -> o/p

1. Input layer - original data like image, customer data, transactions
2. Encoder - compress the information eg 10000 features - compress is 100 features
   like summary of a book into notes
3. Bottleneck - Most important compressed representation/ knowledge learned
4. Decoder - Rebuild the original data
5. o/p - original data

Autoencoders is - not supervised learning
                - not a classification 
it is self supervised learning. which means input itself becomes target o/p

Why encoders matter 
--------------------
Banking - Fraud detection
Healthcare - MRI noise detection
Manufacturing - predictive maintainance
Retail - recommendation system
Cybersecurity - intrusion detection
finance - Risk anomaly detection

Autoencoders learns the normal behaviour
if reconstruction errors become high- it is anomaly

--------------------------------------------------------
Boltzmann machines
----------------
how does netflix guess what movie you may like next ?

or

how dows spotify recommend songs ?

AI systems try to discover 
1. hidden preferences
2. hidden patterns
3. hidden relationships

Boltzmann machines were one of the early deep learning models designed for this

Boltzmann machines learns -
WHICH THINGS USUALLY OCCUR TOGETHER ?

eg customers who buy phones also buy covers
   people who watch action movies also watch thrillers
   users who like cricket may like football highlights

Human brain analogy
Rain - umbrella
coffee - biscuits

Boltzmann machine is a neural network that learns probability patters and hidden 
relationships in the data

unlike ML - it does not memorize exact answers
instead it learns probabilities and relationships

Structure of Boltzmann machines
------------------------------
Visible nodes -> hidden nodes

visible nodes -  movie ratings purchases, clicks, symptoms
hidden nodes  - customer taste, personality, preferences behaviour patters

User A - you like movies which are having
         Action and Thriller

User B - likes Romance, Drama
User C - likes action and sci fi

hidden layer may learn 
hidden feature 1 => likes excitement
hidden feature 2 => lines emotional stories

Ludwig Boltzmann
low energy = stable patters
high energy = unlikely patters

Boltzmann machines were the foundational models of 
- recommendation engines
- collaborative filtering (combination of content based and user based filtering)
- preference learning

user based filtering - it can go wrong as taste of people are different
content based filtering 

Problem with Boltzmann machines 
extremely slow

RBM - restricted Boltzmann machines
this is called restrcited because connection among nodes are restricted
there are cross layer connections

- employees can talk only to managers

but - employees cannot talk to each other
      managers cannot talk to each other


if you compare Autoencoders with Boltzmann machines

Autoencoders - Deterministic models, faster, common in today's world, focus is compression
Boltzmann machines - probabilistic, slower, less common today, focus is to find relationship in patters



deployement process of python project
leadership role what path to follow in AI domain
GenAI and Agentic AI industry use cases
Job prospects - genai or agentic AI
genai tools 
algorithms/ libraries used in industry for GenAi 
lang chain
lang graph
crew ai



GAN (Generative Adversarial Networks)

can AI generate - fake human faces 
generate fashion models
generate music
generate product designs
deepfake videos
creating advertisements


what is GAN - two neural networks competing against each other to become smarter
eg counterfeit money

goal of Artist (Generator) - create fake currency
goal of Police (Discriminator) - detect fake notes

initially - fake notes were terrible
            Discriminator easily catches them

over time -  counterfeit artist improves
             police also improves

eventually - fake notes become more realistic

this is called as GAN Training

Generator -- create fake data
Discriminator -- detects fake vs real
comptetion - to fail the other/ both networks improves

Business Examples
--------------------
Banking - fraud simulation 
healthcare - generate medical scane for training
marketing - AI generated ads, personalised product images
fashion - clothing design
gaming - generate characters

how generator and discriminator works - step by step intution

Genrator - Input - random noise
           Output - fake data
it is learning patterns, shapes, styles and structures

Discriminator - Input - real image and fake image
                Output - probability of being real

both are becoming smarter

GAN training process - baby step flow
step 1 - generator creates a fake image
step 2 - Discriminator checks is it real ? is it fake ?
step 3 - Discriminator gives feedback eg the image looks fine or not fine
step 4 - if not fine generator improves
step 5 - repeat above steps 10000 times

GAN do not memorize images
it learns - patterns, distributions, structures

Generator wants - discriminator should say its real
          loss - how bad  the fake image ?
discriminator wants - correctly identify fake or real
          loss - how many mistakes were made ?

Explain Training battle
Epoch          Generator         discriminator
start          weak				 strong
Middle         Better            Better
End            Very realistic    confused



# deployement process of python project

Developer -> writes python code (Flask or django application) -> pushes to github -> cloud platforms (AWS/ Azure/ GCP) -> download the project -> install python and relevant packages in cloud -> Build the application -> start python server -> give public URL -> user can access your app

py2exe


leadership role what path to follow in AI domain
basics of AI and ML (terminologies)
domain knowledge is must
Genarate AI and LLM terminologies 
cloud envt
project management
AI ethics and governance 



GenAI and Agentic AI industry use cases
- generating medical reports
- summarise patient records
- assist doctors in diagnosis

banking - fraud detection, financial doc summarization, chatbots

Retail and ecommerce - 
software devt - code generation, bug fixingm documentation etc


1. Tansformer models 
used in chat bots
machine translation
code geenration
GPT 5
GPT 4
Claude
gemini
llama
deepseek
mistral 

2. Diffusion models - used for high quality images/ videos
eg - DALLE
     MidJourney

3. Vision transformers - based on image adapts its understanding
eg face recognition, image classification

4. CNN

5. LSTM or RNNs































































































































































































































































































































































































































































































































