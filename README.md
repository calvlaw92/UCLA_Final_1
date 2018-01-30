# Abalone

**Domain**<br/>
This problem is drawn from the analysis of the abalone dataset on the UCI Machine Learning Repository, which contains the physical measurements of 4177 abalones collected in Tasmania in 1994. There are many machine learning studies that have been done using this dataset, such as the improvement of the training speed of neural network through the use of the Extreme Learning Machine technique. (Bas et al., 2008)<br/>

**Problem Statement**<br/>
Similar to a counting rings on a tree, the rings on an abalone is able to roughly predict the age of an abalone. It is estimated that an abalone will grow one ring a year, however due to variables such as environmental factors and weather patterns this does not always hold true, this just shows that there are many variables that are missing that can improve the accuracy in this study. The number of rings are counted by researchers after cutting the shell and staining it. As the rings are not always clear, researchers believe that adding 1.5 to the ring count is reasonable in the estimation of an abalone's age. In this study, we will use supervised learning to develop a multiple regression model to predict the number of rings on an abalone based on the attributes Sex, Length, Height, and Viscera weight.<br/>

**Data sets and Input**<br/>
The dataset to be examined is the abalone dataset on the UCI Machine Learning Repository. The dataset contains 4177 rows and 9 columns. The size of the dataset is 187Kb, and the object size is 269528bytes. The dataset contains the column attributes of Sex, Length, Diameter, Height, Whole weight, Shucked weight, Viscera weight, Shell weight and Rings. Given that there are 2 entries with the recorded height of 0, we will discard them as it was likely a mistake due to misrecording. As we will be doing a multiple linear regression, we looked at the collinearity between the attributes, which resulted in narrowing down the attributes to be used in this study to Sex, Length, Height and Viscera weight.The attached jupyter notebook (data_desc.ipynb) contains a more detailed description on the data as well as the models used in this study.<br/>

**Solution Statement**<br/>
The solution to this problem is to use a linear regression model in the form of a multiple linear regression to estimate the number of rings on an abalone (dependent variable) based on the independent variables Sex, Length, Height annd Viscera weight.<br/>

**Benchmark Model**<br/>
Given that we seek a regression model, a good naive benchmark would be to use the mean of the Rings, which is the dependent variable.<br/>

**Evaluation Metrics**<br/>
We will use the R-squared metric and the Root Mean Squared Error(RMSE) to measure the success of our model.<br/>

**Citations**<br/>
Bas,P, Jutten,C, Lendasse,M, Miche,Y, Simula, O. 2008. A methodology for Building Regression Models using Extreme Learning Machine: OP-ELM. European Symposium on Artificial Neural Networks. https://pdfs.semanticscholar.org/d0be/fda52dbd3184d5396548169ada7437c3ea5c.pdf
