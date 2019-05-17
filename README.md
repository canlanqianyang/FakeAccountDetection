# FakeAccountDetection
This work is to detect spammers in our weibo (ID:PowerRanger6歪果仁) fans. A classifier has been built using the machine learning algorithm (Support Vector Machine) combined with the features selected from the user profile and tweets, such as the number of followers, the number of retweets, and so on. 

## Support Vector Machine
SVM is a machine learning algorithm. It is used to build the classifier to distinguish the spammers from the normal ones in this project. We use sklearn+python for it. Here is the tutorial:
[https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)

## Experiment

* Use crawlers to acquire training and test datasets. Users in the training dataset were randomly selected, and users in the test dataset were our weibo fans. The user info ( id, account name, number of followers, number of retweets, number of microblog and number of popular microblog) in both training and test datasets are crawled, while whether a user is a spammer or not is manually judged.
* 
> * 作业二预览链接[homework2](https://canlanqianyang.github.io/datamining/homework2.html "homework2")
