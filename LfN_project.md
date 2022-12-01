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


## step 2 - Basic Literature Review
Identify potential preexisting framework to take advantage of, bothb tehoretical and practical
identify valid datasets, especially small/artifical ones
Identify preexisting work on the problem definition and algorithms

Consider present literature
Consult materials that might cover the topic
- books
- papers
- online resources

The more there is, the less theoretical work we need to do
Documet all research and sources
Research individually, share resources

## step 3 - Further Discussion
When problem definition and literature review complete, meet to discuss future steps
- Consider time spent and remaining before midterm 
- Need to define target problem characteristics and block
- consider need of more theoretical research
- Consider talking with the professor
- potential start of work towards first algorithm designs and implementation

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