# Modeling Steps
Once the data preprocessing is done, we can proceed to decision tree analysis. The table below shows the steps of decision tree analysis.  

## Step 1 - Data Partition Node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DataPartition_1.png)  
- A data partition node was dragged into the diagram, and I connected the impute node to data partition node. After that, I change the data set allocation to 70 for training, 30 for validation and 0 for testing.  


## Step 2 - Decision Tree Node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTree_1.png)  
- 3 decision trees node were dragged into the diagram. In Decision Tree – Max levels, I leave all the settings by default. 

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTree_2.png)  
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTree_3.png)  
- In Decision tree – 3 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 3 levels as shown in figure above.

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTree_4.png)  
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTree_5.png)  
- In Decision tree – 2 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 2 levels as shown in figure above.

## Step 3 - Model Comparison Node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/ModelComparison_1.png)  
- A model comparison node was dragged into diagram and connected by all decision tree models. The node is used for comparing the performance of models. Once connected, run the model comparison node.

# Result Analysis
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_1.png)  
Based on the figure above, we can see that Decision Tree – Max levels has the least misclassification rate in validation, followed by Decision Tree – 3 levels and Decision Tree – 2 levels. This could be due to the data contains complex patterns that are better captured by a deeper decision tree. Furthermore, there are not much difference between valid misclassification rate and train misclassification rate, indicating the model did not encounter overfitting. A deeper decision tree can generalize well in large dataset, resulting lower misclassification rate.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_2.png)  
From the figure above, we can see that Tenure has the highest impact to whether the customer will churn or not. The higher the tenure, the lower the probability that the customer will churn. Apart from that, complain is the second variable that impact whether the customer will churn or not. High complains results in customer’s churn. The figure also showed the variables such as NumberOfAddress, CashbackAmount, PreferredPaymentMode, PreferredOrderCat and more that will impact to whether the customer will churn or not.  
