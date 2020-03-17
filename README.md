# Guide-TP2-inf3135

## Introduction

Ce guide est personelle à ma compréhension du sujet, mais public pour aider les personnes qui ont besoins de s'assurer une bonne compréhension du sujet. De plus tous commentaires et questions son la bienvenue, Mais avant de me poser des questions, les issues du cours seront surement plus utile à vos besoins. Bonne Lecture !!!! :-)

## sommaire

- [Liste exhaustive des entrées sortie](#Liste-exhaustive-des-entrées-sortie)


# Liste exhaustive des entrées sortie

Avant de regarder cette liste il est preferable de lira la suite

Voici les cas a traiter que j'ai trouver je pense avoir fait le tour mais si il manque je ne vois pas les quelle.


| Cas | Entrés | Sorties (ce sont les erreurs possibles) |
|-----|--------|---------|
| Cas 01 si état n'existe pas| 150 01 5 | 08 14 150 ETAT |
|| 150 est la ligne, 01 le code du système et 5 la valeur de l'état | 08 Erreur de valeur innaceptable, 14 système etat de l'avion et 150 la ligne plus information additionel |
|| \<timestamp\> 01 \<etat\>| 08 \<sensor\> \<timestamp\> \[information additionnelle\]|
| Cas 02 si trois erreur consecutive| 124 02 A2 ERROR | |
|| 125 02 A2 ERROR ||
|| 126 02 A2 ERROR| 06 13 126 X3 |
|| | 06 pour erreur système, 13 pour sytème Angle incidant soit le 02, 126 la ligne, X3 est l'information supplémentaire|
|| \<timestamp\> 02 \<A1\|A2\|A3\> \<angle\|ERROR\>| 06 \<système\> \<timestamp\> \[information additionnelle\] |
|Cas 02 si ce n'est pas A1 ou A2 ou A3| 141 02 A4 10.5 | 08 13 141 AI | 
|Cas 02 si angle +ou- 360 |  120 02 A2 370.9 | 08 13 120 ANGLE |
|Cas 03 si valeur innaceptable | 121 03 D -1.700 | 08 11 121 D |
|Cas 03 si valeur on un trop grand ecart | 171 03 G 12.500 | |
| | 172 03 D 24.500| 06 11 172 MARGE |
|Cas 03 si valeur Erreur trois fois | apres toi répétition de erreur| 06 11 ligne X3 |
|Cas 04 si valeur innaceptable | 201 04 G 2.0 | 08 12 201 G | 
|Cas 04 si 3 erreur consecutive| apres 3 erreur | 06 12 ligne X3 |
|Cas 05 | 191 05 15 1 | 06 15 191 |
