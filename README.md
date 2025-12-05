# LSTM-Models-in-Propaganda-Detection
This project deployed a propaganda detection pipeline using a variation of BIO tagging and LSTM models.

# Research Aim
There are two main tasks in propaganda detection. The first task is classifying a set of word sequences by the propaganda technique each of them uses (defined as Task 1 in this study). We compare two methods in solving this problem: one using a Logistic Regression model, i.e. a linear statistical model, and another using a bidirectional-Long- Short-Term-Memory (bi-LSTM) model, i.e. a neural network model. We also include a Multinomial Naïve Bayes (MultinomialNB) model as a baseline of the performance. Generally, a discriminative model like Logistic Regression model should outperform a generative model like Naïve Bayes model (Ng, 2001) (Xue, 2008). Furthermore, Naïve Bayes models often produce widely overconfident probability due to the naïve independence assumptions (Rish, 2001). The second approach adopts bi-LSTM, a neural network model that specialises in analysing relations within sequential data. In practice, a neural network model can have low performance if the data is not large enough or not complex enough (Boulesteix, 2014) (Du, 2013); still, with the bi-LSTM model we aim to have a better performance than the MultinomialNB model at best.

The second task is using neural network approaches in propaganda detection (defined as Task 2 in this study). The detection pipeline includes two parts: first, identifying a propaganda snippet in a sample sentence, and second, classifying the propaganda technique the sample uses. We present SOBIE labelling system we use to complete this pipeline. We compare two models in using the SOBIE labelling system: an LSTM model and a Maximum-entropy Markov Model bi-gram neural language model (MEMM bi-gram NLM). We also discuss how SOBIE labelling system can fix the sparsity issue encountered when tagging word sequences (Allison, 2006) (Chen, 2024).

# Files
In the folder *code* include two jupyter notebooks, Task 1.ipynb shows the code and results of the sequence classification task (i.e. Task 1), and Task 2.ipynb shows that of the sequence tagging task (i.e. Task 2). 

Report is also included in the repository. 
