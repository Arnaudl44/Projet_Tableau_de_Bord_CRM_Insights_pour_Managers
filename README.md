# 📝 À propos de ce projet

Dans ce projet, j'ai assumé le rôle d'un développeur BI pour concevoir un tableau de bord basé sur une base de données CRM fictive mais réaliste provenant d'une entreprise spécialisée dans la vente de matériel informatique aux grandes entreprises. Ils utilisent un nouveau système CRM pour suivre leurs opportunités de vente, mais n'ont aucune visibilité sur les données en dehors de la plateforme.

J'ai créé un tableau de bord Power BI interactif pour permettre aux directeurs des ventes de suivre les performances trimestrielles de leur équipe. L'objectif était de leur fournir une meilleure visibilité sur les performances de leurs équipes, en s'appuyant sur des données simulées.

## 📊 L'ensemble de données

L'ensemble de données contenait des enregistrements exportés du CRM de la société entre octobre 2016 et décembre 2017. Il contenait des détails sur les opportunités avec des informations associées telles que le produit, le compte et si la vente a été gagnée ou perdue.

## 🕵️ Hypothèses clés

Lors de la création d'un tableau de bord interactif, j'aime toujours discuter avec les utilisateurs pour m'assurer de bien comprendre l'objectif visé et les questions auxquelles ils cherchent à répondre avec le tableau de bord. En l'absence de possibilité de discuter avec les responsables des ventes, j'ai formulé les hypothèses clés suivantes que j'ai utilisées pour guider la conception de mon tableau de bord.

### 🎯 Objectifs principaux des responsables commerciaux

- Comment mon équipe (dans son ensemble et les membres individuels de l'équipe) se comporte-t-elle par rapport à nos indicateurs clés de performance ?
- Certains membres de l’équipe ont-ils besoin d’un soutien supplémentaire dans certains domaines ?
- Sur quoi dois-je concentrer mes efforts pour le reste du trimestre pour améliorer mes performances ?
- Mon équipe est-elle plus performante que la moyenne par rapport au reste de l’entreprise ?

Leur principal indicateur de performance clé est la valeur en euros des ventes réalisées, mais des mesures connexes telles que le nombre de ventes, le pourcentage de conversion et la valeur moyenne des ventes sont également importantes et aident à comprendre leur valeur totale des ventes.

Ils peuvent également parfois vouloir approfondir le sujet et examiner les performances de leur équipe au cours de l'année ou en comparaison avec les autres équipes de vente.

### 🛠️ Portée et hypothèses supplémentaires

Le tableau de bord étant destiné aux directeurs des ventes, la vue la plus importante pour eux est de voir leur propre équipe, plutôt qu'un tableau de bord exécutif avec des comparaisons d'équipes de niveau supérieur. Ils peuvent cependant souhaiter examiner d'autres équipes de vente plus en détail et il n'y a aucune exigence de sécurité au niveau des lignes (SNL) pour les empêcher d'accéder aux données d'autres équipes.

On suppose que le « trimestre actuel » est le quatrième trimestre 2017, qui est la dernière période enregistrée dans l'ensemble de données. Cependant, en réalité, ce tableau de bord serait continuellement mis à jour au fil du temps à mesure que de nouvelles données seraient ajoutées.

## 📈 Le tableau de bord

Le tableau de bord étant interactif, j'ai également veillé à le rendre convivial pour les publics qui n'utilisent pas Power BI au quotidien. Si les responsables commerciaux ne se sentent pas à l'aise avec le tableau de bord, ils n'en tireront aucun avantage. C'est pourquoi j'ai ajouté une page d'aide couvrant les fonctionnalités de base du tableau de bord. Cela permet aux responsables commerciaux de naviguer en toute confiance dans le tableau de bord, d'interpréter clairement les informations qu'ils voient et de répondre à leurs questions clés.

### 🏆 Performance du trimestre en cours

![ ](https://github.com/Arnaudl44/Projet_Tableau_de_Bord_CRM_Insights_pour_Managers/blob/main/images/Capture%20d%E2%80%99%C3%A9cran_1.png)

Il s'agit de la page principale du rapport, contenant les informations les plus importantes pour les responsables des ventes. Les utilisateurs sélectionnent leur nom dans le filtre du responsable des ventes, et toutes les pages du tableau de bord sont alors renseignées avec les informations de leur équipe.

Les indicateurs clés de performance sont clairement affichés en haut de la page, avec les chiffres du trimestre précédent. Le chiffre moyen de l'ensemble des équipes de vente pour chaque indicateur est également fourni afin d'apporter davatange de contexte. Cela permet au responsable des ventes de voir ses propres chiffres et de comprendre globalement comment il se positionne par rapport aux autres équipes et vers ses propres objectifs.

À partir de la carte des ventes totales, les utilisateurs peuvent cliquer sur la flèche pour accéder plus en détail à la répartition des ventes pour le trimestre en cours. Cela les aide à comprendre où ils ont connu du succès et même à consulter les données de vente détaillées si nécessaire.

![ ](https://github.com/Arnaudl44/Projet_Tableau_de_Bord_CRM_Insights_pour_Managers/blob/main/images/Capture%20d%E2%80%99%C3%A9cran_4.png)

À partir de la fiche de "potentiel de clôture", les managers peuvent également approfondir toutes les opportunités étiquetées comme engageantes pour leur équipe. Ils peuvent utiliser ces détails pour prioriser des actions telles que le suivi des offres à clôturer avant la fin du trimestre et le nettoyage du CRM, par exemple les opportunités qui sont ouvertes depuis trop longtemps et doivent être marquées comme perdues.

![ ](https://github.com/Arnaudl44/Projet_Tableau_de_Bord_CRM_Insights_pour_Managers/blob/main/images/Capture%20d%E2%80%99%C3%A9cran_5.png)

La page de performance du trimestre en cours approfondit ensuite les données, avec les indicateurs clés de performance répertoriés pour chaque agent commercial individuel et une mise en forme conditionnelle mettant en évidence en jaune pale les membres de l'équipe qui peuvent rencontrer des difficultés dans un domaine particulier. Cela permet au responsable des ventes d'identifier à la fois les domaines sur lesquels il peut se concentrer pour améliorer les performances et les personnes qui peuvent avoir besoin d'une assistance supplémentaire. La répartition au niveau du produit permet également d'identifier les domaines d'amélioration spécifiques pour l'équipe dans son ensemble et pour les individus.

### 🤝 Performances par équipe

Bien que ce ne soit pas l'objectif le plus important pour les directeurs des ventes, ils aimeraient également pouvoir voir comment leur équipe se comporte par rapport aux autres équipes de vente. La page Performances du trimestre en cours par équipe leur permet de le faire, en classant toutes les équipes de vente selon les indicateurs clés et en mettant en évidence l'équipe sélectionnée afin que les responsables puissent facilement voir où elles se situent.

![ ](https://github.com/Arnaudl44/Projet_Tableau_de_Bord_CRM_Insights_pour_Managers/blob/main/images/Capture%20d%E2%80%99%C3%A9cran_2.png)

### 📅 Performances au fil du temps

La dernière page du tableau de bord permet aux directeurs des ventes de visualiser les performances de leur équipe au cours des trimestres précédents afin d'identifier les tendances.

![ ](https://github.com/Arnaudl44/Projet_Tableau_de_Bord_CRM_Insights_pour_Managers/blob/main/images/Capture%20d%E2%80%99%C3%A9cran_3.png)
