# Modeling Steps
Once the data preprocessing is done, we can proceed to decision tree analysis. The table below shows the steps of decision tree analysis.  

Step 1 - Data Partition node 
- A data partition node was dragged into the diagram, and I connected the impute node to data partition node. After that, I change the data set allocation to 70 for training, 30 for validation and 0 for testing.

- 3 decision trees node were dragged into the diagram. In Decision Tree – Max levels, I leave all the settings by default. 
 
- In Decision tree – 3 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 3 levels as shown in figure above.
 
 
- In Decision tree – 2 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 2 levels as shown in figure above.
 
- A model comparison node was dragged into diagram and connected by all decision tree models. The node is used for comparing the performance of models. Once connected, run the model comparison node.
