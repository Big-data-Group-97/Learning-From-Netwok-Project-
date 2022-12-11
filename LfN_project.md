# Plan after porposal submission

## Identified problem types
1. unweighted, directed, changes in shortes path length, removal of node
  - logistic structures, cost is need to change transport flows
  - possible relaxing path checks only between `sources` and `consumers`
  - damage is amount of change in the shortest paths costs
2. Maximum flow problem, changes of flow, removal of node
  - infrastructure networks, such as gas, oil, electricity, traffic, more
  - need definition of producers and consumers
  - identify critical infrastructure elements for simple logistical networks
3. unweighted, directed, Motif count change on removal of node
  - applications in genetic and biological networks
  - need careful performance considerations
  - perhaps even consider changes from one mortif to another ?


## CItations sources 
good basic paper on node removal on simple networks 
  https://www.sciencedirect.com/science/article/pii/S037843710400439X
  https://journals.plos.org/plosone/article/file?id=10.1371/journal.pone.0059613&type=printable
too advanced
  https://www.sciencedirect.com/science/article/pii/S0378437115007037   
  https://www.sciencedirect.com/science/article/pii/S0378437119306740
  https://appliednetsci.springeropen.com/articles/10.1007/s41109-018-0089-9#Sec2
  https://doi.org/10.3390/en15030797

## step 4 - The book
 - read chap 8 of [the book](http://www.networksciencebook.com/chapter/8)
 - define a few basic problems we want to explore from this
 - code basic example of random attacks on simple graph and simple targeted attacks
 - 

# Problem definition
 - type of graph
   - weighted/unweighted
   - directed/undirected
   - edge propertioes/limits
   - node proeprties/limits
   - more
 - definitioon of damage
   - node removed
   - weight altered
   - linked edges removed
     - all/some
   - properties altered
 - metric of effect
   - number of edges removed
   - changes to shortes path pairs
     - length/weight/number of changes
   - isolation of communities
     - fragility of community connection
 - number of nodes removed

Idenitfy possibilituies for all these, consider varipus copmbinations and choose a few (3-6) specific types
Compare with colleagues and choose 2-4 for nect steps