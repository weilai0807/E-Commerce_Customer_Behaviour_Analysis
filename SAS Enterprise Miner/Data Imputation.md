# Data Imputation
[AA1_output.v2.xlsx](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/AA1_output.v2.xlsx) is imported to SAS enterprise Miner for imputation as there are some missing values in dataset.  

## Step 1  
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/FileImport_1.png)  
- A File Import node was dragged to the diagram to import the file. I changed the file destination in Import File under Train. Once done, run the file import node.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/FileImport_2.png)  
To set up the correct role and level for dataset, I edit the variables by right clicking the node. A window popped up and I adjust the role and level as figure above. Once done, click OK.  

## Step 2
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Impute_1.png)  
A Impute node was dragged to the diagram, and I connected the file import node to Impute node. Once done, run it.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/Impute_2.png)  
After run, right click the Impute node and select edit variable. A window popped out, and I can select the columns that contain missing values for imputation. I selected mean method for interval column and tree method for nominal method. Once done, click ok and run the node again.  

## Result
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/SAS%20Enterprise%20Miner/ImputeResult.png)  
From the figure above, we can know the variable name and impute method that selected for imputation. We also can know the impute value and number of missing values for train. 
