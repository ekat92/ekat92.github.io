---
layout: post
title: Matrix Concentration and Perturbation Inequalities
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

<p class="dropcap">T</p>his post collects probabilistic inequalities and perturbation results that
control the behavior of random matrices and their spectra. These tools combine
norm geometry, matrix decompositions, and probabilistic concentration, and form
the theoretical backbone of modern high-dimensional statistics, random matrix
theory, and spectral algorithms.

All results here build on the foundations developed in the earlier posts on
norms, matrix decompositions, and asymptotic notation.

---

## From Scalar to Matrix Concentration

Classical concentration inequalities (Hoeffding, Bernstein, sub-Gaussian tails)
control sums of independent random variables. In high-dimensional settings, the
objects of interest are often matrices, and the relevant quantities are operator
norms, eigenvalues, and eigenspaces.

Matrix concentration inequalities extend scalar results to this setting.

---

## Sub-Gaussian and Sub-Exponential Random Variables

A random variable $X$ is **sub-Gaussian** if there exists $K>0$ such that
$$
\mathbb E e^{tX} \le e^{K^2 t^2/2}
\quad \forall t\in\mathbb R.
$$

It is **sub-exponential** if
$$
\mathbb E e^{tX} \le e^{K^2 t^2}
\quad \text{for } |t| \text{ small}.
$$

These tail conditions underlie most matrix concentration results.

---

## Hanson–Wright Inequality (Quadratic Forms)

Let $x\in\mathbb R^n$ be a random vector with independent, mean-zero,
sub-Gaussian entries with parameter $K$. For any fixed matrix $A\in\mathbb R^{n\times n}$,

$$
\mathbb P\!\left(
\big|x^\top A x - \mathbb E[x^\top A x]\big| > t
\right)
\le
2\exp\!\left[
- c \min\!\left(
\frac{t^2}{K^4 \|A\|_F^2},
\frac{t}{K^2 \|A\|_2}
\right)
\right].
$$

The Hanson–Wright inequality controls fluctuations of quadratic forms and is a
key building block for covariance and Gram matrix analysis.

---

## Matrix Bernstein Inequality

Let $\{X_k\}$ be independent, mean-zero random matrices in $\mathbb R^{d\times d}$.
Assume
$$
\|X_k\|_2 \le L \quad \text{almost surely}.
$$

Define the variance parameter
$$
\sigma^2 := \left\| \sum_k \mathbb E(X_k^2) \right\|_2.
$$

Then for all $t\ge 0$,
$$
\mathbb P\!\left(
\left\|\sum_k X_k\right\|_2 \ge t
\right)
\le
2d \exp\!\left(
-\frac{t^2/2}{\sigma^2 + Lt/3}
\right).
$$

Matrix Bernstein generalizes scalar Bernstein inequalities to operator norms.

---

## Spectral Norm Concentration of Random Matrices

### Sub-Gaussian Noise Matrices

Let $E\in\mathbb R^{m\times n}$ have i.i.d. mean-zero sub-Gaussian entries with
variance proxy $\sigma^2$. Then with high probability,
$$
\|E\|_2
\le
C \sigma \left(\sqrt{m} + \sqrt{n}\right).
$$

This bound is sharp up to constants and is fundamental in low-rank recovery and
denoising.

---

### Sample Covariance Concentration

Let $X_1,\dots,X_n\in\mathbb R^p$ be i.i.d. sub-Gaussian with covariance $\Sigma$.
The sample covariance satisfies
$$
\left\|\frac{1}{n}\sum_{i=1}^n X_i X_i^\top - \Sigma\right\|_2
=
\mathcal O_p\!\left(\|\Sigma\|_2 \sqrt{\frac{p}{n}}\right).
$$

This result underlies consistency of PCA in high dimensions.

---

## Weyl’s Inequality (Eigenvalue Perturbation)

For symmetric matrices $A$ and $E$,
$$
|\lambda_i(A+E) - \lambda_i(A)| \le \|E\|_2
\quad \forall i.
$$

Weyl’s inequality controls eigenvalue stability under perturbations.

---

### Principal Angles Between Subspaces

Let $V,\widehat V \in \mathbb{R}^{n\times r}$ have orthonormal columns, and let
$\mathcal S=\mathrm{col}(V)$ and $\widehat{\mathcal S}=\mathrm{col}(\widehat V)$.
The principal angles $\theta_1,\ldots,\theta_r \in [0,\pi/2]$ between
$\mathcal S$ and $\widehat{\mathcal S}$ are defined by
$$
\cos \theta_i = s_i(V^\top \widehat V),
$$
where $s_i(\cdot)$ denotes the singular values in decreasing order.

Define $\sin\Theta(\widehat V, V)$ as the diagonal matrix with entries
$\sin\theta_1,\ldots,\sin\theta_r$. Its operator norm satisfies
$$
\|\sin\Theta(\widehat V, V)\|_2
=
\|V_\perp^\top \widehat V\|_2,
$$
where $V_\perp$ spans the orthogonal complement of $\mathcal S$.

---

## Davis–Kahan $\sin\Theta$ Theorem (Eigenspace Perturbation)

Let $A$ and $\widehat A = A + E$ be symmetric. Let $V$ and $\widehat V$ be the
matrices of eigenvectors corresponding to a cluster of eigenvalues of $A$,
separated by a spectral gap $\delta>0$.

Then
$$
\|\sin\Theta(\widehat V, V)\|_2
\le
\frac{\|E\|_2}{\delta}.
$$

This theorem quantifies how noise affects eigenvectors and is central to PCA,
factor models, and spectral clustering.

---

## Low-Rank Plus Noise Models

Consider the model
$$
Y = L + E,
$$
where $\mathrm{rank}(L)=r$ and $E$ is random noise.

Basic norm bounds yield
$$
\|Y\|_2 \le \|L\|_2 + \|E\|_2,
\qquad
\|Y\|_F^2 = \|L\|_F^2 + \|E\|_F^2 + 2\langle L,E\rangle.
$$

Combined with spectral concentration,
$$
\|E\|_2 = \mathcal O_p(\sqrt{m}+\sqrt{n}),
$$
one obtains consistency and error bounds for truncated SVD estimators.

---

## Nuclear Norm Bounds and Duality

For any matrices $A,B$,
$$
|\mathrm{tr}(A^\top B)|
\le
\|A\|_*\,\|B\|_2.
$$

This inequality underpins convex relaxations for low-rank recovery and matrix
completion.

---

## Summary of Core Inequalities

| Tool | Controls |
|----|----|
| Hanson–Wright | Quadratic forms |
| Matrix Bernstein | Spectral norm of sums |
| Weyl | Eigenvalues |
| Davis–Kahan | Eigenspaces |
| Sub-Gaussian norm bounds | Noise matrices |
| Nuclear–spectral duality | Low-rank recovery |

---


{: .box-note}
>- Matrix concentration inequalities explain why spectral methods are stable
  under randomness.
>- Perturbation results translate norm bounds into eigenvalue and eigenvector
  guarantees.
>- Together, these tools bridge deterministic linear algebra and stochastic
  high-dimensional models.


