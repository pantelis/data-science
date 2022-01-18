---
title: Syllabus
weight: 10
draft: false
---

# Syllabus

## Books

* [Data Science from Scratch: First Principles with Python (GRUS)](https://www.amazon.com/Data-Science-Scratch-Principles-Python-dp-1492041130/dp/1492041130/ref=mt_other?_encoding=UTF8&me=&qid=). This book is not free and is required for this course _especially by those students that have done limited Python programming_.  The code of the book is [here](https://github.com/joelgrus/data-science-from-scratch.git)

* [Introduction to Statistical learning (ISL)](https://statlearning.com/). This book is _free_ and explains well some of the concepts covered in this course. Is probably the most widely used book as an introduction to data science. The code is in a programming language called $R$ which is still popular for some business and financial firms but increasingly is being displaced by Python especially in big data applications.  We will therefore cover the same concepts but with Python. 
  * You need to [download this Python code](https://github.com/Harvard-IACS/2019-CS109A) to run the examples in Python. 
  * [Video lectures](https://www.dataschool.io/15-hours-of-expert-machine-learning-videos/) of the book authors that you may find useful to supplement mine - you need to omit the Labs. 

## Schedule

The schedule is based on [Academic Calendar Fall 2021](https://www5.njit.edu/registrar/calendars/): 

> NOTE: For most lectures you need to read the Notes that are published in this site _and_ the corresponding book chapters quoted. 

| Lecture     | Description    | Reading List | 
| --- | --- | --- |
|   1  |    **Introduction:** We start with an _introduction to data science_. Through an end to end data science application we understand all the stages of a data science pipeline and the vast open source ecosystem around data science.  You will understand how simple apps like Uber / UberEats hide some really complicated systems that mine data real time,  how literally every aspect of the world economy is powered by data science. | ISL Chapter 1 & GRUS Chapter 1  | 
|   2  |    **Data and their representations in Python**: We review the types of data that we will be dealing with and while doing so we learn some essential Python language data structures that keep them safe.  We will meet [Kaggle](https://www.kaggle.com/) our defacto destination for datasets and Python notebooks that process them and using our first Python libraries we will develop an application that practically showcases data science. We will do all that inside the [Colab](https://colab.research.google.com/) cloud computing environment. We start to see our first representations of data in the form of vectors and aggregations of data in the form of matrices. | GRUS Chapter 2, 3 and 4. | 
|   3  |     **The universal language of probability**:  In this course we will speak a couple of languages. We will introduce a new language such as random variables, independence, probability distributions, expected values and other artifacts for the very brave.  We will learn how to use one of the major libraries in probabilistic modeling that will also revisit later in the course - [Tensorflow  Probability](https://www.tensorflow.org/probability). | GRUS Chapter 5 & 6 | 
|   4  |    **The supervised learning problem**: Almost all the tasks you will be called to perform as data scientists and analysts will have a flavor of  _supervised learning_ for regression and classification. This lecture is foundational - we wont' go into the details of what learning methods we have at our disposal  but what the learning problem is and all the types of learning we are usually dealing with. | ISL Chapter 2.1.1, 2.1.2 & GRUS Chapter 14 |
|   5  |    **Fitting the data**: This is our very first method that fits a regression model to data. We will learn how to calculate the likelihood function  and  maximize this likelihood (ML). ML-based optimization transverses all aspects of machine learning - we learn what ML means by reviewing basic optimization concepts and study an algorithm that is the workhorse of modern machine learning: the _stochastic gradient descent_ algorithm. | ISL Chapter 3.1 & GRUS Chapter 8 |  
|  6  |    **To be or not to be**: We have seen classification as a supervised learning problem but what governs our pursue to design a good classifier? Do you know that good classifiers won World War II ? You will be surprised that the same metrics allied forces used back then to determine an incoming attack from RADAR signals are the very same that Facebook engineers are using to identify your face in your photos. We will use Logistic Regression as an example of a classifier that gives us an bonus feature: the probabilistic interpretation of its output. | ISL Chapter 4.1, 4.2, 4.3, GRUS Chapter 16|
|  7  |   **Good luck in your midterm**  | | 
| 8 |  **One rule to rule them all and model selection**:  The Bayes rule, governs data science like the quantum mechanics rules govern physics. Do you know that for CDC to interpret COVID19 test results correctly they use this rule? We show how we can enhance regression and classification performance (Naive Bayes) by considering prior knowledge.Furthermore Bayes gives us the ability to learn _online_ as data is streamed to applications. It also help us select the right model by avoiding overfitting - something that generically is called _regularization_. | ISL Chapter 6 | 
|  9   |    **Intelligence of the crowds** : _Ensembles_ of predictors can do better than any single one.  _Decision Trees_,  _Random Forests_  and gradient boosters are probably the most versatile and extensively used tools in data science. Such tools survived the deep learning revolution for a good reason. They can still handle massive datasets, offer partially _explainable_ decisions _and_ win Kaggle competitions.  | ISL Chapter 8 & GRUS Chapter 17 | 
|  10   |  **No labels no problem**: The setting this week changes to that of unsupervised learning reviewing data clustering approaches such as K-means. We review use cases in anomaly and novelty detection. | ISL Chapter 10.3 & GRUS Chapter   | 
|  11  |    **800-pounds**. At last, we get to see the gorilla in the room.  _Neural networks_ need to introduction - we use the [Tensorflow playground](https://playground.tensorflow.org/) to understand the tradeoffs between classical and neural architectures and why deep neural networks dominate in big data applications today.  | GRUS Chapter 18  | 
|  12   |    **Water valves**  We get to build our very own DNN training pipeline but not before understanding how neural networks learn. Backpropagation requires some mathematical rigor but in this course we use analogies of valves / gates to visualize how it works for a simple network. Understanding backpropagation is essential for understanding how DNNs behave during training / hyperparameter optimization. | GRUS Chapter 18 & 19 | 
|  13   |   **It was you ...** Before we put DNNs in action they need the right inputs. Sometimes the inputs are two noisy or very high dimensional. Dimensionality reduction and embeddings are key data representation tools that we need to know. Did you know that your face can be represented as vectors in some space? We demonstrate learning the right representations via a face recognition pipeline. | ISL Chapter 10.2 | 
|  14   |  **Final Lecture**  We review what we have learned, preparing for the final.  |  | 
| 15 |   **Good luck in your final** | |
