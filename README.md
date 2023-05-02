Download Link: https://assignmentchef.com/product/solved-comp90049-assessment-1-naive-bayes-and-k-nearest-neighbour-for-predicting-stroke
<br>
<span class="kksr-muted">Rate this product</span>

In this project, you will implement Naive Bayes and K-Nearest Neighbour (K-NN) classifiers. You will explore inner workings and evaluate behavior on a data set of stroke prediction, and on this basis respond to some conceptual questions.

Implementation

The lectures and workshops contained several pointers for reading in data and implementing your Naive Bayes classifier. You are required to implement your Naive Bayes classifier from scratch. You may use Python libraries of your choice for implementing K-NN, evaluation metrics, procedures and data processing.

For marking purposes, a minimal submission should have a preprocess() function, which opens the data file, and converts it into a usable format. It should also define the following functions:

• split_data(), where you split your data sets into a training set and a hold-out test set.• train(), where you build Naive Bayes and K-NN classifiers from the training data. You can

create train your data as you answer the related question.

• predict(), where you use a trained model to predict a class for the test data. You can also do prediction as you answer the related question.

• evaluate(),whereyouwilloutputtheaccuracyofyourclassifiers,orsufficientinformation so that it can be easily calculated by hand.

There is a sample iPython notebook S2020S2-proj1.ipynb that summarizes these, which you may use as a template.

You may alter the above prototypes to suit your needs; you may write other helper functions as you require. Depending on which answers you choose to respond, you may need to implement additional functions.

Packages

To provide the possibility of running your codes by markers, limit utilising the packages to the fol- lowing packages in this project:

<ul>

 <li>pandas to read, split and preprocess the data</li>

 <li>sklearn to develop K-NN model and evaluate models</li>

 <li>numpy to implement scientific computing</li>

 <li>math to access to the mathematical functions</li>

 <li>matplotlib to create plots and visualizationsDataFor this project, we have adapted the Stroke data that have been used for stroke prediction [1], avail- able online at (https://data.mendeley.com/datasets/x8ygrw87jw/1):Some critical information:</li>

</ul>

<ol>

 <li>File name: stroke_update.csv</li>

 <li>2740 instances</li>

 <li>10 attributes that include numeric and nominal attributes. The attributes avg_glucose_- level, bmi and age are numeric. the rest of attributes are nominal.</li>

 <li>The file stroke_features.txt explains each attribute</li>

 <li>2 classes, corresponding to the stroke outcomes: {0: No stroke, 1: Having stroke}</li>

</ol>

Questions

You should respond to questions 1-3. In question 2 (b) you can choose between two options for smoothing and two options for Naive Bayes formulation. A response to a question should take about 100–200 words, and make reference to the data wherever possible.

Question 1

<ol>

 <li>a  Explore the data and summarise different aspects of the data. Can you see any interesting characteristic in features, classes or categories? What is the main issue with the data? Considering the issue, how would the Naive Bayes classifier work on this data? Discuss your answer based on the Naive Bayes’ formulation [2]. (3 marks)</li>

 <li>b  Is accuracy an appropriate metric to evaluate the models created for this data? Justify your answer. Explain which metric(s) would be more appropriate, and contrast their utility against accuracy. [no programming required] (2 marks)</li>

</ol>

Question 2

a Explain the independence assumption underlying Naive Bayes. What are the advantages and disadvantages of this assumption? Elaborate your answers using the features of the provided data. [no programming required] (1 mark)

<ol start="2">

 <li>b  Implement the Naive Bayes classifier. You need to decide how you are going to apply Naive Bayes for nominal and numeric attributes. You can combine both Gaussian and Categorical Naive Bayes (option 1) or just using Categorical Naive Bayes (option 2). Ex- plain your decision.For Categorical Naive Bayes, you can choose either epsilon or Laplace smoothing for this calculation. Evaluate the classifier using accuracy and appropriate metric(s) on test data. Explain your observations on how the classifiers have performed based on the met- ric(s). Discuss the performance of the classifiers in comparison with the Zero-R baseline. (4 marks)</li>

 <li>c  Explain the difference between epsilon and Laplace smoothing. [no programming required] (1 mark)</li>

</ol>

Question 3

<ol>

 <li>a  Implement the K-NN classifier, and find the optimal value for K. (1 mark)</li>

 <li>b  Based on the obtained value for K in question 4 (a), evaluate the classifier using accuracy and chosen metric(s) on test data. Explain your observations on how the classifiers have performed based on the metric(s). Discuss the performance of the classifiers in compari- son with the Zero- R baseline. (2 marks)</li>

 <li>c  Compare the classifiers (Naive Bayes and K-NN) based on metrics’ results. Provide a comparatory discussion on the results. [no programming required] (1 mark)</li>