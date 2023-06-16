---
layout: page
title: research
permalink: /projects/
#description: Here is my research.
nav: true
#display_categories: [work, fun]
horizontal: false
math: true

---

<!-- pages/projects.md -->

My research areas lie in the intersection of combinatorics and algebra. In particular, I am interested in the [Erdős-Ko-Rado (EKR) theorem](https://en.wikipedia.org/wiki/Erd%C5%91s%E2%80%93Ko%E2%80%93Rado_theorem) for permutation groups and, sometimes, for other combinatorial structures. I also do research on some topics in the field of algebraic/spectral graph theory.

### Intersecting problems for permutation groups
Given a set of permutations F of a set Ω, we say that F is *intersecting* if any two permutations of F agree on an element of $\Omega$. That is,

 $$ \forall g,h \in F, \exists \omega\in \Omega \text{ such that } \omega ^g = \omega^h.$$

A transitive permutation group G≤Sym(Ω) is said to have the EKR property if any family of intersecting permutations of G has size no more than a stabilizer of a point. The long term objective of this project is to classify groups that have the EKR property.

Here are some materials on this topic:
1. Karen Meagher, Pablo Spiga, and Pham Huu Tiep. An Erdős-Ko--Rado theorem for finite 2-transitive groups. European Journal of Combinatorics, 55:100--118, 2016.
2. Chris Godsil and Karen Meagher. A new proof of the Erdős-Ko-Rado theorem for intersecting families of permutations. European Journal of Combinatorics, 30(2):404--414, 2009.
3. Chris Godsil and Karen Meagher. Erdős-Ko-Rado theorems: algebraic approaches
4. Hujdurović, A., Kutnar, K., Kuzma, B., Marušič, D., Miklavič, Š., and Orel, M. On intersection density of transitive groups of degree a product of two odd primes. Finite Fields and Their Applications 78 (2022): 101975.


### Spectral graph theory

I am also interested in questions regarding eigenvalues of graphs that are more or less ''symmetric''. Here, I will describe some of them.

#### Spectrum of normal Cayley graphs  
Consider the Cayley graph $$ Cay(Sym(n),T_n) $$, where $$T_n$$ is the set of all transpositions of $$Sym(n)$$. It is clear that the eigenvalue corresponding to a self-transpose partition of $$n$$ is equal to $$0.$$ Find the multiplicity of the eigenvalue $$0$$ of this graph.