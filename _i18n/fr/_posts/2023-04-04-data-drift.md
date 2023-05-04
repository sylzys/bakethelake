---
layout: post
title:  "Data Drift"
author: sz
language: en
categories: [ Data Science, Machine Learning, Performance ]
image: assets/images/data_drift.jpg
description: "Data Drift occrus when the initial performance of a model decrease."
featured: true
hidden: true
---

<div class="disclaimer"><i>Disclaimer : this website offers a metaphorical approach to big data, data science and data engineering concepts. They are purposely simplified and some of them may be eluded or approximative.</i></div>

C'est la panique. Le modèle que nous avons entraîné et déployé il y a quelques mois ne fonctionne plus aussi bien qu'avant.
Que s'est-il passé? Voyons une solution possible:

## Data Drift (Dérive de données)

La dérive de données est un phénomène qui se produit lorsque les performances initiales d'un modèle diminuent. Cela peut être dû à beaucoup de choses. Mais pour l'illustrer, allons dans notre pâtisserie.

Notre chef, très doué, prépare son célèbre gâteau. Recette secrète. Il le fait depuis des années. Il sait exactement combien de farine, de sucre, de chocolat, de crème, etc. il faut pour faire ce gâteau parfait. Les clients sont heureux, les ventes (mesures de performance) sont bonnes.

Tout va bien, jusqu'au jour où, quelques semaines plus tard, les clients commencent à se plaindre. "Chef, votre gâteau n'est plus aussi bon qu'avant". Les ventes diminuent, et le chef est inquiet. Les performances de notre "modèle" se dégradent.

Alors, que s'est-il passé? Le chef utilise pourtant toujours la même recette, les mêmes ingrédients, le même processus. L'entrée (les ingrédients) est la même, mais la sortie (le gâteau) ne l'est plus. Bien décidé à enquêter, le chef inspecte tout.

Il s'avère que la farine a commencé à se détériorer. C'est une forme de dérive de données. Les ingrédients initiaux, qualifiés et utilisés pour produire un excellent gateau, ne sont plus les mêmes, finalement. Même si le chef ne change rien dans la recette et le processus, le résultat n'est plus aussi bon.

<figure>
    <img src="assets/images/nlp.jpg" alt="Monitoring dashboard"/>
    <figcaption>Un modèle de Traitement de Langage Naturel peut facilement subir la dérive des données</figcaption>
</figure>

## Dérive de données en Machine Learning

Sachant cela, quelle pourrait être un exemple de Data Drift en apprentissage automatique ? Prenons une usine qui surveille ses machines de près, via des capteurs IoT. Les responsables de l'usine s'appuient fortement sur la maintenance prédictive: ils veulent prédire quand une machine va tomber en panne, pour empêcher le problème en amont et éviter tout arrêt de production.

Les capteurs IoT fonctionnent bien, et l'équipe de scientifiques de données entraîne un modèle vraiment bon, avec une grande précision (mesures de performance). Tout va bien, jusqu'au jour où... une machine tombe en panne, et le modèle ne l'a pas prédit. Les performances du modèle ont diminué. Eh bien... il s'avère qu'un des capteurs ne fonctionne plus correctement. Dans l'ensemble, les données ne sont plus les mêmes qu'auparavant, et le modèle ne peut plus atteindre les mêmes résultats.

Un autre exemple concret serait un modèle d'analyse de sentiment. Nous entraînons notre modèle sur de nombreuses phrases en anglais, et il fonctionne vraiment bien. Mais une langue n'est pas statique, et de nouveaux mots, expressions et argot sont créés tous les jours. Le modèle peut ne pas être en mesure de prédire le sentiment d'une phrase contenant un nouveau mot ou une nouvelle expression. Lentement, à mesure que les nouveaux mots et l'argot sont de plus présents dans le langage quotidien, la performance de notre analyse de sentiments va baisser.

Enfin, un changement dans la distribution des données peut conduire à du Data Drift. Prenons l'exemple d'un modèle prédisant la prime d'une assurance à facturer. Au fil du temps, la population globale vieillit, ou l'IMC moyen augmente. Le modèle ne fonctionnera plus aussi bien qu'avant. Dans notre pâtisserie, cela pourrait être un changement dans le goût des clients. Le chef utilise toujours la même recette, mais les clients ne veulent plus autant de gâteau au chocolat qu'avant.

<figure>
    <img src="assets/images/monitoring.jpg" alt="Monitoring dashboard"/>
    <figcaption>Surveiller la performance des modèles peut aider a identifier le data drift</figcaption>
</figure>

## Comment prévenir la dérive des données ?

La dérive des données est un problème réel et insidieux. Il peut être difficile à détecter et encore plus difficile à prévenir. Mais il existe quelques moyens de la prévenir, ou du moins d'atténuer ses effets.

### Surveillance

La première chose à faire est de surveiller les performances. Si nous ne savons pas que notre modèle ne fonctionne plus aussi bien qu'avant, nous ne pouvons rien faire à ce sujet. Tout comme nous pouvons surveiller les ventes de notre pâtisserie et prendre des mesures lorsque cela commence à diminuer, nous devons surveiller les performances de notre modèle. Cela peut être des journaux quotidiens envoyés à l'équipe, un système d'alerte, ou même un tableau de bord complet.

### Ré-entraînement régulier

Nous pouvons ré-entraîner notre modèle périodiquement. Si l'on reprend l'exemple de l'analyse de sentiment, une fois que nous observons l'apparition de nouveaux mots ou expressions, nous pouvons ré-entraîner le modèle, tous les mois par exemple, pour les prendre en compte. Cela semble évident, mais attention : les anciennes données ne sont pas (la plupart du temps) remplacées. Nous utilisons de nouveaux mots, certes, mais nous parlons toujours français.

### Augmentation de données

Une autre technique de prévention est l'augmentation de données. Si nous savons que la distribution des données change, nous pouvons essayer de collecter plus de données pour en tenir compte et refléter la réalité, en obtenant plus plus de données concernant les personnes âgées, par exemple.

<p><a href="https://unsplash.com" target="blank_"><small>Images from Unsplash (PhotoPum RanaRoja, Stephen Dawson, Glen Carrie)</small></a></p>