# LMMs

=============== Chapter 1: LMM overview ==============================

LMM overview:
1. can learn multiple tasks in one go with different types of input data.
2. has many parameters
3. cost millions to trian

LMM applications:
- customer support chatbots
- sentiment analysis -> market research!
- automated content creation -> marketing
- personalised learning in education


Multimodel LLMs
*** can work with multiple types of input data

video + text --> social media analysis
video (interview) + text (cv) -> automated job interviews
video + text + images -> wildlife conservation

More use cases:
chatbots + sentiment analysus tool - that understand sarcasm + humor
code generation - to accelerate software development



What makes LLMs powerful?
1. Context aware:
A word have different meaning depending on context.
2. Multi-task learning:
Models are trained to perform multiple related tasks in one go
eg. image captioning + text summary + language translation
... which improves accuracy of each individual tasks
... reduce cost due to not having to train many individual models



================ Chapter 2: NLP overview ======================

1. Tokenization
   split sequence into k-mers / list of words
2. Stop word removal
   remove redundant information eg. special characters, common words
3. Lemmatization
   group similar words together eg. run & running
4. Embedding & representation eg. Bag of words
   conver words to numerical representations

================ Chapter 3: LMMs in practice ======================

* Data preparation
1. tozenization
2. stop word removal
3. lemmantization

* LMM pre-training
Pre training LMMs is very hard:
1. COST: LMMs often cost millions of dollars
2. RESOURCES: use thousands of GPUs to pre-train.
3. TIME: An LMMs pretraining could take months!
4. DATA: Requires ALOT of data.

* LMM fine tuning
However, LMMs after pre-training can be FINE-TUNED for specific tasks
using single CPU/GPUs ... and this only takes a few hours / days

FINE TUNING TECHNIQUES:
Fine tuning LMMs are an example of TRANSFER LEARNING.
1. Zero-shot:
   with no task specific data required.
   eg. a zebra is like a horse with stripes.
   ... note we do not require any zebra images
2. Few-short
   with little task specific data
3. Multi-shot
   with many training data




================ Chapter 4: Relevant Concepts ======================

TRANSFORMERS
- architecture emphasise LONG RANGE relationships between words
- utilises ATTENTION MECHANISM

TRANSFORMER ARCHITECTURE:
1. Pre-processing
   tozenization, stop word removal, lemmantization, embeddings
2. Positional encoding
   tags positional information of each word
3. Encoders
   uses ATTENTION mechanism & neural network
   which focuses attention on SPECIFIC words & relationships
   and identify LONG RANGE DEPENDENCIES.
   neural nets picks out most important features
4. Decoders
   uses ATTENTION mechanism & neural network
   to return back final output

ATTENTION MECHANISM
- identify long range dependecies of words
- understand complex structures and patterns
- focus attention on important words

TWO types of Attention
1. Self Attention
   > focus on importance of each word
   > captures long range dependencies of each word
2. Multi-headed attention
   > for each word, we focus on many different aspect of analysis
   eg. for a given sentence we can focus on:
       a) sentiment and emotions
       b) primary topic
       c) related side topics
   > can focus on multiple aspects of a sentence simultaneously
