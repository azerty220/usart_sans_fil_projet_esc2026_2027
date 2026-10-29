# Projet de Transmission UART Sans Fil
Projet Système réalisé en troisième année spécialité Electronique et Systèmes de Communication à l'ENSEA : 

> Mise en place d'une communication sans fil USART avec un drône

## Cahier des charges

L'objectif de ce projet est de concevoir une chaîne de transmission/réception RF à partir de composants existants. Cet émetteur-récepteur est destiné à la communication avec un drone. Il y a donc une contrainte de place sur au moins une des versions du système.

Contraintes générales :

    Portée du système : 10m
    Durée du projet : 40h
    Budget : 250€

Paramètres de l'USART fourni : 

    Débit : 115 200 baud
    8 bits de données
    1 bit de parité (pair)
    1 bit de stop

## Choix de la fréquence porteuse et de la modulation

Nous avons choisi une porteuse à **868MHz**, ainsi que la modulation **ASK**,
<br>-Notre choix s'est porté sur la modulation ASK afin d'obtenir une portée nettement supérieure. De plus, nous avons pris en compte l'expérience d'un groupe ayant réalisé ce même projet en 2025 avec la modulation BPSK : leur choix avait entraîné de lourdes difficultés, notamment au niveau de la démodulation et de la récupération de la porteuse en phase. Cette dernière nécessitait en effet une PLL sans erreur de phase, alors qu'une PLL est initialement conçue pour minimiser les erreurs de fréquence.
<br>-En ce qui concerne la fréquence, nous avons choisi de réutiliser les composants des années précédentes afin de réduire les coûts. De plus, opter pour la bande des 2,4 GHz nous aurait exposé à de nombreuses interférences proches du Wi-Fi, qui se seraient avérées difficiles à filtrer.

## Description du système
![Schéma système](Images/Schéma_flipper.png)
## Choix des composants

