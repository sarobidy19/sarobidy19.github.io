---
layout: post
title: Erdős-Ko-Rado theorem for doubly transitive groups
date: 2032-01-30 11:12:00-0400
description:
tags: EKR theorem
categories: math
---

Let $$G\leq \operatorname{Sym}(\Omega)$$ be a transitive group. A set $$\mathcal{F} \subset G$$ is *intersecting* if for any $$g,h\in G$$, there exists $$\omega \in \Omega$$ such that $$\omega^g = \omega^h$$. The study of the largest intersecting sets of permutations in a permutation group goes back to the late 70s. 

One of the most important results in this area is due to Meagher, Spiga and Tiep in their paper titled [An Erdős–Ko–Rado theorem for finite 2-transitive groups](https://instrepo-prod.cc.uregina.ca/bitstream/handle/10294/8288/WeakerConjecture2015_7_17B.pdf?sequence=1&isAllowed=y).
Recall that a transitive group $$G\leq \operatorname{Sym}(\Omega)$$ is of *$$2$$-transitive* if it is transitive on the set $$\Omega^{(2)} = \{ (x,y) \in \Omega\times\Omega \mid x\neq y\}$$.

> **Theorem (Meagher, Spiga, Tiep)** *If $$G\leq \operatorname{Sym}(\Omega)$$ is $$2$$-transitive, then any intersecting set of $$G$$ has size at most $$ \frac{\mid G\mid }{\mid \Omega\mid }$$.*

The authors gave an elegant proof using a consequence of the classification of $$2$$-transitive groups, and various upper bounds on the independence number. 
Here, I would like to talk about the proof of this theorem.

The proof relies on the so-called *derangement graph* $$\Gamma_G$$ of $$G$$, which is the graph whose vertex set is $$G$$, and two group elements $$g$$ and $$h$$ are adjacent if they are not intersecting. The derangement graph of $$G$$ encodes the intersecting sets of $$G$$, which just correspond to cocliques (or independent sets in $$\Gamma_G$$). Hence, proving this theorem is the same as proving that $$\alpha(\Gamma_G) = \frac{\mid G \mid}{\mid \Omega \mid}$$, for any $$2$$-transitive group $$G$$.

To prove this theorem, the authors first reduce the problem to the study of transitive subgroups via the so-called **No-Homomorphism Lemma**, which we state as follows.
  > **Lemma (No-Homomorphism, Albertson and Collins 1997)** *Let $$X$$ be a vertex-transitive graph, and let $$Y$$ be a graph*. If $$Y \to X$$ is a graph homomorphism, then 
  \begin{equation}
      \frac{\mid\alpha(X)\mid}{\mid V(X) \mid} \leq \frac{\mid\alpha(Y)\mid}{\mid V(Y)\mid}.
  \end{equation}

It is immediate from this lemma that if $$H\leq G$$ is a transitive subgroup such that $$\alpha(\Gamma_H) = \frac{\mid H \mid }{\mid \Omega \mid}$$, then $$\alpha(\Gamma_G) = \frac{\mid G \mid}{\mid \Omega \mid}$$. Consequently, it is enough to prove the result for minimal $$2$$-transitive groups.

From here, the authors use a result of Burnside which asserts that a $$2$$-transitive group has a unique *minimal normal subgroup*, which is either an **elementary abelian group** or an **almost simple group**. Since normal subgroups in a $$2$$-transitive permutation group are transitive, these two types of subgroups are our candidates to prove the main result.


Let $$G\leq \operatorname{Sym}(\Omega)$$ be a $$2$$-transitive group and  $$S$$ be a minimal normal subgroup of $$G$$.
### Affine types 
Assume that $$S$$ is an elementary abelian group of order $$q^k$$, for some prime power $$q$$ and $$k\geq 1$$. In this case, $$S$$ acts regularly. Consequently, the derangement graph of $$S$$ is a complete graph, so $$\alpha(\Gamma_S) = 1  =\frac{\mid S \mid}{\mid \Omega \mid}$$. 



### Almost simple types

Assume that $$S$$ is an almost simple group. By definition, we have $$S \leq G\leq \operatorname{Aut}(S)$$, where $$S$$ is a non-abelian simple group. Due to the classification of finite simple groups,  the group $$S$$ is one of groups in the table below.

|Line     | $$S$$   || Degree|
|---------|:-------:|---|-------:|
1         | $$\operatorname{Alt(n)}$$    |    |  $$n$$      |
2         | $$\operatorname{PSL}_k(q)$$    | |   $$\frac{q^k-1}{q-1}$$      |
3         | $$Sp_{2n}(2)$$ |      | $$2^{n−1}(2n \pm 1)$$ | 
4         | $$\operatorname{PSU}_3(q)$$ |   | $$q^3+1$$ |
5         | $$\operatorname{Sz}(q)$$    |   |     $$q^2+1$$      |
6         | $$\operatorname{Ree}(q)$$   |   |        $$q^3+1$$            |
7         | $$\operatorname{M}_n$$      |   |    $$n\in \{ 11,12,22,23,24 \}$$|
8         | $$\operatorname{M}_{11}$$   |   | $$12$$|
9         | $$\operatorname{PSL}_2(11)$$|   |  $$11$$|
10        | $$\operatorname{Alt}(7)$$   |   | $$15$$ |
11        | $$\operatorname{PSL}_2(8)$$ |   | $$28$$ |
12        | $$\operatorname{HS}$$       |   |  $$176$$|
14        | $$\operatorname{Co}_3$$      |   | $$276$$ |


For each of these 14 groups, either the Hoffman bound on the corresponding derangement graph yields the order of a point stabilizer or there exists a weighted adjacency matrix for which the weighted Hoffman bound yields the order of the point stabilizer.

 <!-- The $$2$$-transitive groups are an important classes of transitive groups which. -->