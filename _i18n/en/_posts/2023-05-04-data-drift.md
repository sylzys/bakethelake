---
layout: post
title:  "Data Drift"
author: sz
language: en
categories: [ Data Science, Machine Learning, Performance ]
image: assets/images/data_drift.jpg
description: "Data Drift occurs when the initial performance of a model decrease."
featured: true
hidden: true
---

<div class="disclaimer"><i>Disclaimer : this website offers a metaphorical approach to big data, data science and data engineering concepts. They are purposely simplified and some of them may be eluded or approximative.</i></div>

Panic in the room. The model we trained and deployed a few months ago is not performing as well as it used to.
What happened ? Let's investigate one possible solution:

## Data Drift

Data Drift is a phenomenon that occurs when the initial performance of a model decreases. It can be due to a lot of reasons, but to illustrate that, let's go to our pastry shop first.

Our skilled chef is baking is famous cake. Secret recipe, he's been doing it for years. He knows exactly how much flour, sugar, chocolate, cream etc. he needs to make the perfect cake. The customers are happy, the sales (performance metrics) are good.

All is good, until one day, a few weeks later, customers begin to complain. "Chef, your cake is not as good as it used to be". Sales are decreasing, and the chef is worried. Our "model" performance is decreasing.

So what happened ? The chef is still using the same recipe, the same ingredients, the same process. The input (ingredients) is the same, but the output (cake) is not anymore. Well decided to investigate, the chef inspect everything. Turns out that the flour has begun to deteriorate. That's a form of data drift. The initial ingredients, qualified and used to output a great result, are not the same in the end. Even if the chef dont change anything in the recipe and the process, the final result is not as good.

<figure>
    <img src="assets/images/nlp.jpg" alt="Monitoring dashboard"/>
    <figcaption>A NLP model can easily suffer from Data Drift</figcaption>
</figure>

## Data Drift in Machine Learning

Knowing that, what could be an example of data drift in Machine Learning ? Imagine a factory, monitoring a lot of its machines, through IoT sensors. The factory managers rely heavily on predictive maintenance, which mean  they want to predict when a machine will break, to prevent it and avoid production loss.

At the beginning, the IoT sensors are performing well, and the data scientists team train a really good model, with high accuracy (performance metrics). All is good, until one day... A machine breaks, and the model did not predict it. The model performance decreased. Well.. turns out one of the sensor is not working properly anymore. Overall, the data is not the same as before, and the model can't achieve the same results.

Another concrete example would be a sentiment analysis model. We train our model based on a lot of English sentences, and it performs really well. But a language is not static, and new words, new expressions, new slang are created everyday. The model may not be able to predict the sentiment of a sentence containing a new word, or a new expression. Slowly, as the new words and slang are more and more used, our sentiment analysis performance will decrease.

Finally, a change in the data distribution can also lead to data drift. Imagine a model predicting insurance premiums. Over time, the overall population is getting older, or the average BMI is increasing. The model will not perform as well as it used to. In our shop, that could be a change in the customers' taste. The chef is still using the same recipe, but the customers are not wanting chocoate cake as much as they used to.

<figure>
    <img src="assets/images/monitoring.jpg" alt="Monitoring dashboard"/>
    <figcaption>Monitoring model performances can help prevent data drift</figcaption>
</figure>

## How to prevent Data Drift ?

Data drift is a real, insidious problem. It can be hard to detect, and even harder to prevent. But there are some ways to prevent it, or at least to mitigate its effects.

### Monitoring

First thing is to monitor the performance. If we don't know that our model is not performing as well as it used to, we can't do anything about it. Just as we can monitor our pastry shop sales and take actions when it starts to decrease, we need to monitor our model performance. That can be some daily logs sent to the team, an alert system, or even a whole dashboard.

### Periodic retraining

Additionally, we can retrain our model periodically. Getting back to our NLP example, once we observe the rise of some new words or expressions, we can retrain our model, every month for instance, to take them into account. Seems obvious, but be careful: old data are not (most of the time) replaced. We speak new words, but we still use English.

### Data augmentation

We can also use data augmentation techniques. If we know that the data distribution is changing, we can try to gather more data to take that into account and reflect the reality. If we know that the population is getting older, we can augment our data with more older people. That's a form of data augmentation, and it can be really useful to prevent concept drift.


<p><a href="https://unsplash.com" target="blank_"><small>Images from Unsplash (PhotoPum RanaRoja, Stephen Dawson, Glen Carrie)</small></a></p>