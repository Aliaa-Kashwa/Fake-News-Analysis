# Fake-News-Analysis
In this project, we are going to answer 3 interesting questions through using different models that they are related to this important topic in NLP field. 

THe three question are:

1) The hypothesis question we provide is:
   - Is the ratio of fake news in Emergent fact-checking site significantly higher than the ratio of fake news by all other fact-checking sites?

2) The regression question is:
   - Predicting the number of user comments for each news.
   -The benefit of answering this question is: Helping knowing that which type of news users can interact with it and may be indicative of its importance or impact.

3) The question that can be answered via predictive analysis is:
   - Predicting fake news with/without urls.
   -The benefit of the this question is: knowing the type of url whether it contain fake news or not. 
    So the user can distinguish between them. And that if the user know that the url was fake for one news we may predict 
    that the other news that has the same link is also fake.
    
The notebook consists of:
    
1) Import important libraries.
2) Import data.
   - You will find the data link in ("Link of competition on Kaggle") file attached above.
3) Data Exploration.
4) Hypothesis Test Question.
5) Regression Question (Predicting the number of user comments for each news).

   - We will extracte the length of comments of each news as a new feature, then used it as label to predict later the expected number of comments on each news and applied this through 2 scenarios:

     • 1: Using the whole data ( 69396 rows) that has missing values in reddit_comments column assuming that the remained news have no comments (0).

     • 2: Using part of the data that has comments on each news without the ones that has missing values assuming that their comments are missed, so delete them, and use that 5235 rows to train/test our model.

6) Predictive Question (Predicting fake news with/without URLs).

   - We tried to predict fake news in two different scenarios:

    • 1: predicting it by the some features including the url.

    • 2: predicting it by the same some features but url.

Hint: To run this notebook on colab, you should download the "kaggle.jison" from your kaggle account then upload it to colab environment.
