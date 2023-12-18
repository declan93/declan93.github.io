---
layout: post
title:  Quick and easy gene set enrichment
categories: [CompBio]
excerpt: 
---

One thing that seems to always waste a huge amount of time is searching for whether a set of genes identified as significant from some model are enriched for a specific set of functions. Its relatively easy to write a list of genes to a file along with a set of p-values or some ranking metric and use a database over a web browser such as DAVID or PANTHER. This becomes burdensome when you have multiple gene sets from differing models. You can use an R package or API to try and automate this. For me a quick wrapper makes a lot of sense. I don't necessarily need a complicated statistical model - I don't care about the false negative rate if there is something there it will be analysed more carefully.

