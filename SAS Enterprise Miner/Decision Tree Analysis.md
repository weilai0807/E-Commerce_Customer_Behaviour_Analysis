# Modeling Steps
Once the data preprocessing is done, we can proceed to decision tree analysis. The table below shows the steps of decision tree analysis.  

Step 1 - Data Partition node
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_1.png)  
- A data partition node was dragged into the diagram, and I connected the impute node to data partition node. After that, I change the data set allocation to 70 for training, 30 for validation and 0 for testing.  

- 3 decision trees node were dragged into the diagram. In Decision Tree – Max levels, I leave all the settings by default. 
 
- In Decision tree – 3 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 3 levels as shown in figure above.
 
 
- In Decision tree – 2 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 2 levels as shown in figure above.
 
- A model comparison node was dragged into diagram and connected by all decision tree models. The node is used for comparing the performance of models. Once connected, run the model comparison node.

# Result Analysis

Based on the figure above, we can see that Decision Tree – Max levels has the least misclassification rate in validation, followed by Decision Tree – 3 levels and Decision Tree – 2 levels. This could be due to the data contains complex patterns that are better captured by a deeper decision tree. Furthermore, there are not much difference between valid misclassification rate and train misclassification rate, indicating the model did not encounter overfitting. A deeper decision tree can generalize well in large dataset, resulting lower misclassification rate.  

From the figure above, we can see that Tenure has the highest impact to whether the customer will churn or not. The higher the tenure, the lower the probability that the customer will churn. Apart from that, complain is the second variable that impact whether the customer will churn or not. High complains results in customer’s churn. The figure also showed the variables such as NumberOfAddress, CashbackAmount, PreferredPaymentMode, PreferredOrderCat and more that will impact to whether the customer will churn or not.  
