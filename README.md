# Study of the influence of driver profile, canton and vehicle type on car accidents in Switzerland

## Abstract (Unchanged since Milestone 1)

​	In 2017, there were 17,799 accidents on Swiss roads causing body injuries. Even though the number of victims is decreasing since 25 years, Switzerland still faces around 20,000 victims each year. In this data story, we try to investigate three main factors influencing car accidents: driver profile, accident per canton and car type. Identifying which profiles are more dangerous is an interesting result for policy makers and insurance companies, considering an annual cost of car accidents equal to 4 billion francs. Factors of difference between each profile are also a targeted, to tackle the issue at its roots. Furthermore, Swiss cantons benefit from a high political responsibility. Studying the distribution of accidents at this scale is therefore valuable, as well as their potential cultural factors based on past votings (e.g. which cantons voted for or against higher speed limitations or the obligation to put the seat belts on). Finally, a study of the vehicle type's influence on accidents is also carried out. All datasets used in this study were collected on the Federal Statistical Office website.

## Milestone 2

We cleaned the chosen datasets to start our analysis. This allowed us to have a better insight on what is and isn't possible to do with it. We can thus give a first answer to our original research questions, as presented below.

### Research Questions from Milestone 1 and Insights of Answers towards Milestone 3

1) Is there a high influence of the driver profile (age, gender, driving experience) on car accident risk?

> At the stage of milestone 2, we have already cleaned and normalized the data of accidents per drivers profiles, where an interesting history of women accidents responsibility can be shown. Some profiles have been observed more dangerous than others, thus responding to the question. 

2) What could be the main factors triggering that difference between driver profiles?

> The main issue that we have had is that the dataset for drivers profiles is aggregated, which limits us in finding correlations with other datasets, especially at a broad national scale. Therefore, we have contacted the Federal Statistical Office to see if it is possible to have access to raw data of individual accidents. 

> Remark: We would like to extend the first part of our work to a generall contextualization of car accidents in Switzerland, therefore involving personal actors, victims, but also implied objects and driving environments where accidents took place. These might result in first insights useful to decision makers. 

3) Based on votations and urban data, what could be the main factors triggering the difference of accidents between cantons?

> To establish the factors of difference of accidents between cantons, we have download many datasets about road policy in cantons, household expenses in alcool and public transport as well as type of cars used per canton. A link between votations and our results about cantonal accidents will be studied.

4) Does car type have an influence on car accidents? 

> This question will be already answered in the comparative canton-scale study from question 3.

5) Based on our results, can we identify uesful recommandations for insurance companies or policy makers?

> The first part should illustrate more dangerous profiles and therefore provide interesting insights to insurance companies. On the other hand, the second part at scale of cantons should come out with some correlations between factors and number of accidents, therefore potentially useful for policy makers, especially at canton scale.


### Dataset

​	Since we have discovered that all our datasets provide accidents with aggregated numbers (and not individual IDs), we have decided to download more datasets at the scale of cantons to study correlations between various factors and the bigger amount of data that we have when splitting it into cantons. Here is the list of additional datasets:  

- [Dépenses détaillées des ménages selon le canton (seulement les cantons les plus peuplés)](https://www.bfs.admin.ch/bfs/en/home.assetdetail.1400701.html) 
- [Recettes des cantons pour les routes](https://www.bfs.admin.ch/bfs/en/home.assetdetail.5286939.html )
- [Besoins financiers nets des cantons et des communes pour la santé - Total](https://www.bfs.admin.ch/bfs/de/home/statistiken/kataloge-datenbanken/medienmitteilungen.assetdetail.6386476.html)
- [Routes nationales par canton: longueur totale par type de route](https://www.bfs.admin.ch/bfs/fr/home/statistiques/catalogues-banques-donnees/tableaux.assetdetail.3644575.html)


### A list of internal milestones up until project milestone 3

​	We have three weeks left to describe clearly the context of car accidents in Switzerland, find which factors have relevant correlations with cantons accidents, realize a predictive strategy based on resulting correlations, and finally create our full data story. 

- A notebook has already been started studying correlations between collected features and cantons accidents. 

<u>Until 2nd of November:</u>
- Describe clearly the context of car accidents in Switzerland (based on drivers profiles, objects, route type and victims) 

- Re-contact the FSO to get chances of having access to a more granular dataset of Swiss accidents

- Find which features have a clear influence on cantons accidents and which have no particular correlation 


<u>Until 9th of November:</u> 
- Start clear and good looking visualizations for the national contextualization of the topic

- Propose a predictive model based on previously found relationships between features and cantons accidents (machine learning)


<u>Until 16th of November:</u> 

- Create a link with an attractive data story, easy to follow and with concise description of the outcomes of our study
