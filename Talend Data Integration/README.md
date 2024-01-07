# Data Manipulation
The [E-commerce Dataset.csv](https://github.com/weilai0807/WQD7005_AA1/blob/main/Dataset/E%20Commerce%20Dataset.csv) was imported to Talend Data Integration for data manipulation. A Date column named LastPurchaseDate is added to the dataset as the dataset did not contain any date column. Date column is important as it allows us to analyse the trend over time. Thus, a random date was added to each row by using Talend Data Integration.

## Step 1
![Updated Image](https://github.com/username/repository/blob/main/path/to/new_image.png)
A tFileInputDelimited component was dragged into the designer. I have changed the saved file destination, row separator, field separator and skip empty rows as figure above. After that, click the 3 dots beside edit schema.
2. A window popped out, and I filled up all the variable name and types. This steps to make sure we can import all columns into Talend. 

tRowGenerator	 
1. A tRowGenerator was dragged to the designer to generate random date for all the rows in input files. 
2. In edit schema, I created 2 new columns with name and type.
3. In RowGenerator Editor, I selected the functions and environment variables for both column. CustomerID is used for joining input file and LastPurchaseDate will be mapped to input file.

tMap	 
1. A tMap was dragged to the designer. tFileinputDelimited and tRowGenerator should be connected to tMap as figure above. To edit in tMap, double click the tMap
2. I linked the CustomerID from input file to CustomerID from Generator as figure above. After linked, an output is created, and I dragged all the columns into it. 

tFileOuputDelimited	 
1. A tFileOutputDelimited was dragged into designer. I have changed the output file destination, row separator, field separator and include header as figure above. Once done, we can run it.
