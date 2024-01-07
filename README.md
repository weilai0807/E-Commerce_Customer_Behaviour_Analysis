# WQD7005 Data Mining - Alternative Assessment 1
## Objective
Conduct a comprehensive e-commerce customer behaviours analysis through a set of software, including SAS Enterprise Miner, Talend Data Integration, and Talend Data Prep

## Process Flow
- Step 1 - Data Manipulation with Talend Data Integration. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/README.md)
- Step 2 - Data Cleaning with Talend Data Prep. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/README.md)
- Step 3 - Handled Missing Values with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Data%20Imputation.md)
- Step 4 - Conduct Decision Tree Analysis with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Decision%20Tree%20Analysis.md)
- Step 5 - Apply Ensemble Methods with SAS Enterprise Miner. [Link](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Ensemble%20Methods.md)

## Deliverables
In this study, 3 robust software, including Talend Data Integration, Talend Data Prep and SAS Enterprise Miners are applied for data import and preprocessing, decision tree analysis and ensemble method.  
In Talend Data Integration, I create an additional date column for the Kaggle dataset. I use tRowGenerator component to create the date column because it allows us to create random date with user friendly interface. As this component is new to me, it took some time for me to understand the way to use it.  
I use Talend Data Prep to clean the noisy and inconsistent data. In Talend Data Prep, I can easily clean the data by searching the function in the right side pane. Furthermore, it allows me to view the data information, including the number of missing values.  
To handle missing values and construct the model, I use SAS Enterprise Miner. I can use SAS enterprise to impute the missing values based on the method I want as it offers various methods. After that, I construct a few machine learning models in SAS Enterprise Miner with just a few clicks. Fine-tuned the model in SAS Enterprise Miner is a challenging part for me. If the model did not find-tuned properly, it could lead to bad performance.  
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/DecisionTreeResult_2.png)  
Based on the figure above, we can see the feature importance that could help in analysing customer behaviours and suggest the best business strategy. For instance, the figure showed the tenure and complain is top 2 important factor that impact the customers. Thus, to retained customers, e-commerce company should ensure low number of complain from customers, so that the customers will not churn. Furthermore, we can also see the cash back amount and preferred payment mode are also the important factors that affect the loyalty of customers. Thus, marketing manager should think of a great strategy that allow them to offer great cash back to customers while the payment team should offer variety of payment mode to customers.  
In conclusion, this study offers valuable insights into customer behaviour and suggestion for business strategies through a set of software.  

