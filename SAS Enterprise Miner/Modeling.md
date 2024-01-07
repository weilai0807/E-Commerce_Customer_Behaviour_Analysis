Data Partition	 
1. A data partition node was dragged into the diagram, and I connected the impute node to data partition node. After that, I change the data set allocation to 70 for training, 30 for validation and 0 for testing.

Decision Tree node	 
1. 3 decision trees node were dragged into the diagram. In Decision Tree – Max levels, I leave all the settings by default. 
2. in Decision tree – 3 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 3 levels as shown in figure above.
3. In Decision tree – 2 levels, I leave all the settings by default, except the interactive under Train. After I clicked the 3 dots under interactive, a window popped up, and I adjust the node to 2 levels as shown in figure above.

Gradient Boosting	 
1. A Gradient Boosting node was dragged into the diagram, and I connected the data partition node to it. I leave all the setting by default.
HP Forest	 
2. A HP Forest node was dragged into the diagram, and I connected the data partition node to it. I leave all the setting by default.

Model Comparison	 
1. A model comparison node was dragged into diagram and connected by all the models. The node is used for comparing the performance of models. Once connected, run the model comparison node.
