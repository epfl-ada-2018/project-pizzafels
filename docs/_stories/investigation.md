---
layout: default
category: investigation
title: Investigation of Car Accidents Factors in Switzerland since 1992
id: 1
---
<!--- category : Enter the category here in description, correlation, prediction. You can create new ones in '_config.yml' -->
<!--- title : Set the name to the precise part -->
<!--- id : The id is just to set the order of the parts inside a category -->




<!--- The title set above is already a level 2 title so use only title with 3# or more -->
### Who are the most dangerous drivers in Switzerland?  
<br />

This question is important for policy makers as well as insurance companies since it underlines which category of the population has the higher responsibility in the issue of car accidents. The easiest categories to study are gender and age, and it first seems intuitive that young drivers with less experience are generating more accidents than experienced ones. However, with experience might arise some unsecure driving habits such as stopping using the indicator before turning, that's why a study according to driver's habits is also proposed. Finally, some data about illegal drivers are provided.
<br />
<br />


#### Dangerous categories according to gender and age

When splitting the drivers into multiple categories according to their age and gender profiles, it becomes possible to compare the dangerousness of those profiles. In the following graph, the number of accidents are normalized by the Swiss population corresponding to each category. Only the top 5 more dangerous drivers categories are illustrated below.
<br />
<br />


<p align="center">
<iframe src="img/plotly/accident_sexe&age_top5.html" height="450" width="75%"></iframe>
<br />
</p>
<br />

The most striking observation is that the three most dangerous driving categories are only concerning men and belonging to the three younger driving classes. The only women category of the top 5 corresponds to the age of 20 years old, which is also the more dangerous category for men. We can suppose that at this age, many drivers are still beginners, but they might feel more confident than those of the category 18/19 years old. Finally, the fifth category still corresponds to men, much more experienced in theory but with results in practice very close to the ones of women of 20 years old. When exploring a bit deeper the data, men aged of more than 70 years old come to the 7th position in 2017. However, their accident rate still remains at half of this corresponding to 20 years old men. 

If we now compare the records of 2017 with the ones from 1992, we see a drastical decrease, which was to be expected with the numerous improvements observed around the security of travelers, including the improvements of the cars themselves, but also the stricter rules of today. The decrease is more marked for young people, the number of accidents dropped of 2/3 for men aged 20!
<br />
<br />

#### *Fun fact!*

We can interestingly see that more than 1 in 20'000 men is involved in an accident before 18 years old ! Back 25 years ago, some boys even younger than 10 years old were involved as drivers in car incidents.

Nicely, we can see that in 2017, women did not have any accident before the legal age to drive a car in Switzerland, i.e. 18 years old, which wasn't the case 25 years earlier. However, men younger than legal age are still responsible of car accidents in 2017, which will be detailed below. 
<br />
<br />

#### Dangerous categories according to driving experience

We discussed above the number of accidents according to the age of drivers, however a 25 years-old driver might have only his/her driving licence since a few days. Therefore, the following plot shows the number of accidents according to driver's experience, and lets us see if any counter-intuitive value comes out. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_driving_licence.html" height="450" width="75%"></iframe>
<br />
</p>
<br />

The results are as expected: one can easily see that the more experienced the people are, the less accidents they provoque. As before, and especially for new drivers, we observe a kind of pick in the early 2000's, but the tendency has been clearly decreasing in the past years.
<br />
<br />

#### Dangerous categories among illegal drivers

Some of the drivers responsible of accidents were not possessing any driving license, and were therefore illegal. To which category did the most dangerous illegal drivers belong? Were these drivers representing a significant part in their category? Let's check that on next graph. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_illegal_driver.html" height="450" width="75%"></iframe>
<br />
</p>
<br />

Among illegal drivers and as in previous cases, it is clear that young men below 29 years old are the most dangerous. However a new category of drivers has entered the game: the 15-17 years old. Clearly because of their very low experience, these drivers were on the first step of the podium in 2017. In addition to being more secure, women drivers are also more legal, since only a tiny part of women drivers involved in a car accident was not possessing a licence. They only appear on the 5th step of the top 5. 

Now let's compare men 18-19 year old men involved in an accident legally and illegally. We can see that out of 10'000 people from their category, 34.5 have legally provoked an accident in 2017, whereas only 0.32 did it without any licence. As a result, round 1% of young men involved in an accident in 2017 didn't were not allowed to drive.  
<br />

### Who are the most vulnerable victims of car accidents? 
<br />

Between drivers, passengers and pedestrians, which category has been the most exposed to car accidents? Let's check it out in the table below. 
<br />
<br />

<p align="center">

<iframe src="img/dataframesly/victims_sum.html" height="200" width="50%"></iframe>
<br />
<i>Table of victims for the 3 categories</i>
</p>
<br />

We can see the expected drop in the number of victims in 25 years. In the table above, we can clearly distinguish a difference between the pedestrian victims and the car passengers. The pedestrian are indeed not protected by the car, the security of which has been greatly improved. That's why we can note a lower drop in pedestrian victims compared to car passengers. 

Similarly to pedestrians, the number of car drivers has also decreased of only round 20%, compared to 50% for passengers. Therefore, decreasing the security of drivers should become a higher priority, even though it seems to be more challenging for car manufacturers. 
<br />
<br />

#### *Analysis of pedestrian victims*

