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

Now that a contextual investigation of car accident factors has been provided for Switzerland, the second part is oriented towards a Machine-Learning model of car accidents at canton scale according to various features. The methodology has been to first gather multiple datasets related to roads/accidents and available for each canton. These data were constituting our input features, and the outcome was the number of car accidents per canton. Finally, the set was trained for each canton over data from 1996 to 2014, and tested on the value of 2015. This predicted value was then compared to the real one of that year, thus defining a score of accuracy. 

Since the number of values was low, we decided to implement various ML strategies, to compare their accuracy over the 25 cantons and to select the approach with best predictions for 2015. The best ML approach turned out to be the regression tree, which also provides visual decision trees. 

<p align="center">
<img src="img/graphs/AA_8.png" alt="My Image" height="75%" width="75%">
<br />
<i>Exemple for a legend</i>
</p>
<br />
<br />
<br />

#### What are the main factors influencing the number of accidents per canton?

For each canton, the most influent factors are the ones from top levels of the decision tree. Therefore, a tool is provided to get the five more important factors for each canton: 

**Dynamic tool de BG**


