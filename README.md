# FakeAccountDetection
This work is to detect spammers in our weibo (ID:PowerRanger6歪果仁) fans. A classifier has been built using the machine learning algorithm (Support Vector Machine) combined with the features selected from the user profile and tweets, such as the number of followers, the number of retweets, and so on. 

## Support Vector Machine
SVM is a machine learning algorithm. It is used to build the classifier to distinguish the spammers from the normal ones in this project. We use sklearn+python for it. Here is the tutorial:[https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)

## Experiment

> Use crawlers to acquire training and test datasets.Users in the training dataset were randomly selected, and users in the test dataset were our weibo fans.
> * 关联规则挖掘选择的数据集为Wine Reviews
> * 作业二预览链接[homework2](https://canlanqianyang.github.io/datamining/homework2.html "homework2")
