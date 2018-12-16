---
layout: default
category: correlation
title: Correlation between influent factors and accidents in cantons
id: 1
---
<!--- category : Enter the category here in description, correlation, prediction. You can create new ones in '_config.yml' -->
<!--- title : Set the name to the precise part -->
<!--- id : The id is just to set the order of the parts inside a category -->




<!--- The title set above is already a level 2 title so use only title with 3# or more -->

### Correlation with cantonal road expenses


In previous section, the ML tree model has determined "road expenses" as a highly influencing factor of car accidents. To plot the relation between both variables, the number of accidents has been normalized by 1000 people living in the canton, and the road expenses have been normalized by 100km of road distance in the canton. Because of this normalization by road distance, the canton of Basel Stadt was always an outlier (urban canton), therefore it has been removed from the maps. 

Below, we can see the map of road distance per canton, as well as the plot of car accidents versus the road length for cantons whose correlation fits into a 95% confidence interval. 
<br /> 
<br /> 

<div class="row">
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/maps/expenses_road_canton.html" height="450" width="100%"></iframe>
    	<center> <i>Map of expenses in roads</i></center> 
    </div>
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/plotly/correlation_expenses_roads_zoomin.html" height="450" width="100%"></iframe>
    	<center><i>Plot of victims versus road expenses</i></center>
    </div>
</div>
<br /> 

A clear negative correlation between road expenses and car accidents appears. One could argue that it is because roads become safier with more spendings in the renovation, however we are only showing a correlation here, and not an explicit relation of causality. The number of accidents might have decreased in the time for other reasons than an increase in road expenses. 

<br />
### Correlation with cantonal police expenses

In 6 cantons, police surveillance is among the top 3 levels of the decision tree, such as TG and OW for example. Therefore, it is worth to check the relation between accidents and this variable. As before, a map is provided with the police expenses normalized per 100km of roads in each canton. Besides, a plot of the relation with car acidents is shown for cantons with 95% confidence of correlation.
<br /> 
<br /> 

<div class="row">
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/maps/expenses_police_canton.html" height="450" width="100%"></iframe>
    	<center><i>Map of expenses in police</i></center>
    </div>
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/plotly/correlation_expenses_police.html" height="450" width="100%"></iframe>
    	<center><i>Plot of victims versus police expenses</i></center>
    </div>
</div>
<br /> 

One more time, expenses seem to be justified. The higher the expenses in police surveillance, the lower the number of accidents. However, this is only representative of cantons with a high confidence level, whereas 5 other cantons such as Neuchatel and Vaud are having a positive correlation (>0.6 for both!). As a conequence, no clear conclusion can be drawn for Switzerland, even despite it is a good indicator for prediction of accidents within each canton. 

<br /> 
### Correlation with vehicles cylinder size

According to the canton, the average cylinder size of vehicles might vary a lot, that's why a formula has derived to compute the cylinder score of cantons. Cylinders are provided into 5 sub-categories, going from 'below 1399 cm3' to 'above 2500 cm3'. 

To have a general idea of the kind of cars used in each canton, we thus decided to build a score for it. We give more weight to cars with bigger cylinders and normalize it to get the final score between 0 and 1:  
<!-- <center> $$ Score = \frac{0.2x_0 + 0.4x_1 + 0.6x_2 + 0.8x_3 + x_4}{\sum_i{x_i}} $$</center>
where each $x_i$ corresponds to one of the category, from $x_0$ for the smallest cylinder to $x_4$ for the biggest one.  -->
In words, this describe how "big cylinders" friendly a canton is.

Besides the map of cylinder score per canton below, we can then look at the correlation between this and the number of victims:
<br /> 
<br /> 

<div class="row">
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/maps/cylinder_score_canton.html" height="450" width="100%"></iframe>
    	<center><i>Map of cylinder score</i></center>
    </div>
    <div class="col-xs-12 col-md-6">
    	<iframe src="img/plotly/correlation_car_cylinders_best.html" height="450" width="100%"></iframe>
    	<center><i>Plot of victims versus cylinder scores</i></center>
    </div>
</div>
<br /> 

For Grisons and Schwytz (most confident cases), it seems that we have a soft negative correlation.

Again, the correlation is only significant for a few cantons, namely 11. What is worse, part of them exhibit positive correlations while others have negative ones. It it thus impossible to draw any conclusion from this data.

However, it is interesting to look at the shape of the scatter plots of both cantons: if you go from the highest to the lowest point (decreasing number of victims, the observed trend in time), you will first move right then left. This corresponds to the evolution in time of the "cylinder score" of the two cantons.
<br /> 

### Correlation with gear boxes

We can also look at the different gear boxes: does the number automatic vehicles influence the number of accidents? Or for it to be more meaningful across the different cantons, does a higher share of automatic vehicles on the road influence the number of accidents?
<br /> 
<br /> 

<p align="center">
<iframe src="img/plotly/correlation_gear_box_best.html" height="450" width="75%"></iframe>
</p>
<br />

The results are more interesting than before: 16 cantons (61.5%) exhibit a clear and significant negative correlation between the number of accidents and the percentage of automatic vehicles with a confidence of 95%.
<br /> 

### Summary

One must firstly keep in mind that we cannot draw any significant conclusions from this analysis since a corrélation doesn't always imply a causality, as it is famously known. Actually, throughout our analysis, we were focused on the normalized number of victims on a yearly basis, which has a clear decreasing tendency for every canton. But it is really hard to identify factors explaining it, or at least on a global scale.

Note that we also analyzed other features (length of the roads in the cantons, health budget, expenses of the households, other informations on the cars, ...) but decided to restrain ourselves to the most interesting ones in this notebook.

If we now treat the cantons separately, then the expenses or the type of cars in the cantons might influence the number of accidents in some or the other canton, as shown above. Then, correlations can be identified. But the same problem still arises: is it really explaining the number of accidents ? Probably not, or at least not if taken individually.

To try to gain some deeper insight in it, we thus decided to put everything we have in a machine learning setting and to run differrent algorithms to see if we can identify more complex relations between those features and the resulting number of accidents. 