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
### Focusing the analysis at canton scale: Machine-Learning approach

#### Methodology

Now that a contextual investigation of car accident factors has been provided for Switzerland, the second part is oriented towards a Machine-Learning model of car accidents at canton scale according to various features. The methodology has been to first gather multiple datasets related to roads/accidents and available for each canton. These data were constituting our input features, and the outcome was the number of car accidents per canton. Finally, the set was trained for each canton over a period from 1996 to 2014, and tested on the value of 2015. This predicted value was then compared to the real one of that year, thus defining a score of accuracy. 

Since the number of values was low, we decided to implement various ML strategies, to compare their accuracy over the 25 cantons and to select the approach with best predictions for 2015. One of the best ML approaches turned out to be the regression tree, which gave more precise results than a simple algorithm for more than 80% of the cantons. The simple algorithm was only based on dates as features, so the tree method shows that other features were useful for predicting car accidents. Our mean error to predict the number of accidents in 2015 was only of 7.38%. 

In addition to its good performance, our selected method also provides visual decision trees. The interesting aspect of decision trees is that they show the most influent factors at level 0, and then each time the tree level increases, the influence of features decreases. An example of decision tree is provided below for Appenzell Ausserrhoden:
<br />
<br />

<p align="center">
<img src="img/graphs/AA_8.png" alt="My Image" height="75%" width="75%">
<br />
<i>Decision tree of car accidents in Appenzell Aus.</i>
</p>
<br />

On previous graph, the top level features are 'electric fuel' at level 0, 'diesel fuel' and 'cantonal road expenses' at level 1. 

#### What are the main factors influencing the number of accidents per canton?

Since each canton has different influent factors at the top levels of its decision tree, it can be interesting to see which factors have more influence according to the canton. Therefore, a tool is provided to get the top level factors for each canton: 

<p align="center">
<iframe src="img/plotly/htmlTEST.html" height="280" width="90%" frameBorder="0"></iframe>
</p>
<br />