We measured a 20% decrease in pedestrian victims since 1992. But does it mean a similar improvement for all age categories of walkers? And who among pedestrian victims are most vulnerable to car accidents? 

The first table measures the exposure of various age categories to car accidents regardless the gravity. 
<br />
<br />

<p align="center">

<iframe src="img/dataframesly/pedestrian_victims.html" height="250" width="50%"></iframe>
<br />
<i>Table of pedestrian victims in the top 5 more exposed</i>
</p>
<br />

Interestingly, and quite sadly, we can see that the young people are the prior pedestrian victims. It even increased since 1992 for people between 15 and 20 years old. However, it clearly dropped for younger children, which is consolating.

Let's measure in a second table the number of pedestrian victims who strictly died from a car accident. 
<br />
<br />

<p align="center">

<iframe src="img/dataframesly/pedestrian_victims_death.html" height="250" width="50%"></iframe>
<br />
<i>Table of the top 5 dead pedestrian victims</i>
</p>
<br />

Interestingly, the categories are now completely different! Older people are more likely to die from an accident: they are indeed involed in less accidents while resulting in more deaths. We also sadly find very young children in the top 5 of the deadliest categories.

Following this tragic part of the analysis oriented on victims, it would be pleasant to find recommendations for drivers to increase their awareness about the sensible periods and circumstances under which they should be more careful. 
<br />
<br />

### During which period should drivers be more careful? 
<br />

#### The trap of accidents per month

Under which road circumstances are most of the accidents taking place? The answer to that question is illustrated in next bar plot.
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_circumstances.html" height="450" width="75%"></iframe>
</p>
<br />

The first accident circumstance is therefore due to skidding, which not only depends on a driving action but also on the weather. Therefore, it seems intuitive that the more dangerous months should be in winter, when the road is more likely to be covered with ice or snow. This intuition is verified in next plot. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_month.html" height="450" width="75%"></iframe>
</p>
<br />

Que pasa?! It looks like the number of accidents is higher in summer than winter, which is counter-intuitive! Moreover, the 6 months with most accidents due to skids are also from may to october, definitely the contrary of what was initially supposed. During summer months, drivers might think that the risk of skid is absent, and thus lack of caution. In the contrary, winter months are known to be more slippery, and drivers might increase their vigilence, consequently reducing the number of skids. A friend of mine lived the experience of skidding last month of June and he had to repay two trees that he destroyed to the municipality, so he won't deny that!

To conclude, if you wish to contribute decreasing the number of car accident victims, please be careful about the stability of your vehicle when you drive under the rain, even in summer :)

#### The rule of weekdays accidents

Another trend of accident periods should be studied at the timescale of weekdays this time. Let's give a look at the number of car accidents per hour from thursday to sunday in the next plot. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_special_day.html" height="450" width="75%"></iframe>
</p>
<br />

Apart from Saturdays and Sundays, all the week days are following a similar same distribution, that's why only Thursdays and Fridays have been shown. We identify two peaks: one in the morning and one between 17h and 19h: this corresponds to the starting and ending working hours and is as expected. Throughout the Friday afternoon, more accidents are occuring compared to Thursday. This might be due to the excitement of workers finishing earlier their hard week, but unfortunately lacking of caution and then BOOM getting struck by a bus! Life is unfair sometimes...

Concerning the weekends, when people don't work, the patterns are clearly different, the two peaks corresponding to the work hours disappeared and we observe less accidents in general. However, we see more of them in the early hours of the day, probably explained by the end of Fridays and Saturdays night. When comparig Thursday and Friday morning between 0-2h, the Jeudredi is also identified with higher rates of accidents. Overall, Sunday appears to be the chillest day in terms of accidents. 

It is commonly agreed that drivers are having more accidents on Friday and Saturday night because of their consumption of substances that have an impact on human's behavior and awareness faculty. Therefore, the last part of our brief investigation is dealing with substances consumed before car accidents. 
<br />

### Which substances should be the most monitored by the police? 

Mentioning Jeudredi and other night events above, the question of substance contribution to accidents is key. Which substance is the most commonly involved in car accidents? This is illustrated in next plot. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_known_substances.html" height="450" width="75%"></iframe>
</p>
<br />

Even though most of the accidents were not the consequence of any illegal substance, the key substance leading to accidents in Switzerland is clearly the alcohol. Indeed, in 2017, 411 accidents implying strict alcool consumption were counted, whereas only 71 for the second substance (drugs). It is moreover clear that the issue of alcool-related accidents has been well tackled by the Swiss government and citizens since it has decreased of 58% over last 25 years (not even considering the normalization to a growing population).  

What about the influence of other substances on car accidents? To observe it, the contribution of alcool has been removed from the graph. 
<br />
<br />

<p align="center">
<iframe src="img/plotly/accident_substances_noalcool.html" height="450" width="75%"></iframe>
</p>
<br />

Interestingly, the accidents ensuing from alcohol have had a decreasing trend over the last 25 years, however this trend is not observed for all the other substances! The more striking case is concerning drugs, which led to only 40 accidents in 1992, and reached more than 70 in 2017. The involvement of medicaments has also increased in the number of accidents, from 10 to 41 in 2015, before starting decreasing last 2 years. Therefore, it looks like all the government's efforts have been oriented towards alcool monitoring, which is understandable because of the wider impact of this substance on the number of car accidents compared to drugs and medicaments. 
