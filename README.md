# E-Commerce Customer Behaviour Analysis
## Objective
Conduct a comprehensive e-commerce customer behaviours analysis through a set of software, including SAS Enterprise Miner, Talend Data Integration, and Talend Data Prep.

## Process Flow
- Step 1 - Data Manipulation with Talend Data Integration. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/README.md)
- Step 2 - Data Cleaning with Talend Data Prep. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/README.md)
- Step 3 - Handled Missing Values with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Data%20Imputation.md)
- Step 4 - Conduct Decision Tree Analysis with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Decision%20Tree%20Analysis.md)
- Step 5 - Apply Ensemble Methods with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Ensemble%20Methods.md)

## Result Analysis
### Decision Tree Analysis
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_1.png)  
Based on the figure above, we can see that **Decision Tree – Max levels has the least misclassification rate in validation**, followed by Decision Tree – 3 levels and Decision Tree – 2 levels. This could be due to **the data contains complex patterns that are better captured by a deeper decision tree**. Furthermore, there are not much difference between valid misclassification rate and train misclassification rate, indicating **the model did not encounter overfitting**. A deeper decision tree can **generalize well in large dataset**, resulting lower misclassification rate.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_2.png)  
From the figure above, we can see that **Tenure** has the highest impact to whether the customer will churn or not. The higher the tenure, the lower the probability that the customer will churn. Apart from that, **complain** is the second variable that impact whether the customer will churn or not. High complains results in customer’s churn. The figure also showed the variables such as **NumberOfAddress**, **CashbackAmount**, **PreferredPaymentMode**, **PreferredOrderCat** and more that will impact to whether the customer will churn or not.  

### Ensemble Methods
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/EnsembleResult_1.png)  
Random Forest has lower misclassification rate in both Valid data and Train Data compared to Gradient Boosting. This indicating that Random Forest perform better than Gradient Bosting. **Random Forest applied bagging**, which build a collection of decision trees with some level of diversity. It may help in capturing different aspects of the data and improve generalization, resulting lower misclassification rate. While **Gradient Boosting applied boosting**, which focuses on correcting errors of previous tree. If the errors are not captured well by the weak learners, it may result in higher misclassifications rate. However, **random forest may encounter overfitting issue** as train misclassifications rate is lower than valid misclassification rate. On the other hand, **gradient boosting did not encounter overfitting issue** as the train misclassification rate close to the valid misclassification rate.  

In overall, the **decision tree – max levels has the lowest valid misclassification rate among other models**. This interpreting that if the decision tree is constructed properly, it can outperform than any other robust model like Random Forest. Apart from that, **the feature importance assigned in Decision Tree and Random Forest may different**, resulting decision tree perform better than random forest.  

## Reflection or Learning Outcomes
In this study, 3 robust software, including Talend Data Integration, Talend Data Prep and SAS Enterprise Miners are applied for data import and preprocessing, decision tree analysis and ensemble method.  

In Talend Data Integration, I **create an additional date column** for the Kaggle dataset. I use **tRowGenerator** component to create the date column because it allows us to create random date with user friendly interface. As this component is new to me, it took some time for me to understand the way to use it.  

I use Talend Data Prep to clean the noisy and inconsistent data. In Talend Data Prep, I can easily **clean the data by searching the function in the right side pane**. Furthermore, it allows me to view the data information, including the number of missing values.  

To handle missing values and construct the model, I use SAS Enterprise Miner. I can use SAS enterprise to **impute the missing values based on the method** I want as it offers various methods. After that, I **construct a few machine learning models in SAS Enterprise Miner with just a few clicks**. Fine-tuned the model in SAS Enterprise Miner is a challenging part for me. If the model did not find-tuned properly, it could lead to bad performance.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_2.png)  
Based on the figure above, we can see the feature importance that could help in analysing customer behaviours and suggest the best business strategy. For instance, the figure showed the **tenure and complain are top 2 important factor** that impact the customers. Thus, to retained customers, e-commerce company should ensure low number of complain from customers, so that the customers will not churn. Furthermore, we can also see the **cash back amount and preferred payment mode** are also the important factors that affect the loyalty of customers. Thus, marketing manager should think of a great strategy that allow them to offer great cash back to customers while the payment team should offer variety of payment mode to customers.  

In conclusion, this study offers valuable insights into customer behaviour and suggestion for business strategies through a set of software.  

