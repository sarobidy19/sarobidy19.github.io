---
layout: page
title: research
permalink: /projects/
#description: Here is my research.
nav: true #to remove project
#display_categories: [work, fun]
horizontal: false
math: true

---

<!-- pages/projects.md -->

My research areas lie in the intersection of combinatorics and algebra. In particular, I am interested in the [Erdős-Ko-Rado (EKR) theorem](https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93Ko%E2%80%93Rado_theorem) for permutation groups and, sometimes, for other combinatorial structures. I also do research on some topics in the field of algebraic/spectral graph theory.

### Intersecting problems for permutation groups
Given a set of permutations $$\mathcal{F}$$ of a set Ω, we say that F is *intersecting* if any two permutations of F agree on an element of $$\Omega$$. That is,

 $$ \forall g,h \in \mathcal{F}, \exists \omega\in \Omega \text{ such that } \omega ^g = \omega^h.$$

It is easy to see that the subgroup $$ G_\omega = \{ g\in G : \omega^g = \omega \} $$ and any of its cosets are always intersecting. These are the so-called *canonical intersecting sets* of $$G$$. A transitive permutation group G≤Sym(Ω) is said to have the EKR property if any family of intersecting permutations of G has size no more than a stabilizer of a point. The long term objective of this project is to classify groups that have the EKR property. This is of course a very ambitious plan and seems to be out of reach with the tools at our disposal.

Let us now introduce a parameter that *measures* how far from a point stabilizer an intersecting is. Define the **intersection density** to be the rational number

$$ \rho(G) = \max \left\{ \frac{|\mathcal{F}|}{|G_\omega|}: \mathcal{F}\subset G \mbox{ is intersecting} \right\}.$$

Clearly $$\rho(G)\geq 1$$. In a [paper](https://www.sciencedirect.com/science/article/pii/S0097316520301825?casa_token=gJcp2-2pwxkAAAAA:K6S7EpTnCMg-Lfz_BZ64HSMhFtDbgA6n65MpXdUHwpPnfFiur1-HqN6SgwlDVAO8n2FbZgTPmOg) with Karen Meagher and Pablo Spiga, we showed that in fact

$$ 1 \leq \rho(G) \leq \frac{|\Omega|}{3}. $$ 

The upper bound is sharp since the group $$\operatorname{Alt}(4)$$ acting on cosets of $$C_2$$ has intersection density $$2$$ (due to the fact that the largest intersecting sets are cosets of the Klein group $$C_2\times C_2$$) and $$\frac{6}{3} = 2$$. In fact, there are only four transitive groups with intersection density attaining the upper bound. 

One typical method often used to prove an EKR type problem is to turn it into a graph theoretic problem. Define the **derangement graph** $$\Gamma_G$$ of a transitive group $$G\leq \operatorname{Sym}(\Omega)$$ to be the graph whose vertex set is $$G$$ and two group elements $$g$$ and $$h$$ are adjacent if and only if $$hg^{-1}$$ is a *derangement*, i.e., a fixed-point-free permutation of $$G$$. It follows that 

$$ \mathcal{F} \subset G \mbox{ is intersecting} \Leftrightarrow \mathcal{F} \mbox{ is a coclique of }\Gamma_G.$$

Using this fact, we deduce that

$$ \rho(G) = \frac{\alpha(\Gamma_G)}{|G_\omega|}. $$

On thing to note here is that all the transitive groups attaining the upper bound $$\frac{|\Omega|}{3}$$ have very special derangement graphs. In particular, their derangement graphs are complete tripartite. So far, we have not been able to find more groups attaining this upper bound.
A problem that I would like to be solved is the following.

**Problem.** 

Construct a family of transitive groups attaining whose intersecting density is 
$$\frac{|\Omega|}{3}$$
.
Is the intersection density $$\frac{|\Omega|}{3}$$ always an integer for such groups?

In fact, I counjecture that the following statement is true.

**Conjecture.**

Given a transitive group $$G\leq \operatorname{Sym}(\Omega)$$, we have that $$\rho(G) = \frac{|\Omega|}{3}$$ 
if and only if 
$$\Gamma_G$$ is a complete tripartite graph.

Here are some reading materials on this topic:
1. Karen Meagher, Pablo Spiga, and Pham Huu Tiep. An Erdős-Ko--Rado theorem for finite 2-transitive groups. European Journal of Combinatorics, 55:100--118, 2016.
2. Chris Godsil and Karen Meagher. A new proof of the Erdős-Ko-Rado theorem for intersecting families of permutations. European Journal of Combinatorics, 30(2):404--414, 2009.
3. Chris Godsil and Karen Meagher. Erdős-Ko-Rado theorems: algebraic approaches
4. Hujdurović, A., Kutnar, K., Kuzma, B., Marušič, D., Miklavič, Š., and Orel, M. On intersection density of transitive groups of degree a product of two odd primes. Finite Fields and Their Applications 78 (2022): 101975.


### Non-diagonalizable vertex-primitive arc-transitive digraphs

Let $$X = (V,E)$$ be a digraph with vertex set $$V$$ and arc set $$E$$. We say that $$X$$ is *diagonalizable* if its adjacency matrix is diagonalizable over the complex number. If $$E$$ is symmetric, then of course the adjacency matrix of $$X$$ is a symmetric matrix, hence diagonalizable. An example of a non-diagonalizable digraph is one whose adjacency matrix is a Jordan block. In general, one can come up with lots of examples but those arising from highly symmetric digraphs are more or less rare.

In 1982, P. J. Cameron asked whether all arc-transitive digraphs are diagonalizable. In this [paper](https://onlinelibrary.wiley.com/doi/pdf/10.1002/jgt.3190090308), L. Babai answered this question by contructing non-diagonalizable arc-transitive digraphs. Babai also asked to construct non-diagonalizable vertex-primitive digraphs. Recently, Y. Li, B. Xia, S. Zhou, and W. Zhu constructed such digraphs in this [paper](https://link.springer.com/article/10.1007/s00493-023-00068-x), and posed the following conjecture.

**Conjecture.**
*Every vertex-primitive arc-transitive digraph is diagonalizable.*

This conjecture has been verified for all such digraphs with at most 1000 vertices. As noted [here](https://ajc.maths.uq.edu.au/pdf/89/ajc_v89_p305.pdf), the analysis can be restricted to vertex-primitive arc-transitive digraphs with the property that if $$G$$ is a transitive subgroup of the automorphism group, then the permutation character of $$G$$ is not multiplicity free. 

