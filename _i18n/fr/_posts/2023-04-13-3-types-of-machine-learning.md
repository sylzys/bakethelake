---
layout: post
title:  "Apprentissage supervisé, non supervisé, par renforcement: 3 concepts du Machine Learning"
author: sz
language: fr
categories: [ machine learning, theorie ]
image: assets/images/ML_header.jpg
description: "3 apprentissages de Machine Learning"
featured: true
hidden: true
---

<div class="disclaimer"><i>Attention : ce site Web propose une approche métaphorique des concepts de big data, de Data Science et de Data Engineering. Ceux-ci sont volontairement simplifiés et certains d'entre eux peuvent être éludés ou approximatifs.</i></div>

Il existe trois principaux types d'apprentissage dans le Machine Learning : l'apprentissage supervisé, non supervisé et par renforcement. Chacun de ces types a des caractéristiques et des cas d'utilisation différents, et les comprendre est crucial pour quiconque s'intéresse au domaine de l'apprentissage automatique.

## Apprentissage supervisé

Pour l'apprentissage supervisé, le modèle est alimenté avec de nombreuses informations (entrées) et le résultat attendu (cible, ou sortie). Prenons un exemple simple : classer les images de chats et de chiens.

De nombreuses images sont étiquetées ("chat", "chien") et transmises au modèle ML. Avec ces images, le modèle apprend à distinguer les deux animaux, s'améliore (mesuré par les paramètres sélectionnés) et devient capable de les classer correctement ("Cette image est un chat, je suis sûr à 92,18 %")

Il en va de même avec un chef et son élève. Au début, l'élève ne sait rien. Par conséquent, le chef doit tout lui apprendre. Les intrants peuvent être les ingrédients et leur quantité, le processus... la cible, ou le résultat, est le gâteau. En pratiquant, sous la supervision du chef, l'élève s'améliore (mesuré par l'aspect et le goût du gâteau) et devient capable de réaliser la recette.

<figure>
    <img src="assets/images/ML_supervised.jpg" alt="Sous supervision, avec des entrées et des sorties connues, l'étudiant s'améliore"/>
    <figcaption>Sous supervision, avec des entrées et des sorties connues, l'étudiant s'améliore.</figcaption>
</figure>

## Apprentissage non supervisé

Parfois, l'étudiant est un candidat libre. Il n'a pas de chef pour le superviser et lui apprendre. Il prend donc ce qui est disponible en entrée : les recettes.

Imaginons que l'élève trouve plusieurs recettes, sans titre ni image. Des entrées sont disponibles (ingrédients, processus), et il a besoin de regrouper les recettes par similarités. S'il trouve une recette contenant du lait, du caramel, de la vanille et un frigo, il est peu probable que l'élève la classe avec une recette avec du chocolat, de la farine, du beurre, du sucre et un four.

C'est l'un des scénarios de l'apprentissage non supervisé : le clustering.

Retour à l'apprentissage automatique. Un cas courant d'apprentissage non supervisé est la segmentation marketing. Pour une place de marché, nous avons de nombreuses entrées telles que les commandes, les dépenses moyennes, les données socio-démographiques (âge, famille, emploi...). Avec tout cela, le modèle ML va, sans assistance, découvrir des modèles ou une structure dans les données sans connaître les bonnes réponses à l'avance, et trouver des similitudes entre les clients et les "regrouper".

Autre exemple avec nos images de chats et de chiens, nous allons passer les images au modèle, mais pas les labeliser. L'ordinateur devra trouver un moyen de distinguer chaque type (peut-être avec la forme des yeux, la longueur de la queue, les pattes, etc.)


<figure>
    <img src="assets/images/ML_unsupervised.jpg" alt="Contrairement à l'apprentissage supervisé, nous ne transmettons pas les résultats attendus au modèle"/>
    <figcaption>Contrairement à l'apprentissage supervisé, nous ne transmettons pas les résultats attendus au modèle.</figcaption>
</figure>

## Apprentissage par renforcement

L'apprentissage par renforcement est celui qui nécessite le plus d'autonomie. Notre chef pâtissier n'a aucune recette, aucun procédé, aucune photo du gâteau attendu. Tout ce qu'il peut utiliser, c'est un processus d'essais et d'erreurs. Mais comment saura-t-il s'il est sur la bonne voie ?

Il doit trouver un système de récompense / pénalité et utiliser l'amélioration continue :

- préparer un gâteau
- le faire goûter aux clients
- obtenir les retours (positif : récompense, négatif : pénalité)
- itérer en fonction des retours
- répéter jusqu'à ce que l'objectif soit atteint (une quantité précise de gâteaux vendus, par exemple)

Dans l'apprentissage automatique, l'apprentissage par renforcement est souvent utilisé pour "apprendre" aux voitures autonomes à conduire.

La voiture est récompensée pour avoir respecté les règles de circulation et navigué en toute sécurité sur les routes, et est pénalisée pour avoir enfreint le code de la route ou causé des accidents. Évidemment, l'objectif est de maximiser la récompense (et minimiser la pénalité).

Grâce à l'apprentissage par renforcement, la voiture peut continuellement apprendre et améliorer son comportement de conduite, pour se rendre avec succès du point A au point B.

<p><a href="https://unsplash.com" target="blank_"><small>Image Unsplash (Fabrizio Magoni, Todd Quackenbush)</small></a> & <a href="https://burst.shopify.com/" target="blank_"><small> Burst (Sarah Pflug)</small></a></p>
