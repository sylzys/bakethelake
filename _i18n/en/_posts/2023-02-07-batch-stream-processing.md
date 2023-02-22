---
layout: post
title:  "Batch & Stream processing "
author: sz
language: fr
categories: [ data engineering, flow ]
image: assets/images/batch_stream_processing.jpg
description: "An important Data Engineering step is about processing datas to further analyze them."
featured: true
hidden: true
---

<div class="disclaimer"><i>Disclaimer : this website offers a metaphorical approach to big data, data science and data engineering concepts. They are purposely simplified and some of them may be eluded or approximative.</i></div>

One of the most important aspects of data processing in Data Engineering is the Lambda architecture. This concept is based on 2 methods. The choice of one or the other will depend on the insights you need.

## Stream processing

Back to our bakery. Throughout the day, customers come into the store and buy our products.

From time to time, the boss drops by. He wants to have an (almost) "real time" overview of the store's performance.

To meet his need, and since the visits are unplanned, the employees write down each of their sales on a whiteboard. The data arrives in real time (after each sale) and the analysis is instant.

The analysis of the data and its visualization ("dataviz") is of course based on the data collected. It can be simply the number of sales, but also by which employee, which type of product, at which period or time of the day, which type of customer (socio-demographic data), which type of payment...

<figure>
    <img src="assets/images/stream_processing.jpg" alt="Les données peuvent être collectées en 'stream processing', en (quasi) temps-réel"/>
    <figcaption>Data can be processed on (near) real-time by using 'stream processing'.</figcaption>
</figure>

## Batch processing

While stream processing can provide a real-time overview, it does not easily give a clear, in-depth perspective on the data.

It is difficult to imagine a gigantic whiteboard on which all the transactions of the year would be recorded in detail.

So we store the data and analyze it in "chunk". A batch of a week, a month, a year of sales... We can make analysis on larger data and have a global vision, see the "big picture".

Of course, nothing prevents stream processing over long periods of time, assuming you have the necessary resources and adapt your workflow with the appropriate tools.


<figure>
    <img src="assets/images/batch_processing.jpg" alt="Le 'batch processing' permet une vision plus globale"/>
    <figcaption>'Batch processing' allows a broader view, using more data.</figcaption>
</figure>

## Stream or batch ?

It is often recommended to start with batch processing, which is considered as a solid base for a performing big data platform.

The process is simple, easy to set up and pretty low cost, allowing to get a global view on data, customers...

As the business grows, and if the need for real-time analysis arises, we can then add a stream pipeline to our big data platform.

<p><a href="https://unsplash.com" target="blank_"><small>Image from Unsplash (Petr Sevcovic)</small></a></p>
