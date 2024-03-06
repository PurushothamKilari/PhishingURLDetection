

# PhishingURLDetection



## Overall Process: 
Intuition behind model generation is to detect the malicious Url that causes exploits and unauthorized access of the user system through rua(remote User Access).
The Building of the model involves data cleaning & feature extraction then finding out the important labels based on the heat map and the labels with high correlation is taken into consideration and proceed with the choosing of the algorithm in my case I go with the Random forest algorithm that is more accurate with the decision making.
The dataset contains to many labels so with keep the high correlation one and split the dataset into two parts namely training data and testing data both in the ratio of about 70:30 ratio to make the training more accurate
finally calculating the performance of the model based on the precision recall & f-score
The major thing is the confusion matrix that depict the overall model standard and performance 
## solution approach:
  To detect the Maliciour Url  the decision process must be accurate and it must not be overfit to the dataset and  having the generalization of the model with variance and bais .
  The second dataset consists of 1353 URLs with 17 features, and these URLs are classified into 3 categories: Phishing, non-phishing and suspicious. We are going to make use of both of these datasets.
The first thing to do after the datasets are obtained is data slicing. Here, we divide the datasets into two parts: testing dataset and training dataset. The training dataset is used to train a model. The testing dataset is only used once the trained model is ready. Once the model is trained, we test its accuracy on the testing dataset.
By considering all the circumstances decided to go with the Random forest algorithm which have multiple levels of decision tree that generalize the data with no.of classifiers .
by using the scikit-learn module importing the randomforest with max_level of atleast 5 .
train the model with high correlation labels to achieve atleast 80% accuracy over the testing dataset.
## ML_Model Used & Reason for using it:
For the Phishing URL detection I used the random forest algorithm. RandomForest is a best suite for the decision making in the Phishing URL detection since it is a supervised machine learning algorithm that is used to perform both regression and classification task in data mining. It is an ensemble based technique that can be used to perform classification. It makes use of a number of classification trees (like decisiontrees) and then gives the final result. In our case it is important to decide the legitimate URL detection and report the phishing URL
This algorithm works by creating a number of classification trees randomly. These trees are created by making use of different samples from the same dataset and
also they may use different types of features each time to create the trees. Thus, all the trees are created randomly by making use of different sub sets of the same dataset. Also
the features are taken randomly for the creation of any tree. By doing so, Random Forest ensures that it does not overfit the data, as in the case of the decision trees. Once the trees have been formed, we can do the classification by finding the results of each tree and then assigning it to the class that
has been determined by the most number of trees that makes the decision more accurately and detect the  malicious URL accurately so I go with the Random Forest Algorithm
