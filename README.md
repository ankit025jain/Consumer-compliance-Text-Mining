# Consumer-compliance-Text-Mining

# Text Mining

# Predict performance ratings of banks based on Grievance desriptions of their customers.

# Problem Statement

Generally, the consumer grievances against Banks broadly fall into two categories; “Un-fair and deceptive business practice related (UFDP)” and “efficiency related (not UFDP)”.
It is expected that the Bank monitors compliance management system on a regular basis to “self-identify weaknesses and take corrective action” by closing grievance (irrespective of type of grievance) with or without monetary relief etc. Similarly, where grievance is closed with explanation, resulting in a potential dispute, it is expected that “consumer grievance response” is measured in terms of effectiveness of communication. While the “number of grievances” involving Unfair and deceptive practices, as defined under Section 5 (Unfair or Deceptive Acts) of Federal Trade Commission Act, USA (Please refer to the detailed discussion of Section 5 as applicable to banks at consumer compliance handbook at https://www.federalreserve.gov/boarddocs/supmanual/cch/ftca.pdf), out of all grievances is an important measure, it is also important for the Regulator to keep a tab on “duration” (persistence of violation over a long period of time) of such grievances.
Note : You are required to develop unique words/phrases for identification of a grievance as UFDP or otherwise by using key words of regulations and/or the text forming part of Grievance description through the use of text mining techniques. You can refer to the above cited link for definition of UFDP as per act and you may explore domain further to dig into the details. Exploration of domain and also usage of Grievance Description column to identify the grievance category as UFDP or otherwise may help you not only to understand the problem well but also to understand some of the required domain based feature extraction in solving the problem.
Objective: You are expected to create an analytical and modelling framework to predict the rating of the compliance management function of Banks as outstanding/satisfactory/deficient based on the given data using the above criteria.

## Business Understanding

Banks have their own set of people who work in the compliance department to classify the queries of customers as UFDP or Non UFDP. But with the help of techniques of machine learning and artifitial intelligence (AI agent) the grievance description of customers can be classified as UFDP or Non UFDP without human intervention. The data available is text data and with the help of text mining, we can predict whether the grievance description of the customer falls under UFDP or Non UFDP.
Further, based on other parameters/performance of the banks. Banks can be rated as "outstanding", "staisfactory" or "Deificient".
Business can utilize these performance ratings to understand the Grievance description of customers, customer sentiments towards the bank. It will help them to improve their strategies, practices, build better customer services and many more imporvements to reach the oustanding performance.

### Prerequisites

You need to install Python software

```
Python 3
Jupyter Notebook
```

### Add to git and push

```
$cd /project path
$git add https://github.com/ankit025jain/Consumer-compliance-Text-Mining-
$git commit -m "Enter commit message here"
$git push

```
# Instructions

## Steps to be followed:

```
Step1: Clone or download using this link(https://github.com/ankit025jain/Consumer-compliance-Text-Mining.git)

Step2: Run the preprocessing and clustering file (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Preprocesing%20and%20clustering)

Step3: Followed by preprocessing and clustering file, Run the model building files (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Model%20Building)

Note: Cluster1, cluster2, cluster3, cluster4 are obtained by different methods followed in preprocessing of the text data.
```
### Folder information and files description:

```
Consumer-compliance-Text-Mining/Dataset/ - Contains the dataset. 
    i) GrievancesData_Train.csv - contains the train data without target.
    ii) Train.csv - contains BankID and BankGrade(target) columns data.
    iii) GrievancesData_Test.csv - contains the test data without target.
    iv) Test.csv - contains BankID column on which our model should do the predictions.
    v)ftca.xlsx - contains the data copied from ftca.pdf (ftca.pdf can be found in this link (https://www.federalreserve.gov/boarddocs/supmanual/cch/ftca.pdf)
    vi)ftca and cch.xlsx - Content copied from ftca.pdf and cch.pdf (cch.pdf can be found in this link- (https://www.federalreserve.gov/boarddocs/supmanual/cch/200711/cch200711.pdf)

Refer (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Dataset)

Consumer-compliance-Text-Mining/Preprocesing and clustering/ - Contains the preprocessing and clustering .ipynb file.

Refer (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Preprocesing%20and%20clustering)

Consumer-compliance-Text-Mining/Model Building dataset/ - Dataset obtained after preprocessing and clustering which can be used for model building.
    i) final_train_data.csv - Train data for model building
    ii) final_test_data.csv - Test data for model building

Refer (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Model%20Building%20dataset)

Consumer-compliance-Text-Mining/Model Building/ - Contains the code used for model building.
  Major difference in the below models is the cluster values. Please refer below to get more insights.
    i)Model_Building_Cluster_1.ipynb - Cluster values used from cluster 1 which was obtained from doc2vec of ftca document and the Grievace description column and then performing clustering on it.
    ii) Model_Building_Cluster_2.ipynb - Cluster values used from cluster 2 which was obtained from doc2vec of ftca document and the Cleaned Grievace description column(Text Preprocessed Grievance description column) and then performing clustering on it.
    iii) Model_Building_Cluster_3.ipynb - Cluster values used from cluster 3 which was obtained from doc2vec of (ftca document + consumer compiance handbook[cch]) and the Grievace description column and then performing clustering on it.
    iv) Model_Building_Cluster_4.ipynb - Cluster values used from cluster 4 which was obtained from tfidf of grievance description column and then performing clustering on it.

Refer (https://github.com/ankit025jain/Consumer-compliance-Text-Mining/tree/master/Model%20Building)

```
**Please feel free to connect with the author in case you get stuck anywhere or if you are facing any issues**

## Author

* **Ankit Jain** - *Initial work* - [Ankit Jain](https://github.com/ankit025jain)

**Contributing to this code is much appreciated:)**

See also the list of [contributors](https://github.com/ankit025jain/Consumer-compliance-Text-Mining/graphs/contributors) who participated in this project.

## What more you can try?

I wanted to try LSTM or Skip thoughts approach before the classification of the Grievance description into UFDP and Non UFDP by clustering algorithm.

A detailed description of skip thoughts can be found in this link: https://medium.com/@sanyamagarwal/my-thoughts-on-skip-thoughts-a3e773605efa

Also refer this link for skip thoughts summarization and clustering which is another approach to this problem (https://medium.com/jatana/unsupervised-text-summarization-using-sentence-embeddings-adb15ce83db1)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

## Acknowledgments

* INSOFE for conducting hackathon on this topic.
* Google
* Stackoverflow
* Github
* Inspiration
* Motivation
* Smartwork
* Hard work
* etc

#Text mining #Risk Compliance #Compliance #INSOFE #Banks #Consumer #Grievances #Inspiration #Machine Learning #Deep Learning #AI #Artifitial Intelligence #Accuracy #SMOTE #Python #Logistic regression #Decision trees #random forest #XGBoost #Adaboost #Gaussian naive bayes #Naive bayes #SGD #sequential #functional #Programming #Linear regression #LSTM #GRU #Artifitial neural network #Deep learning #Long Short Term Memory #CNN #Convolutional neural network #Clustering # #Ensemble Methods #ensemble.AdaBoostClassifier() #ensemble.BaggingClassifier() #ensemble.ExtraTreesClassifier() #ensemble.GradientBoostingClassifier() ensemble.RandomForestClassifier() #Gaussian Processes #gaussian_process.GaussianProcessClassifier() #GLM #linear_model.LogisticRegressionCV() #linear_model.PassiveAggressiveClassifier() #linear_model.RidgeClassifierCV() #linear_model.SGDClassifier() #linear_model.Perceptron() #Navies Bayes #naive_bayes.BernoulliNB() #naive_bayes.GaussianNB() #Nearest Neighbor #neighbors.KNeighborsClassifier() #SVM #svm.SVC(probability=True) #svm.NuSVC(probability=True) #svm.LinearSVC() #Trees #tree.DecisionTreeClassifier() #tree.ExtraTreeClassifier() #Discriminant Analysis #discriminant_analysis.LinearDiscriminantAnalysis() #discriminant_analysis.QuadraticDiscriminantAnalysis() #XGBClassifier() #Best text mining #Best project #Happy #HappyGithubing.
