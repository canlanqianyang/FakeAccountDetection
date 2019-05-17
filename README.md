# FakeAccountDetection
This work is to detect spammers in our weibo (ID:PowerRanger6歪果仁) fans. A classifier has been built using the machine learning algorithm (Support Vector Machine) combined with the features selected from the user profile and tweets, such as the number of followers, the number of retweets, and so on. 

## Support Vector Machine
SVM is a machine learning algorithm. It is used to build the classifier to distinguish the spammers from the normal ones in this project. We use sklearn+python for it. 
Here is the tutorial:[https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html](https://scikit-learn.org/stable/modules/generated/sklearn.svm.SVC.html)

## Experiment

* Use crawlers to acquire training and test data sets. Users in the training data set were randomly selected, and users in the test data set were our weibo fans. The user info ( id, account name, number of followers, number of retweets, number of microblog and number of popular microblog) in both training and test data sets are crawled, while whether a user is a spammer or not is manually judged in training data set.
* Train the classifier using SVM and training data sets.
* Finally, decide whether users in test data set are spammers or not using the classifier. 

## Files
* getFansData.ipynb: the crawler.
* SVM.ipynb: train the classifier and forecast.
* data/trainData.txt: traing data set.
* data/predData.txt: test data set.
* data/preResult.txt: result file.

## Result
![](https://github.com/canlanqianyang/FakeAccountDetection/blob/master/pic.PNG)
>id;name;verified;followers_count;follow_count;post_count;hot_blog_count;is_spammer<br>
>6349014467;优秀图;1;6953;6152;343;100;0<br>
>6937931818;美人天下992;0;55;2947;6;0;1<br>

In result file, "1" in the last column means the user is spammer, and "0" means the normal user.

