Project Proposal - Video Game Ratings
---
Joris van Vugt, Guido Zuidhof

### Problem domain
Video games are released constantly, finding the perfect game becomes a challenge. Game review sites provide reviews of newly released video games to help consumers decide which game to pick up. A higher review score is likely favorable for the game publisher, as it will likely pull in more customers. Certain genres may sell better than others, and also the release date is carefully selected by the publisher: often right before christmas. 

In this project, we build on review data from over 20 years, scraped from the biggest game review website to build a Bayesian network model about the factors involved scoring a game.

### Data
We use data from the *20 Years of Games* dataset, which is a dataset obtained by scraping the game review website IGN.com. It is publicly available at [Kaggle datasets](https://www.kaggle.com/egrinstein/20-years-of-games). It contains 18625 game reviews. For every review the score phrase (e.g. *Great* or *Unbearable*) , the title of the game, url, the platform, score, genre, whether it was editors choice, and the release day, month and year. 

### Implementation Plan
We will implement our network in the hipster programming language for technical computing: *Julia*. This will be a first for us. We have done some research on bayesian network libraries, and found [BayesNets](https://github.com/sisl/BayesNets.jl) which seems to be a good fit. If it is not, we will roll our own. 

As a fallback plan we will resort to a Python implementation.

### Inference problem
We are interested in which of the variables make for a good review score, can a game publisher use it to pinpoint a specific formula to get a masterpiece rating with editor's choice seal? Are games released just before christmas also rated higher? Which genre is most highly rated in 2016?




