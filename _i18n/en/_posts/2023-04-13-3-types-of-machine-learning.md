---
layout: post
title:  "Supervised, unsupervised, reinforcement: 3 types of Machine Learning"
author: sz
language: en
categories: [ machine learning, theory ]
image: assets/images/ML_header.jpg
description: "3 main types of Machine Learning"
featured: true
hidden: true
---

<div class="disclaimer"><i>Disclaimer : this website offers a metaphorical approach to big data, data science and data engineering concepts. They are purposely simplified and some of them may be eluded or approximative.</i></div>

Machine learning is a type of artificial intelligence that allows computers to learn and improve from experience. There are three main types of Machine Learning (ML): supervised, unsupervised, and reinforcement learning. Each of these types has different characteristics and use cases, and understanding them is crucial for anyone interested in the field of machine learning.

## Supervised Learning

In supervised learning, the model is fed with many informations (inputs) and the expected result (target, or output). Let's take a simple example: classify images of cats and dogs.

De nombreuses images sont étiquetées ("chat", "chien") et transmises au modèle ML. Avec ces images, le modèle apprend à distinguer les deux animaux, s'améliore (ce qui mesuré par les métriques sélectionnées) et devient capable de les classer correctement ("Cette image est un chat, je suis sûr à 92,18 %")

Il en va de même avec un chef et son élève. Au début, l'élève ne sait rien. Par conséquent, le chef doit tout lui apprendre. Les entrées peuvent être les ingrédients et leur quantité, le processus… la cible, ou le résultat, est le gâteau.

En pratiquant, sous la supervision du chef, l'élève s'améliore (mesuré par l'aspect et le goût du gâteau) et devient capable de réaliser la recette.

<figure>
    <img src="assets/images/ML_supervised.jpg" alt="Sous supervision, avec des entrées et des sorties connues, l'étudiant s'améliore."/>
    <figcaption>Sous supervision, avec des entrées et des sorties connues, l'étudiant s'améliore..</figcaption>
</figure>

## Apprentissage non supervisé

Parfois, l'étudiant est un candidat libre. Il n'a pas de chef pour le superviser et lui apprendre. Il prend donc ce qui est disponible en entrée : les recettes.

Imaginons que l'élève trouve plusieurs recettes, sans titre ni image. Des entrées sont disponibles (ingrédients, processus), et qu'il ai besoin de regrouper les recettes par similarités. S'il trouve une recette contenant du lait, du caramel & de la vanille et un frigo, il est peu probable que l'élève la classe avec une recette avec du chocolat, de la farine, du beurre, du sucre et un four.

C'est l'un des scénarios possible de l'apprentissage non supervisé : le clustering.

Retour à l'apprentissage automatique. Un cas courant d'apprentissage non supervisé est la segmentation marketing. Pour une place de marché, nous avons de nombreuses entrées telles que les commandes, les dépenses moyennes, des données socio-démographiques (âge, famille, emploi...).

Avec tout cela, le modèle ML va, sans assistance, découvrir des modèles ou une structure dans les données sans connaître les bonnes réponses à l'avance, et trouver des similitudes entre les clients et les "regrouper".

Autre exemple avec nos images de chats et de chiens, nous allons passer les images au modèle, mais pas de label. L'ordinateur devra trouver un moyen de distinguer chaque type (peut-être avec la forme des yeux, la longueur de la queue, les pattes, etc.)

<figure>
    <img src="assets/images/ML_unsupervised.jpg" alt="L'apprentissage non supervisé ne fournit pas de sortie"/>
    <figcaption>Contrairement à l'apprentissage supervisé, nous ne transmettons pas les résultats attendus au modèle.</figcaption>
</figure>

## Apprentissage par renforcement

L'apprentissage par renforcement est celui qui nécessite le plus d'autonomie. Notre chef pâtissier n'a aucune recette, aucun procédé, aucune photo du gâteau attendu. Il ne peut que procéder avec des essais et des erreurs. Mais comment saura-t-il s'il est sur la bonne voie ?

Il doit trouver un système de récompense / pénalité et utiliser l'amélioration continue :

- faire cuire un gâteau
- le faire goûter aux clients
- obtenir les retours (positif : récompense, négatif : pénalité)
- itérer en fonction des retours
- répéter jusqu'à ce que l'objectif soit atteint (une quantité précise de gâteaux vendus, par exemple)

Dans l'apprentissage automatique, l'apprentissage par renforcement est souvent utilisé pour "apprendre" aux voitures autonomes à conduire.

La voiture est récompensée pour avoir respecté les règles de circulation et navigué en toute sécurité sur les routes, et est pénalisée pour avoir enfreint le code de la route ou causé des accidents. Évidemment, nous cherche à maximiser la récompense (et minimiser la pénalité).

Grâce à l'apprentissage par renforcement, la voiture peut continuellement apprendre et améliorer son comportement de conduite, pour se rendre avec succès du point A au point B.

<p><a href="https://unsplash.com" target="blank_"><small>Image from Unsplash (Fabrizio Magoni, Todd Quackenbush)</small></a> & <a href="https://burst.shopify.com/" target="blank_"><small> Burst (Sarah Pflug)</small></a></p>
