---
layout: page
title: Non-diagonalizable digraphs
description: 
img: assets/img/cube.jpg
importance: 2
category: Spectral graph theory
giscus_comments: false 
---

## Background results

Let $$X = (V,E)$$ be an undirected graph. Since the adjacency matrix of $$X$$ is symmetric, it is *diagonalizable*, and its eigenvalues are real. If we replace $$X$$ with a digraph, then its adjacency matrix need not be diagonalizable. For instance, the digraph with adjacency matrix

$$ A =\begin{bmatrix} 0 & 1 & 0\\ 0 & 0 & 1\\ 0 & 0 & 0\end{bmatrix}$$

is not diagonalizable. If the adjacency matrix of a digraph is diagonalizable, then we say that the graph is diagonalizable.

In the 1980s, Peter J. Cameron [[1]](#1) asked whether whether all arc-transitive digraphs are diagonalizable. Godsil [[2]](#2) showed later that if $$A$$ is an integral matrix, then there is vertex-transitive digraph whose minimal polynomial is divisible by that of $$A$$. In 1985, Babai [[3]](#3)extended this result for arc-transitive digraphs, and therefore gave a negative answer to Cameron's question. In [[3]](#3), Babai additionally asked whether one can construct examples of *non-diagonalizable $$s$$-arc-transitive digraphs and vertex-primitive digraphs*

## Non-diagonalizable vertex-primitive digraphs
Recently, Li et al [[4]](#4) constructed an infinite family of non-diagonalizable $$s$$-arc-transitive digraphs, for $$s\geq 2$$, and an infinite family of non-diagonalizable vertex-primitive digraphs. Both constructions involve finding a Cayley digraph with the desired property, and then using the tensor product of digraphs. In fact, if either $$X$$ or $$Y$$ is non-diagonalizable digraphs, then the tensor product $$X \times Y$$ is non-diagonalizable.

Cayley digraphs are ''easier'' to deal with since their entire spectra can be obtained, in theory, from the regular representation of the underlying group. Vertex-primitive digraphs that are not Cayley digraphs are much harder to  handle since there is no obvious framework to study their eigenvalues. In [[4]](#4), Li et al. gave other examples of non-diagonalizable vertex-primitive digraphs that are non-Cayley. The smallest of these was a digraph arising from the action of $$PSL_2(17)$$ on the $$2$$-subsets of points in $$PG_1(17)$$.
It turns out that this example is one of the two smallest non-diagonalizable vertex-primitive digraphs with valency $$24$$.

**Theorem.** *The smallest non-diagonalizable vertex-primitive digraphs with least valency arise from $$PSL_2(17)$$ acting on the $$2$$-subsets of $$PG_1(17)$$.*

#### Association schemes

If $$G\leq Sym(\Omega)$$ is a transitive group, then the orbitals of $$G$$ form an association scheme, which is not always commutative, called the *orbital scheme* of $$G$$. This scheme is commutative if and only if the point-stabilizer $$G_\omega$$ is a *multiplicity-free subgroup*, that is, the character $$\operatorname{Ind}^G(\mathbf{1}_{G_\omega})$$, where $$\mathbf{1}_{G_\omega}$$ is the trivial character of $$G_\omega$$, is a sum of distinct irreducible characters of $$G$$.

Commutativity in association schemes gives a nice way to show diagonalizability. Indeed, if $$A_0,A_1,\ldots,A_d$$ are the adjacency matrices of digraphs in a commutative association scheme, then $$\{A_0,A_1,\ldots,A_d\}$$ is set of commuting normal matrices. Therefore, they are simultaneously diagonalizable. We can deduce from this fact that if $$G\leq Sym(\Omega)$$ is transitive, and the point-stabilizer $$G_\omega$$ is multiplicity free, then every digraph admitting $$G$$ as a subgroup of automorphism is diagonalizable.

Therefore, we may only consider the primitive groups whose point-stabilizers are not multiplicity free. The group $$PSL_2(17)$$ acting on $$2$$-subsets of $$PG_1(17)$$ has degree $$153$$. The primitive groups of degree up to $$153$$ whose point-stabilizers are multiplicity free are given below.

|---|---|---|---|
|Group | Stabilizer | Rank| id|
|$$PSL_2(11)$$ | $$D_{12}$$| 9 | PrimitiveGroup(55,1)|
|$$PSL_2(13)$$| $$D_{14}$$| 9| PrimitiveGroup(78,1)|
|$$PSL_2(13)$$| $$D_{12}$$| 12| PrimitiveGroup(91,1)|
|$$PSL_2(13)$$ | $$Alt(4)$$| 11 |PrimitiveGroup(91,3)|
|$$PSL_2(17)$$| $$D_{18}$$| 12 |PrimitiveGroup(136,1)|
|$$PSL_2(17)$$ | $$D_{16}$$| 15 |PrimitiveGroup(153,1)|

## References

<a id="1">[1]</a> 
P. Cameron (1983). 
Automorphism groups of graphs. 
*Selected topics in graph theory 2.*

<a id="2">[2]</a> 
C. Godsil (1982) 
Eigenvalues of graphs and digraphs. 
*Linear Algebra Appl.*, 46, 43–50

<a id="3">[3]</a> 
L. Babai  (1985)
 Arc transitive covering digraphs and their eigenvalues. 
*J. Graph Theory*, 9 (3), 363–370

<a id="4">[4]</a> 
Y. Li, B. Xia, S. Zhou, and W. Zhu (2024)
A solution to Babai’s problem on digraphs with non-diagonalizable adjacency matrix
*Combinatorica*, 44: 179–203