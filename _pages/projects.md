---
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /resume
---

In reverse chronological order:

* **Identify Misinformation/Fake news from social media**
  * Research in Deep Learning and NLP approach to identify fake news and rumour 
  * Collect fake news data in Singapore, crawl and annotate rumour/non-rumour data gleaned from social media (Twitter, Facebook, Forums)
  * Work in progress

* **Topic modelling for scientific authors**  \|  [[code](https://github.com/tramanh06/rpms)]
  * Researched in topic model using Latent Dirichlet Allocation. Extended LDA for a hierarchical collection of documents. Achieved good results with Author-Topic Model
  * Built a ranking system to assign relevant reviewers to papers and automatically nominate reviewers during review process
  * Advisor: Prof [Bryan Low](https://www.comp.nus.edu.sg/~lowkh/research.html)

* **Financial Reporting using Machine Learning**
  * Applied ML methods on financial transaction data. Solution using Neural Network and Decision Tree.
  * Enhanced interpretability of ML system by displaying Decision Tree result. Certain level of pruning was done to make the tree more readable
  * Replace hand-coded rules with 99% accuracy

* **Enhance Customer Churn prediction through Semi-Supervised Learning**  \|  [[code](https://github.com/tramanh06/CDR-analysis)]
  * Modeled customer and their calls as one big graph, with edge weights as a function of calls and text activities
  * Researched on Label Propagation to propagate labeled nodes (already churned customers) to unlabeled nodes in a graph. Churned customers might influence their friends in the network to churn
  * Used Label Propagation score as a feature to train churn classifier. Winner classifier is Logistic Regression with accuracy of 96.9% accuracy
  * Designed an architecture to train the data in a distributed manner using MapReduce, speeding up training time
  * Advisor: Prof [Ng Wee Keong](http://www.ntu.edu.sg/home/awkng/)
  

* **Prediction of genetic sequence mutation using Neural Network**  \|  [[code](https://github.com/tramanh06/HIV-DNA-neural-network)]
  * Implemented Recurrent Neural Network to train and predict how genetic sequence mutates under influence of HIV-1 drugs. Used one-hot encoding to encode 4 proteins (T, G, A, C) and LSTM to process the sequence. Correctly predicted positions of mutation and corresponding types up to 80%
  * Researched and experimented alternative approach using Game Theory and Cellular Automata
  * Advisor: Dr [Samuel Gan](http://www.bii.a-star.edu.sg/research/trd/apd.php), Dr [Su Tran To Chinh](https://www.linkedin.com/in/chinhsutranto/?originalSubdomain=sg)

* **Privacy-preserving in Outsourced Database**  \|  [code: [ElGamal](https://github.com/bazzilic/ElGamalExt), [Paillier](https://github.com/bazzilic/PaillierExt)]
  * Implemented ElGamal and Paillier Homomorphic Cryptosystems to encode plaintext SQL queries and retrieve result from encrypted database
  * Built different handlings for different types of queries (AND, OR, and aggregate functions)
  * Advisor: Prof [Ng Wee Keong](http://www.ntu.edu.sg/home/awkng/), Dr [Vasily Sidorov](http://bazzilic.me/)


* **Preserving Data Integrity in Cloud Storage** \| [Technical Report](https://dr.ntu.edu.sg/handle/10220/26032)
  * Researched on a tree-based hashing function to detect changes in files. Idea: File is split into blocks, and forms leaves of a B-tree. Root of the tree is hashed in a bottom-up manner, becoming signature of the file. Signature is computed regularly on the third-party storage site and sent to a server for integrity checks
  * Implemented a working solution for the generation of signature and server check. Confirmed the runtime complexity of calculating signature is less than O(n)
  * Work is selected to present at *International Conference of Undergraduate Research 2015*
  * Advisor: Prof [Ng Wee Keong](http://www.ntu.edu.sg/home/awkng/)


<!-- {% include base_path %}

Education
======
* B.S. in GitHub, GitHub University, 2012
* M.S. in Jekyll, GitHub University, 2014
* Ph.D in Version Control Theory, GitHub University, 2018 (expected)

Work experience
======
* Summer 2015: Research Assistant
  * Github University
  * Duties included: Tagging issues
  * Supervisor: Professor Git

* Fall 2015: Research Assistant
  * Github University
  * Duties included: Merging pull requests
  * Supervisor: Professor Hub
  
Skills
======
* Skill 1
* Skill 2
  * Sub-skill 2.1
  * Sub-skill 2.2
  * Sub-skill 2.3
* Skill 3

Publications
======
  <ul>{% for post in site.publications %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Talks
======
  <ul>{% for post in site.talks %}
    {% include archive-single-talk-cv.html %}
  {% endfor %}</ul>
  
Teaching
======
  <ul>{% for post in site.teaching %}
    {% include archive-single-cv.html %}
  {% endfor %}</ul>
  
Service and leadership
======
* Currently signed in to 43 different slack teams
 -->