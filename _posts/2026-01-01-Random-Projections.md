---
layout: post
title: Random Projections
subtitle:
comments: false
---

<!-- MathJAx Import -->

$$\newcommand{\abs}[1]{\left\lvert#1\right\rvert}$$
$$\newcommand{\norm}[1]{\left\lVert#1\right\rVert}$$
$$\newcommand{\inner}[1]{\left\langle#1\right\rangle}$$
$$\DeclareMathOperator*{\argmin}{arg\,min}$$
$$\DeclareMathOperator*{\argmax}{arg\,max}$$
$$\DeclareMathOperator*{\E}{\mathbb{E}}$$
$$\DeclareMathOperator*{\V}{\mathbb{V}}$$

<!-- MathJAx End -->
<p style="margin-bottom:-2cm;"></p>

<p class="dropcap">T</p>his post introduces random projections as a tool for dimensionality reduction
in high-dimensional spaces. The emphasis is geometric: how random linear maps
approximately preserve distances, inner products, and subspace structure.
Probabilistic limit theory is used only implicitly; detailed asymptotic tools
are treated separately.

---

## Motivation: Geometry in High Dimensions

In high dimensions, many datasets exhibit redundancy: although observations live
in $\mathbb{R}^N$ with $N$ large, their intrinsic dimension is often much smaller.
Random projections exploit this by embedding high-dimensional data into a lower-
dimensional space while approximately preserving Euclidean geometry.

The central question is:

{: .box-warning}
How small can the target dimension be while preserving pairwise distances?

---

## Random Linear Maps

Let $R \in \mathbb{R}^{n\times N}$ be a random matrix and define the linear map
$$
f(x) = \frac{1}{\sqrt{n}} R x.
$$

Common choices for $R$ include:
- i.i.d. Gaussian entries $R_{ij}\sim \mathcal N(0,1)$,
- i.i.d. Rademacher entries $R_{ij}\in\{\pm1\}$ with equal probability,
- sparse or structured random matrices.

The normalization ensures that $\mathbb E\|f(x)\|_2^2=\|x\|_2^2$.

---

## Johnson–Lindenstrauss Lemma

The foundational result in random projection theory is the
Johnson–Lindenstrauss (JL) lemma.

{: .box-success}
Let $Q=\{x_1,\ldots,x_q\}\subset\mathbb{R}^N$ and let $\epsilon\in(0,1)$.
There exists a linear map
$f:\mathbb{R}^N\to\mathbb{R}^n$ with
$$
n = O\!\left(\frac{\log q}{\epsilon^2}\right)
$$
such that, for all $u,v\in Q$,
$$
(1-\epsilon)\|u-v\|_2^2
\le
\|f(u)-f(v)\|_2^2
\le
(1+\epsilon)\|u-v\|_2^2.
$$

Moreover, a random projection with i.i.d. Gaussian or Rademacher entries
satisfies this property with high probability.

---

## Interpretation

- The embedding dimension $n$ depends **logarithmically** on the number of points,
  not on the ambient dimension $N$.
- Pairwise Euclidean distances are approximately preserved.
- The result is non-adaptive: the same random map works for all pairs in $Q$.

This phenomenon is a manifestation of **concentration of measure** in high-
dimensional probability.

---

## Distance and Inner Product Preservation

Distance preservation implies approximate inner product preservation.
For centered data,
$$
\langle u,v\rangle
=
\frac{1}{2}\left(\|u\|_2^2 + \|v\|_2^2 - \|u-v\|_2^2\right).
$$

Thus, JL embeddings preserve:
- angles between vectors,
- cosine similarity,
- norms of individual vectors.

---

## Subspace Embeddings

The JL lemma extends beyond finite point sets.

Let $S\subset\mathbb{R}^N$ be a fixed $k$-dimensional subspace. A random projection
$f:\mathbb{R}^N\to\mathbb{R}^n$ with
$$
n = O\!\left(\frac{k}{\epsilon^2}\right)
$$
satisfies
$$
(1-\epsilon)\|x\|_2^2 \le \|f(x)\|_2^2 \le (1+\epsilon)\|x\|_2^2
\quad \forall x\in S
$$
with high probability.

Such maps are called **oblivious subspace embeddings**.

<!-- ---

## Connections to Linear Algebra

Random projections interact naturally with matrix decompositions.

- **Sketching**: For a data matrix $X\in\mathbb{R}^{T\times N}$,
  $XR^\top$ is a low-dimensional sketch preserving column geometry.
- **Approximate SVD/PCA**: Random projections reduce dimension before applying SVD.
- **Least squares**: Subspace embeddings yield fast approximate solvers.

These ideas underpin randomized numerical linear algebra.

---

## Geometry of Random Projections

Geometrically, random projections:
- approximately preserve Euclidean balls,
- map high-dimensional spheres to nearly spherical clouds,
- flatten anisotropy without strong distortion.

This explains their robustness and broad applicability.

---

## Beyond Gaussian Projections

Variants of JL embeddings include:
- sparse JL transforms (faster multiplication),
- fast JL transforms (FFT-based),
- structured random features.

The core geometry remains unchanged as long as concentration holds.

---

## Limitations

- Guarantees are probabilistic, not deterministic.
- Distortion bounds apply uniformly only to finite sets or fixed subspaces.
- Extremely small $\epsilon$ requires large $n$. -->

---

{: .box-note}
>- Random projections are geometry-preserving, not data-adaptive.
>- They complement, rather than replace, structured decompositions like SVD.
>- JL-type results explain why high-dimensional data often behaves
  “as if” it were low-dimensional.

