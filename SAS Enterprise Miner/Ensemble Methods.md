# Modeling Steps
In this study, I also apply Gradient Boosting and Random Forest for prediction in SAS interprise Miner. Below shows the steps of applying Gradient Boosting and Random Forest.  

## Step 1 - Gradient Boosting Node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_1.png)  
A Gradient Boosting node was dragged into the diagram, and I connected the data partition node to it. I leave all the setting by default and connect it to model comparison node.  

## Step 2 - Random Forest Node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_1.png)  
A HP Forest node was dragged into the diagram, and I connected the data partition node to it. I leave all the setting by default and connect it to model comparison node.  

# Result Analysis
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_1.png)  
Random Forest has lower misclassification rate in both Valid data and Train Data compared to Gradient Boosting. This indicating that Random Forest perform better than Gradient Bosting. Random Forest applied bagging, which build a collection of decision trees with some level of diversity. It may help in capturing different aspects of the data and improve generalization, resulting lower misclassification rate. While Gradient Boosting applied boosting, which focuses on correcting errors of previous tree. If the errors are not captured well by the weak learners, it may result in higher misclassifications rate. However, random forest may encounter overfitting issue as train misclassifications rate is lower than valid misclassification rate. On the other hand, gradient boosting did not encounter overfitting issue as the train misclassification rate close to the valid misclassification rate.  

In overall, the decision tree – max levels has the lowest valid misclassification rate among other models. This interpreting that if the decision tree is constructed properly, it can outperform than any other robust model like Random Forest. Apart from that, the feature importance assigned in Decision Tree and Random Forest may different, resulting decision tree perform better than random forest.  

