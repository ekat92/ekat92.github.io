---
layout: post
title: Matrix Decompositions
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

<p class="dropcap">T</p>his post collects the most important matrix decompositions used in
dimensionality reduction, optimization, and statistical learning.
All results here are deterministic and linear-algebraic; probabilistic
and asymptotic tools are treated separately.

---

## Spectral Decomposition (Symmetric Matrices)

Let $A\in\mathbb{R}^{n\times n}$ be symmetric. Then $A$ admits the spectral
decomposition
$$
A = \sum_{i=1}^n \lambda_i v_i v_i^\top,
$$
where $\lambda_1\ge\cdots\ge\lambda_n$ are real eigenvalues and
$\{v_i\}_{i=1}^n$ is an orthonormal basis of $\mathbb{R}^n$.

This decomposition underlies principal component analysis (PCA),
covariance matrices, and quadratic forms.

---

## Singular Value Decomposition (SVD)

For any matrix $A\in\mathbb{R}^{m\times n}$ with rank $r$,
$$
A = \sum_{i=1}^r s_i\,u_i v_i^\top,
$$
where $s_1\ge\cdots\ge s_r>0$ are singular values,
$u_i\in\mathbb{R}^m$ and $v_i\in\mathbb{R}^n$ are orthonormal vectors.

The singular values satisfy
$$
s_i^2 = \lambda_i(A^\top A).
$$

Equivalently, $A = U\Sigma V^\top$, where
$\Sigma=\mathrm{diag}(s_1,\ldots,s_r)$.

The SVD generalizes the spectral decomposition to rectangular matrices.

---

## Courant–Fischer Min–Max Theorem

Let $A\in\mathbb{R}^{n\times n}$ be symmetric with eigenvalues
$\lambda_1\ge\cdots\ge\lambda_n$.

The largest eigenvalue admits the variational characterization
$$
\lambda_1 = \max_{\|z\|_2=1} z^\top A z.
$$

More generally, the $k$-th largest eigenvalue satisfies
$$
\lambda_k
=
\min_{\dim(S)=n-k+1}\;
\max_{z\in S,\ \|z\|_2=1} z^\top A z.
$$

---

### Semidefinite Programming Formulation

An equivalent formulation of the top eigenvalue problem is the SDP
$$
\max_{Z\succeq 0,\ \mathrm{tr}(Z)=1} \ \mathrm{tr}(AZ).
$$

This representation plays an important role in convex relaxations and
spectral methods.

---

## Eckart–Young–Mirsky Theorem

Let $A=\sum_{i=1}^r s_i u_i v_i^\top$ be the SVD of $A$.
For any $k<r$, define the truncated SVD
$$
A_k = \sum_{i=1}^k s_i u_i v_i^\top.
$$

Then $A_k$ solves
$$
\min_{\mathrm{rank}(B)\le k} \|A-B\|_F
\quad\text{and}\quad
\min_{\mathrm{rank}(B)\le k} \|A-B\|_2.
$$

Thus, truncated SVD provides the best low-rank approximation of $A$
under both Frobenius and spectral norms.

---

## Polar Decomposition

Any matrix $A\in\mathbb{R}^{m\times n}$ admits the polar decomposition
$$
A = QH,
$$
where $Q$ has orthonormal columns and
$$
H = (A^\top A)^{1/2}
$$
is symmetric positive semidefinite.

The polar decomposition separates rotational and scaling components
of a linear map.

---

## QR Decomposition

For $A\in\mathbb{R}^{m\times n}$ with $m\ge n$, there exists a decomposition
$$
A = QR,
$$
where $Q\in\mathbb{R}^{m\times n}$ has orthonormal columns
and $R\in\mathbb{R}^{n\times n}$ is upper triangular.

The QR decomposition is fundamental for least squares problems and
numerical linear algebra algorithms.

---

## Schur Decomposition

For any square matrix $A\in\mathbb{R}^{n\times n}$, there exists an
orthogonal matrix $Q$ such that
$$
A = QTQ^\top,
$$
where $T$ is upper triangular.

The eigenvalues of $A$ appear on the diagonal of $T$.
The Schur decomposition is useful when eigenvectors are ill-conditioned
or non-orthogonal.

---


{: .box-note}
>- Spectral decomposition applies only to symmetric matrices; SVD applies
  to all matrices.
>- Low-rank approximations, PCA, and matrix denoising are all consequences
  of SVD and Eckart–Young.
>- Variational characterizations connect matrix decompositions to
  optimization and convex analysis.

Probabilistic tools (asymptotic notation, convergence theorems) and
randomized embeddings are treated separately.
