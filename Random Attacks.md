\newcommand{\braket}[1]{ \langle #1 \rangle}

# Random attacks

Percolation theory is the basis of our analysis.
Here we'll cover some basic parameters and formulas used in it, in a model for infinite, repeating lattices.

> The exponents $\gamma_p$, $\beta_p$, and $\nu$ are called critical exponents, as they characterize the system’s behavior near the critical point pc. Percolation theory predicts that these exponents are universal, meaning that they are independent of the nature of the lattice or the precise value of pc. Therefore, whether we place the pebbles on a triangular or a hexagonal lattice, the behavior of $\braket{s}$, $P_{\infty}$, and $\xi$ is characterized by the same $\gamma_p$, $\beta_p$, and $\nu$ 
> [...] the critical exponents do not depend on the lattice type, but only on the lattice dimension.  


Percolation theory allows us to work backwards from a fully constructed network into a fragmented one, studying how random node/link failures can be modelled as p<1 and how these values impact the wider network connectedness.

The parameters can be studied for random and other types of networks, allowing us to apply percolation theory beyond lattices.


> Random networks under random node failures share the same scaling exponents as infinite-dimensional percolation. Hence, the critical exponents for a random network are $\gamma_p$ = 1, $\beta_p$ = 1 and $\nu$ = 1/2, corresponding to the d > 6 percolation exponents encountered earlier

> for a scale-free network the exponent $\beta_p$ depends on the degree exponent $\gamma$, see advanced section 8.A for details

We can use the Molly-Reed Criterion to compute the existence of a Major Connected Component, and from this the Percolation Threshold for arbitrary degree distributions, including Random Networks and our Scale Free real networks

Thus, when $\frac{\braket{k^2}}{\braket{k}}>2$, for any $p_k$ degree distribution we have a giant component.

From this we derive the Percolation Threshold, in the form of $f_c = 1-p_c$ Breakdown Threshold

In general, we have $f_c = 1-\frac{1}{\frac{\braket{k^2}}{\braket{k}}-1}$

Random networks usually follow a Poisson distribution, we have $f_c = 1-\frac{1}{\braket{k}}$

Wikipedia gives a value for tree-like networks $p_{c}={\frac {\langle k\rangle }{\langle k^{2}\rangle -\langle k\rangle }}$

And for Scale Free Models, thus using the Power Law distribution, we have a more complex function, depending also on $\gamma$

$f_c = \begin{cases}
   1-\frac{1}{\frac{\gamma-2}{3-\gamma}k_{min}^{\gamma-2}k_{max}^{3-\gamma}-1} &\text{if } 2 < \gamma < 3 \\
   1-\frac{1}{\frac{\gamma-2}{\gamma-3}k_{min}-1} &\text{if } \gamma > 3
\end{cases}$

These values are extremely high for high $\braket{k^2}$ which we expected as scale free networks are quite resilient to random failures due to hubs being major connection points

## Names 

`power law` - distribution of type $p(x) = a*c^{-x}$

`scale-free networks` - 'real' networks, linked to a Power law distribution for node degree instead of a Poisson of a random network 

`percolation cluster` - huge single cluster that appears after $p_c\le p$

## Parameters

**NB**: $\gamma \ne \gamma_p$

 - p - probability for link existence
 - $\gamma$ - parameter describing the distribution of node degrees in scale-free/real networks
 - $p_c$ - critical probability from p for percolation cluster
 - d - Average Cluster Size: diverges  
 - $P_\infty$ - Order Parameter: probability that single node connects to percolation cluster
 - $\xi$ - Correlation Length: avg distance between members of same cluster
 - $P_{\infty}(f)/P_{\infty}(0)$ Ratio comparing Oder parameter of the original network and after removal of nodes with probability $f$
 - $\braket{k}$ average node degree and its moments

## Formulas

$d \thicksim \lvert p-pc \lvert ^{-\gamma_p}$

 $p_{\infty}\thicksim(p-pc)^{\beta_p}$

 $\xi\thicksim \lvert p-pc \lvert ^{-\nu}$

### Tasks 

1. Random network model
   - generate random network
   - compute analytically percolation parameters
   - compute node degree distribution
   - check if fits expected Poisson distribution
   - plot parameters d, $p_{\infty}$, $\xi$, $P_{\infty}(f)/P_{\infty}(0)$ as network erosion grows, both with analytical model and direct measurement
2. Scale-Free model
   - pick scale free model, possibly from real world dataset
   - compute node degree distribution
   - check if fits expected Power Law distribution
   - compute analytically percolation parameters
   - plot parameters d, $p_{\infty}$, $\xi$, $P_{\infty}(f)/P_{\infty}(0)$ as network erosion grows, both with analytical model and direct measurement