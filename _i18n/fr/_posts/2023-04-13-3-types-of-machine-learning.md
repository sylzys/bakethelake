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

Many images are labeled ("cat", "dog") and passed to the ML model. With these images, the model learns how to distinguish both animals, improves (measured by the selected metrics) and become able to correctly classify them ("This image is a cat, I'm 92.18% sure")

Same goes with a chef, and her student. At the beginning, the student does not know anything. Hence, the chef has to teach him everything. Inputs could be the ingredients and their quantity, the process... the target, or output, is the cake. By practicing, under the supervision of the chef, the student improves (measured by the cake aspect and taste) and becomes able to realise the recipe.

<figure>
    <img src="assets/images/ML_supervised.jpg" alt="Under supervision, with known inputs and outputs, the student improves"/>
    <figcaption>Under supervision, with known inputs and outputs, the student improves.</figcaption>
</figure>

## Unsupervised Learning

Sometimes, the student is an external candidate. He has no chef to supervise and teach him. So he takes what's available as input: the recipes.

Let's imagine that the student finds many recipes, with no title nor picture. Inputs are available (ingredients, process), but he needs to group recipes by similarities. If he finds a recipe containing milk, caramel & vanilla and fridge, it's unlikely that the student will classify it with a recipe with chocolate, flour, butter, sugar and oven.

That's one of the scenarios of Unsupervised Learning: clustering.

Back to Machine Learning. A common case of unsupervised learning (and clustering) is marketing segmentation. For a marketplace, we have many inputs such as orders, average spending, socio-demographics data (age, family, job...). With all this, the ML model will, without assistance, uncover patterns or structure in the data without knowing the correct answers in advance, and find similarities between customers and "cluster" them.

Another example with our cats and dogs images, we will pass the images to the model, but no label. The computer will have to find a way to distinguish between each type (maybe with eyes shape, tail length, paws etc)


<figure>
    <img src="assets/images/ML_unsupervised.jpg" alt="Unsupervised learning does not provide output"/>
    <figcaption>Unlike supervised learning, we don't feed the expected results to the model.</figcaption>
</figure>

## Reinforcement Learning

Reinforcement learning is the one that needs the most autonomy. Our pastry chef has no recipes, no process, no picture of the expected cake. All he can use is trial and error. But how will he know if he's on the good way ?

He has to find a reward / penalty system, and use continuous improvement:
- bake a cake
- have the customers taste it
- get the feedbacks (positive: reward, negative: penalty)
- iterate based on the feedbacks
- repeat until the goal is met (a specific amount a cakes sold, for instance)

In Machine Learning, Reinforcement Learning is often used to "teach" autonomous cars to drive.
The car is rewarded for following traffic rules and safely navigating the roads, and is penalized for breaking traffic laws or causing accidents. Obviously, we want to maximize the reward (and minimize the penalty).

Through reinforcement learning, the car can continuously learn and improve its driving behavior and ultimately go successfully from point A to point B.

<p><a href="https://unsplash.com" target="blank_"><small>Image from Unsplash (Fabrizio Magoni, Todd Quackenbush)</small></a> & <a href="https://burst.shopify.com/" target="blank_"><small> Burst (Sarah Pflug)</small></a></p>
