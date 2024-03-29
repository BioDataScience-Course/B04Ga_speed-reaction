Régression non linéaire : Vitesse de réaction chimique
================

<!--- do not edit readme.md ---->

## Avant-propos

Les consignes sont reprises dans ce document, ainsi que sous forme de
commentaires dans les différents fichiers. Elles sont susceptibles
d’évoluer. N’hésitez pas à vérifier le lien suivant afin de voir si des
modifications n’y ont pas été apportées :
<https://github.com/BioDataScience-Course/B04Ga_speed-reaction>

## Objectif

Ce projet est un projet *court*, *cadré*, *individuel* et qui doit être
**terminé pour la fin du module 4**. Il permet de nous démontrer que
vous avez acquis les compétences suivantes :

-   être capable d’utiliser la fonction nls()
-   être capable d’appliquer l’équation de Michaelis-Menten.

## Consignes

``` r
speed <- read("data/reaction.rds")
```

Des scientifiques ont déterminé la vitesse d’une réaction chimique en
fonction de la concentration en substrat. Le jeu de données
(`reaction.rds`) mis à votre disposition dans le dossier `data/`.

Avec ces données, le graphique ci-dessous, qui sera la base de votre
recherche, a été réalisé. Les scientifiques ont maintenant besoin de
vous pour déterminer les paramètres de la régression non linéaire.

``` r
chart(speed, speed ~ conc) +
  geom_point()
```

![](README_files/figure-gfm/unnamed-chunk-2-1.png)<!-- -->

Dans le cadre de cet exercice, vous devez analyser la situation mise à
votre disposition et consignez vos résultats sous la forme d’un carnet
de laboratoire au format Rmd. Ce document, nommé `speed_reaction.Rmd`,
se trouve dans le dossier `docs/`.

Afin de cadrer votre recherche, tentez de réaliser une régression non
linéaire qui suit l’équation proposée par Michaelis-Menten.

Une fois le travail réalisé, *assurez-vous que le document compile en un
rapport final HTML sans erreurs via le bouton `Knit`*, sinon, corrigez
les erreurs qui s’affichent avant votre soumission finale.
