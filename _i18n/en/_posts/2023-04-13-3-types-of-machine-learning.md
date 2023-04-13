---
layout: post
title:  "Supervised, unsupervised, reinforcement: 3 types of Machine Learning"
author: sz
language: fr
categories: [ machine learning, theory ]
image: assets/images/ML_header.jpg
description: "3 main types of Machine Learning"
featured: true
hidden: false
---

<div class="disclaimer"><i>Disclaimer : this website offers a metaphorical approach to big data, data science and data engineering concepts. They are purposely simplified and some of them may be eluded or approximative.</i></div>

Machine learning is a type of artificial intelligence that allows computers to learn and improve from experience. Let's go over three types of Machine Learning (ML): supervised, unsupervised, and reinforcement learning.

## Supervised Learning

In supervised learning, the model is fed with many informations (inputs) and the expected result (target, or output). Let's take a simple example: classify images of cats and dogs.

Many images are labeled ("cat", "dog") and passed to the ML model. With these images, the model learns how to distinguish both animals, improves (measured by the selected metrics) and become able to correctly classify them.

Same goes with a chef, and her student. At the beginning, the student does not know anything. Hence, the chef has to teach him everything. Inputs could be the ingredients and their quantity, the process... the target, or output, is the cake. By practicing, under the supervision of the chef, the student improves (measured by the cake aspect and taste) and becomes able to realise the recipe.

<figure>
    <img src="assets/images/ML_supervised.jpg" alt="Under supervision, with known inputs and outputs, the student improves"/>
    <figcaption>Under supervision, with known inputs and outputs, the student improves.</figcaption>
</figure>

## Unsupervised Learning

Sometimes, the student is an external candidate. He has no chef to supervise and teach him. So he takes what's available as input: the recipes.

Let's imagine that the student finds many recipes, with no title nor picture. Inputs are available (ingredients, process), but he needs to group recipes by similarities. If he finds a recipe containing milk, caramel & vanilla and fridge, it's unlikely that the student will classify it with a recipe with chocolate, flour, butter, sugar and oven.

That's one of the scenarios of Unsupervised Learning: clustering.

Back to Machine Learning. A common case of unsupervised learning (and clustering) is marketing segmentation. For a marketplace, we have many inputs such as orders, average spending, socio-demographics data (age, family, job...). With all this, the ML model will, without assistance, find similarities between customers and "cluster" them.

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
The car is rewarded for following traffic rules and safely navigating the roads, and is penalized for breaking traffic laws or causing accidents.

Through reinforcement learning, the car can continuously learn and improve its driving behavior and ultimately go successfully from point A to point B.

<p><a href="https://unsplash.com" target="blank_"><small>Image from Unsplash (Fabrizio Magoni, Todd Quackenbush)</small></a> & <a href="https://burst.shopify.com/" target="blank_"><small> Burst (Sarah Pflug)</small></a></p>
