---
title: Midterm Report - Identifying critical components in a network
author: 
 - Spina Lorenzo
 - Giustini Piermarco
 - Trapanotto Martino
date: December 10, 2022
---

# Identifying critical components in a network
## Problem definition
After receiving approval for the topic of the project, we focused on defining the specific versions of the problem we wanted to consider.

We thought that specific problem types, based on the topics and ideas we saw in class, would be the most helpful and interesting to explore, so we identified these three problems:

 1. Critical nodes in a _sources_ and _consumers_ directed network, with Shortest-Path as a metric
 2. Maximum flow model, in a directed graph between _sources_ and _consumers_
 3. Motif number in an undirected graph

After the problem were clearly defined, we moved to a partial review of the existing literature on these topics, which had come unexpected results.

## Literature review

We searched for papers and materials linked to the topics of node removal and its impacts on network performance, specifically discussing our models and problems.

We wanted to find some theoretical groundwork on which to plant ourselves on to ensure that our next moves were based in good computer science theory and network science, and not our unclear assumptions.

The search had unsatisfying results: the broader topic clearly is of major concern considering the huge amount of papers and materials we found, but most of these were highly specialized, discussing vastly more advanced and complex topics and models than our ideas. Existing also as parts of the larger body of works that cover these topics, many cross-references and implicit definitions made them hard to read and fully digest.

Nonetheless, some useful insights and ideas could be drawn out of these papers, and they assured us that our ideas and research are not a step in uncharted waters, but a first step inside a large body of existing research. They also provided inspirations and ideas for our later steps.

We then focused our research on more basic works, finding some papers that resembled our models and problems from the '00s, but here again a difference in model complexity and lack of fundamental theory behind the concept created a barrier to our deeper understanding.

Finally, we focused on looking for books on the subject, and a very inserting find was _Network Science_ by _Albert-László_ _Barabási_, which contains an entire chapter on network robustness and results from attacks, building the theoretical framework we were looking for in through the lenses of Percolation Theory. This meant a change in the specifics of our problem, as we decided to change tracks to follow the lead of some of the books' ideas instead of blindly keep to our own.

## Dataset identification

While we searched for papers and materials, we also searched for datasets resembling our models. While we found some, with our recent change in direction these are not any more of major interest. Instead, we'll focus on generated graphs, switching to real world datasets only when we'll have a reasonable algorithm to test.

## Next steps

We've decided therefore to change approach, from our preferred models to a more structured approach, using this book and further resources as references and guides.

For now, we'll focus on digesting the contents of the book and converting these understanding in a framework in which to understand network attacks and vulnerabilities, including connections to Percolation Theory. To achieve this, we'll also build some of the problems and experiments described in the book itself. 

Beyond that, we'll focus on developing more advanced methods, attacks and models, and try to analyze them though the framework we developed, using both random networks, manually created ones and real datasets. We'll try to consider both random attacks and more targeted attacks, identifying for both some metrics to identity network robustness and ranking node criticality

