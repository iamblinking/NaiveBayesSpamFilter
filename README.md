# NaiveBayesSpamFilter V1.0
利用朴素贝叶斯算法实现垃圾邮件的过滤，并结合Adaboost改进该算法。
##1 Naive Bayes spam filtering
&emsp;&emsp;假设邮件的内容中包含的词汇为Wi，垃圾邮件Spam，正常邮件ham。
判断一份邮件，内容包含的词汇为W={W1，W2......Wn}，判断该邮件是否是垃圾邮件，即计算P（S|W）这个条件概率。根据Bayes' theorem：

![Bayes' theorem](https://upload.wikimedia.org/math/a/6/e/a6e7f8c521dcf018b6480a8967773ac3.png)

其中：

- Pr(S|W) is the probability that a message is a spam, knowing that the word "replica" is in it;
- Pr(S) is the overall probability that any given message is spam;
- Pr(W|S) is the probability that the word "replica" appears in spam messages;
- Pr(H) is the overall probability that any given message is not spam (is "ham");
- Pr(W|H) is the probability that the word "replica" appears in ham messages.
