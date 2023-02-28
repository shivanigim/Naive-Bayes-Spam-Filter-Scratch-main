# Naive-Bayes-Spam-Filter
Building a Spam Filter from scratch using Naive Bayes algorithm. I have used a publically available dataset which can be found in the repo.

## About
### Project Overview
Spam classification is implemented in all kinds of messaging services, and it is important that a model can correctly predict them and separate spams for good user experience.

Bayes theorem provides a way of calculating the posterior probability, P(c|x), from P(c), P(x), and P(x|c). Naive Bayes classifier assumes that the effect of the value of a predictor (x) on a given class (c) is independent of the values of other predictors. This assumption is called class conditional independence. This is not true in all the cases and therefore this assumpition is 'Naive'. However, this algorithm gives pretty good results for spam classifications.

The Mathematical formulation is given below : 

![](/images/sample.PNG)

where,

* P(c|x) is the posterior probability of class (target) given predictor (attribute). 
* P(c) is the prior probability of class. 
* P(x|c) is the likelihood which is the probability of predictor given class. 
* P(x) is the prior probability of predictor.

## Input Data

Input Data is publically availble, contains about 5700 messages marked spam and ham (non-spam). The Dataset consists of just two columns and its description is given below :

|#| Column | Type | Description |
| --- | --- | --- | --- |
| 1 | Label | string | Label whether the given example is spam or not|
| 2 | SMS | string | full message |

## Repository Structure and Description:


```
- app
| - images
| |- sample.PNG # image for bayes theorem and naive bayes assumption

- data
|- SMSSpamCollection # the dataset
- README.md 
- spam-classifier.ipynb # Python 3 notebook, which contains notebook version of the program
```

## Conclusion and Improvements

The program is able to predict spam and non-spam messages accurately. However built in packages and other ML algortithms can be much more accurate for this task.

Some improvements that can be made over this are :

* using a bigger dataset 
* using more real world message which are more complex in the datset
