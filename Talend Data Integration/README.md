# Data Manipulation
The [E-commerce Dataset.csv](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/E%20Commerce%20Dataset.csv) was imported to Talend Data Integration for data manipulation. A Date column named LastPurchaseDate is added to the dataset as the dataset did not contain any date column. Date column is important as it allows us to analyse the trend over time. Thus, a random date was added to each row by using Talend Data Integration.

## Step 1 - tFileInputDelimited
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_1.png)  
- A tFileInputDelimited component was dragged into the designer. I have changed the saved file destination, row separator, field separator and skip empty rows as figure above. After that, click the 3 dots beside edit schema.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileInputDelimited_2.png)  
- A window popped out, and I filled up all the variable name and types. This steps to make sure we can import all columns into Talend.  

## Step 2 - tRowGenerator
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tRowGenerator_1.png)  
- A tRowGenerator was dragged to the designer to generate random date for all the rows in input files.

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tRowGenerator_2.png)  
- In edit schema, I created 2 new columns with name and type.  

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tRowGenerator_3.png)  
- In RowGenerator Editor, I selected the functions and environment variables for both column. CustomerID is used for joining input file and LastPurchaseDate will be mapped to input file.  

## Step 3 - tMap
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tMap_1.png)  	 
- A tMap was dragged to the designer. tFileinputDelimited and tRowGenerator should be connected to tMap as figure above. To edit in tMap, double click the tMap

![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tMap_2.png)  
- I linked the CustomerID from input file to CustomerID from Generator as figure above. After linked, an output is created, and I dragged all the columns into it.

## Step 4 - tFileOutputDelimited
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/tFileOutputDelimited_1.png)  	 
- A tFileOutputDelimited was dragged into designer. I have changed the output file destination, row separator, field separator and include header as figure above. Once done, we can run it.  

## Final Workflow
![Updated Image](https://github.com/weilai0807/WQD7005_AA1/blob/main/Talend%20Data%20Integration/FinalWorkflow.png)  	
[AA1_output.v1.csv](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/AA1_output.v1.csv) was generated, it consists of 26 columns and 5631 rows as I have added a new column named LastPurchaseDate to the dataset. Figure above shows the message of successfully generating output in Talend Data Integration.
