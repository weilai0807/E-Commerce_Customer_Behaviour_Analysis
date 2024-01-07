# Data Cleaning
To clean the noisy and inconsistent data, Talend Data Prep was used. [AA1_output.v1.csv](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/AA1_output.v1.csv) was imported into Talend Data Prep for data cleaning.

## Step 1
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/Prep_1.png)  
1. The CustomerID was detected as postal code data type after I imported the data into Talend Data Prep. Thus, I change it to text data type.  

## Step 2
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/Prep_2.png)  
3. There are 3 categories in PreferredLoginDevice column such as Mobile Phone, Phone and Computer. As Mobile phone and Phone are same category, so I replace the phone with mobile phone.  

## Step 3
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/Prep_3.png)  
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/Prep_4.png)  
4. There are 7 categories in PreferredPaymentMode column such as Debit Card, Credit Card, E-wallet, Cash on Delivery, UPI, CC and COD. As CC is same category with Credit Card and COD is same category with Cash on Delivery, so I replace both CC and COD to Credit Card and Cash on Delivery respectively.  

## Step 4
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Prep/Prep_5.png)  
5. There are 6 categories in PreferredOrderCat column such as Mobile Phone, Laptop & Accessory, Fashion, Grocery, Others and Mobile. As Mobile is same category as Mobile Phone, I do the replacement as figure above.  

## Missing Values 
After the data cleaning, I noticed some columns contains missing value in Talend Data Prep. Missing Values will be handled in SAS Enterprise Miner. The table below shows the missing values of the column. 

| Variable                      | Number of Missing Values |
| ----------------------------- | ------------------------ |
| Tenure                        | 264                      |
| WarehouseToHome               | 251                      |
| HourSpendOnApp                | 255                      |
| OrderAmountHikeFromLastYear   | 265                      |
| CouponUsed                    | 256                      |
| OrderCount                    | 258                      |
| DaySinceLastOrder             | 307                      |
| MembershipLevel               | 264                      |

The [data](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/AA1_output.v2.xlsx) is exported from Talend Data Prep for further processing in SAS Enterprise Miner.

