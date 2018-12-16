<!-- ---
layout: default
category: correlation
title: Correlation between influent factors and accidents in cantons
id: 1
--- -->
<!--- category : Enter the category here in description, correlation, prediction. You can create new ones in '_config.yml' -->
<!--- title : Set the name to the precise part -->
<!--- id : The id is just to set the order of the parts inside a category -->




<!--- The title set above is already a level 2 title so use only title with 3# or more -->
### Summary

One must firstly keep in mind that we cannot draw any significant conclusions from this analysis since a corrélation doesn't always imply a causality, as it is famously known. Actually, throughout our analysis, we were focused on the normalized number of victims on a yearly basis, which has a clear decreasing tendency for every canton. But it is really hard to identify factors explaining it, or at least on a global scale.

Note that we also analyzed other features (length of the roads in the cantons, health budget, expenses of the households, other informations on the cars, ...) but decided to restrain ourselves to the most interesting ones in this notebook.

If we now treat the cantons separately, then the expenses or the type of cars in the cantons might influence the number of accidents in some or the other canton, as shown above. Then, correlations can be identified. But the same problem still arises: is it really explaining the number of accidents ? Probably not, or at least not if taken individually.

To try to gain some deeper insight in it, we thus decided to put everything we have in a machine learning setting and to run differrent algorithms to see if we can identify more complex relations between those features and the resulting number of accidents. 