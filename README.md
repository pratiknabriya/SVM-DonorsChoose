## Objective
To predict whether a Classroom Project proposal will get approved or not using linear Support Vector Classifiers. 

DonorsChoose.org receives hundreds of thousands of project proposals each year for classroom projects in need of funding. Right now, a large number of volunteers is needed to manually screen each submission before it's approved to be posted on the DonorsChoose.org website.

Next year, DonorsChoose.org expects to receive close to 500,000 project proposals. As a result, there are three main problems they need to solve:

* How to scale current manual processes and resources to screen 500,000 projects so that they can be posted as quickly and as efficiently as possible.

* How to increase the consistency of project vetting across different volunteers to improve the experience for teachers.

* How to focus volunteer time on the applications that need the most assistance.

The goal of the competition is to predict whether or not a DonorsChoose.org project proposal submitted by a teacher will be approved, using the text of project descriptions as well as additional metadata about the project, teacher, and school. DonorsChoose.org can then use this information to identify projects most likely to need further review before approval.  

## Data set and other details 

Visit: https://www.kaggle.com/c/donorschoose-application-screening/

## Result Summary

#### Model: Linear SVM (Brute implementation) 

| Set |  Text Featurization |   Hyperparameter: C | AUC_Score |
|-----|---------------------|------------------|-----------|
|  1  |         BOW         |       0.0001      |   0.713   |
|  2  |        TF-IDF       |        0.01       |   0.718   |
|  3  |       AVG-W2V       |         0.1        |   0.692   |
|  4  |      TFIDF-W2V      |       0.001       |   0.689   |
|  5  |    SVD on TF-IDF(top n components)   |        0.01       |   0.712   |  
            
