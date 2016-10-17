Project Proposal - Modeling Developer Sentiment
---
Joris van Vugt, Guido Zuidhof

### Problem domain
Every year StackOverflow, the biggest question-and-answer site for developers, asks its visitors to fill in a questionnaire. In this questionnaire the participants are asked about their tech preferences, job descriptors, background and why and how they use the website. 

For the first time this dataset was released publically (2016 questionnaire). We intend to build a Bayesian network model to try and capture the underlying causalities.

### Data
We use data from the *Developer Survey Results 2016* dataset, which is a questionnaire filled in by 56,033 *"coders"* from 173 countries. It is publicly available at [their blog](http://blog.stackoverflow.com/2016/03/stack-overflow-developer-survey-results/?cb=1). The results are nicely displayed and analysed [here](http://stackoverflow.com/research/developer-survey-2016#community-asking-and-answering). It contains 45 questions. The main points found in the dataset are the following according to StackOverflow:

> Developers love Rust. Even back-end developers know JavaScript. Only 7% of developers identify as "rockstars". Most developers prefer dogs to cats. (But not developers in Germany.)

### Implementation Plan
We will implement our network in the hipster programming language for technical computing: *Julia*. This will be a first for us. We have done some research on bayesian network libraries, and found [BayesNets](https://github.com/sisl/BayesNets.jl) which seems to be a good fit. If it is not, we will roll our own. 

As a fallback plan we will resort to a Python implementation.

### Inference problem
We are interested in many different correlations, there are so many variables that it is hard to nail it down to only a few. First of all, education type, tech choice and their effect on salary. Are Vim users really socially awkward and have a lower question rating on stackoverflow? Do those people love their job more? How about company size versus job satisfaction?

As we explore the dataset and build a couple of models, we will probably add to this list.

