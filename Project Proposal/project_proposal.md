---
title: Project proposal - Identifying critical components in a network
author: 
 - Spina Lorenzo
 - Giustini Piermarco
 - Trapanotto Martino
date: November 6, 2022
---

# Identifying critical components in a network
## Motivation
We want to investigate how we can identify *critical* nodes and edges in a graph. 
This means finding elements of the graph that, if removed or altered in their properties, change some relevant characteristic of the graph.

The general concept can be interpreted in practice in multiple ways: a small group of electrical links that keep the grid connected, important logistical nodes that if blocked or disturbed greatly impact the flow of goods, species that if displaced or removed have wide-ranging ecological impact.

Such a wide theoretical construct lends itself to be applied to many datasets.

## Methods

A thorough and complete theoretical and practical analysis of the problem is out of the scope of our project. 

We'll focus on finding simple, yet reasonable approaches through the topics covered in class, a partial review of the current literature and simple implementations of identified methods, to compare on relatively small datasets.

Interpretability of results will have to be kept in mind, so a choice of datasets and approaches where our intuition applies will have to be followed.

Performance will not be a key objective of the project, but only kept as a data point in the conclusion. We'll focus on finding exact algorithms and approaches, optimizations and approximations are outisde the scope.

## Intended Experiments

The first phase will be a theoretical and conceptual analysis of the problem and some possible and real solutions. 

From there, a series of basic methods will be implemented, using current graph libraries as a backbone, and will be executed on one or more datasets. The results will be interpreted and analyzed, trying to compare our intuitions with the results of the algorithms, and their results with one another. If existing methods are available, these will be compared as well.

Some examples of possible metrics include: finding very small sets of nodes that if removed isolate large subgraphs ornodes that if removed alter and raise the length for many shortest path solutions. 

As a machine we'll use our own personal laptops and machines, as wide networks and performance are not the main concern of the project we expect to not run into huge performance issues. The most powerful has a Ryzen 5 5600 6 Code 12 Thread CPU and 16GB of RAM and a Nvidia GTX 1070 GPU with 8GB of VRAM.

