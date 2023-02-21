---
layout: post
title:  "Batch & Stream processing "
author: sz
language: fr
categories: [ data engineering, flow ]
image: assets/images/batch_stream_processing.jpg
description: "Une phase importante du Data Engineering concerne le processing des données pour analyse"
featured: true
hidden: true
---

<div class="disclaimer"><i>Attention : ce site Web propose une approche métaphorique des concepts de big data, de Data Science et de Data Engineering. Ceux-ci sont volontairement simplifiés et certains d'entre eux peuvent être éludés ou approximatifs.</i></div>

Un des piliers du traitement de données en Data Engineering est l'architecture Lambda. Ce concept s'appuie sur 2 méthodes. Le choix de l'une ou l'autre de ces méthodes dépendra de votre besoin d'insights.

## Stream processing

Retournons dans notre boulangerie. Tout au long de la journée, des clients se rendent dans la boutique et achètent nos produits.

De temps à autres, le patron passe à l'improviste. Il veut absolument avoir un aperçu en (quasi) "temps réel" des chiffres de la boutique.

Pour répondre à ce besoin, et les venues étant non planifiées, les employés notent chacunes de leurs ventes sur un tableau blanc. Les données arrivent en temps réel (après chaque vente) et l'analyse est immédiate.

L'analyse des données et sa visualisation ("dataviz") est bien sûr fonction des données collectées. Cela peut-être simplement le nombre de ventes, mais aussi par quel employé, quel type de produit, à quelle période ou heure de la journée, quel type de clientèle (données socio-démographiques), quel type de paiement...

<figure>
    <img src="assets/images/stream_processing.jpg" alt="Les données peuvent être collectées en 'stream processing', en (quasi) temps-réel"/>
    <figcaption>Les données peuvent être collectées par 'stream processing', en (quasi) temps-réel.</figcaption>
</figure>

## Batch processing

Si le stream processing permet un aperçu temps réel, il ne permet pas de prendre du recul sur la data.

Il est difficile d'envisager un gigantesque tableau blanc, sur lequel on noterait toutes les transactions de l'année dans le détail.

Alors on stocke les données et on les analyse par "chunk". Un lot d'une semaine, d'un mois, d'un an de ventes... On peut faire des analyses sur des données plus larges et avoir une vision globale.

Bien sûr, rien n'empêche dans l'absolu de faire du stream processing sur de longues périodes, sous réserve de disposer des ressources nécessaires et d'adapter son workflow avec les outils adaptés.


<figure>
    <img src="assets/images/batch_processing.jpg" alt="Le 'batch processing' permet une vision plus globale"/>
    <figcaption>Le 'batch processing' permet une vision plus globale, sur plus de données.</figcaption>
</figure>

## Stream ou batch ?

Il est souvent recommandé de commencer par le batch processing, considéré comme une base solide d'une plateforme big data performante.

Le procédé est simple, facile à mettre en place et à coût relativement bas, permettant d'obtenir une vision globale sur les données, les clients...

A mesure de l'activité, et si le besoin d'analyse en temps réel se fait sentir, on peut alors ajouter une pipeline "stream" à notre plateforme big data.

<p><a href="https://unsplash.com" target="blank_"><small>Top image from Unsplash (Petr Sevcovic)</small></a></p>
