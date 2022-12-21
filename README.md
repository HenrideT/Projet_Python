# Projet de Python pour la data-science (OMI2F2) : Prédiction de la réélection des maires français
**Professeur**: M. Lino Galiana

**Chargée de TD**: Mme. Nina Vesseron

**Membres du groupe**: Kilian Andru, Henri de Tricornot, Xavier Lacour

# Ordre des Notebooks
1 - Récupération

2 - Statistiques decriptives

3 - Modélisations

# Introduction

<p style='text-align: justify;'> Notre projet a pour thème les élections municipales françaises. Nous allons essayer de prédire si le maire en place est réélu aux élections municipales suivantes ou non en se basant sur celles de 2014 et 2020. Pour ce faire, nous allons utiliser quatre bases de données.
    
<p style='text-align: justify;'> La première regroupe l’ensemble des maires élus en 2014. Celle-ci est assez simple d’utilisation puisque la liste des maires est donnée. L’élection de 2020 ne comporte pas de base de données la résumant de façon synthétique : nous avons dû en exploiter deux. La première donne les noms des maires élus au premier tour alors que la seconde met à notre disposition les résultats du second tour lorsqu’il y en a eu un. Finalement, la dernière base de données regroupe par ville un ensemble de données socio-économiques à plusieurs dates (telles 2013 et 2019 ce qui correspond aux années précédant les élections municipales, celles-ci ayant lieu tous les six ans). 
    
<p style='text-align: justify;'> Après avoir récupéré les données, nous proposerons quelques statistiques descriptives liées aux maires et aux données socio-économiques municipales. Puis nous proposeront quelques comparaisons entre différents modèles afin de tenter de prédire la réélection d’un maire. Jacques Chirac avait dit « Il faut voter avec son intelligence et non avec ses tripes », si nos concitoyens ont suivi ce précepte, prédire les maires selon les données socio-économiques devrait être possible.

<img src="https://images.rtl.fr/~c/1155v769/rtl/www/1313193-jacques-chirac-le-9-mars-1981.jpg">

# Résultats principaux 

<p style='text-align: justify;'> Nous avons essayé de mettre en place plusieurs modèles afin de prévoir la réélection des divers maires : régressions dites lasso, régressions logistiques, k plus proches voisins, SVM ou encore un réseau de neurones. Aucun n’a été efficace : ils étaient soit similaires soit inférieures au modèle donnant toujours le maire gagnant. On en conclut que les données socio-économiques d’une ville ne sont pas suffisantes pour prédire si un maire va être réélu. Cela pouvait être pressenti sachant qu’on a observé très peu de corrélations significatives entre les variables explicatives et l’élection des maires lors des statistiques descriptives. Prendre en compte des données telles que la proximité du maire par rapport à ses concitoyens, son penchant politique – potentiellement comparé aux tendances nationales - ou encore la conjoncture (l’élection 2020 a eu lieu pendant la pandémie du Covid-19) pourraient être utiles afin d’éclaircir le sujet. On pourrait également conclure que les électeurs n’ont peut-être pas suivi le conseil de Jacques Chirac cité plus haut…
