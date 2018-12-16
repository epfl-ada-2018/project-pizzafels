---
layout: default
category: ML_based_study
title: Study of Car Accidents per Canton based on ML
id: 1
---
<!--- category : Enter the category here in description, correlation, prediction. You can create new ones in '_config.yml' -->
<!--- title : Set the name to the precise part -->
<!--- id : The id is just to set the order of the parts inside a category -->


<!--- The title set above is already a level 2 title so use only title with 3# or more -->

### Methodology

Now that a contextual investigation of car accident factors has been provided for Switzerland, the second part is oriented towards a Machine-Learning model of car accidents at canton scale according to various features. The methodology has been to first gather multiple datasets related to roads/accidents and available for each canton. These data were constituting our input features, and the outcome was the number of car accidents per canton. Finally, the set was trained for each canton over a period from 1996 to 2014, and tested on the value of 2015. This predicted value was then compared to the real one of that year, thus defining a score of accuracy. 

Since the number of values was low, we decided to implement various ML strategies, to compare their accuracy over the 26 cantons and to select the approach with best predictions for 2015. One of the best ML approaches turned out to be the regression tree, which gave more precise results than a simple algorithm for more than 80% of the cantons. The simple algorithm was only based on dates as features, so the tree method shows that other features were useful for predicting car accidents. Our mean error to predict the number of accidents in 2015 was only of 7.38%. 

In addition to its good performance, our selected method also provides visual decision trees. The interesting aspect of decision trees is that they show the most influent factors at level 0, and then each time the tree level increases, the influence of features decreases. An example of decision tree is provided below for Appenzell Ausserrhoden:
<br />
<br />

<p align="center">
<img src="img/graphs/AA_3.png" alt="My Image" height="75%" width="75%">
<br />
<i>Decision tree of car accidents in Appenzell Aus.</i>
</p>
<br />

We can see that for the feature at the top level, the 'mse' indicator is higher than for lower level features. Indeed, high 'mse' means a high contribution to lowering the variance of the model. Therefore, the higher the 'mse' and the more contribution our factor has in the outcome, that's to say in the number of car accidents. 

### Which factors are the most influent?
<br/>

#### Influent factors per canton

Since each canton has different influent factors at the top levels of its decision tree, it can be interesting to see which factors have more influence according to the canton. Therefore, a tool is provided to get the top level factors for each canton: 

<p align="center">
<iframe src="img/plotly/htmlTEST.html" height="280" width="90%" frameBorder="0"></iframe>
</p>

Despite its very "appealing" look, this tool can show us that some factors are significant only for few cantons, whereas some others are more constantly important such as 'Road Expenses' for example. 
<br/>
<br/>

#### Influent factors overall cantons

To check which factors are the most frequently influent in Swiss cantons, a new table is shown below with the most recurrent key factors throughout our 26 cantons. 

<p align="center">
<iframe src="img/plotly/top_feat_overall.html" height="380" width="80%"></iframe>
<br />
</p>

From previous bar plot, it seems obvious that 'expenses in roads' are the key factor in Switzerland. Indeed, they are the features that are the most often called at top level of decision trees in our model when considering the 26 cantons. The question remains to know wether the contribution of 'road expenses' has a positive or negative correlation with the number of car accidents. In other words, should decision makers increase or decrease the 'road expenses'? Next section is aimed at answering this question by showing visual graphs of relation between car accidents and some key features of the model.
