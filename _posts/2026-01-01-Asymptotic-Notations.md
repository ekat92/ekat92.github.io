---
layout: post
title: Asymptotic Notation and Stochastic Convergence
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

<p class="dropcap">T</p>his post collects standard asymptotic notation and probabilistic limit tools
used in statistical theory, econometrics, and stochastic optimization.
All statements are formulated for sequences indexed by the sample size $n$
and are independent of linear-algebraic structure.

---

## Deterministic Asymptotic Notation

Let $\{f_n\}$ and $\{g_n\}$ be sequences of real numbers with $g_n>0$.

- **Big-O notation**:
  $$
  f_n = \mathcal O(g_n)
  \quad \Longleftrightarrow \quad
  \exists C>0,\ \exists n_0 \text{ s.t. } |f_n| \le C g_n
  \ \forall n\ge n_0.
  $$

- **Little-o notation**:
  $$
  f_n = o(g_n)
  \quad \Longleftrightarrow \quad
  \lim_{n\to\infty} \frac{f_n}{g_n} = 0.
  $$

- **Big-Omega notation**:
  $$
  f_n = \Omega(g_n)
  \quad \Longleftrightarrow \quad
  g_n = \mathcal O(f_n).
  $$

- **Theta notation**:
  $$
  f_n = \Theta(g_n)
  \quad \Longleftrightarrow \quad
  f_n = \mathcal O(g_n)\ \text{and}\ g_n = \mathcal O(f_n).
  $$

These notions compare deterministic growth rates.

---

## Stochastic Order Notation

Let $\{X_n\}$ be a sequence of random variables and let $g_n>0$.

### Boundedness in probability

$$
\boxed{
\begin{aligned}
X_n = &\mathcal O_p(g_n)
\iff\;
\forall\,\epsilon>0,\ \exists\,M>0:\ 
\\
&\sup_n \mathbb P\!\left(|X_n|>Mg_n\right) < \epsilon
\end{aligned}
}
$$



Equivalently, $\{X_n/g_n\}$ is tight.

---

### Convergence to zero in probability

$$
\boxed{
X_n = o_p(g_n)
\quad \Longleftrightarrow \quad
\frac{X_n}{g_n} \xrightarrow{p} 0
}
$$

That is,
$$
\forall \epsilon>0,\quad
\lim_{n\to\infty}
\mathbb P\!\left( |X_n| > \epsilon g_n \right) = 0.
$$

---

## Algebra of $\mathcal O_p$ and $o_p$

Let $X_n,Y_n$ be random variables and $f_n,g_n>0$.

### Products
- If $X_n=\mathcal O_p(f_n)$ and $Y_n=\mathcal O_p(g_n)$, then
  $$
  X_n Y_n = \mathcal O_p(f_n g_n).
  $$
- If $X_n=o_p(f_n)$ and $Y_n=\mathcal O_p(g_n)$, then
  $$
  X_n Y_n = o_p(f_n g_n).
  $$

---

### Sums
- If $X_n=\mathcal O_p(f_n)$ and $Y_n=\mathcal O_p(g_n)$, then
  $$
  X_n+Y_n = \mathcal O_p\!\big(\max\{f_n,g_n\}\big).
  $$
- If $X_n=o_p(f_n)$ and $Y_n=o_p(g_n)$, then
  $$
  X_n+Y_n = o_p\!\big(\max\{f_n,g_n\}\big).
  $$

---

### Powers
For any $s>0$,
$$
X_n = \mathcal O_p(f_n) \;\Rightarrow\; |X_n|^s = \mathcal O_p(f_n^s),
$$
and similarly for $o_p$.

---

## Modes of Convergence

Let $X_n,X$ be random variables.

- **Almost sure convergence**:
  $$
  X_n \xrightarrow{a.s.} X
  \quad \Longleftrightarrow \quad
  \mathbb P\!\left(\lim_{n\to\infty} X_n = X\right)=1.
  $$

- **Convergence in probability**:
  $$
  X_n \xrightarrow{p} X
  \quad \Longleftrightarrow \quad
  \forall\epsilon>0,\ 
  \mathbb P(|X_n-X|>\epsilon)\to 0.
  $$

- **Convergence in distribution**:
  $$
  X_n \xrightarrow{d} X
  \quad \Longleftrightarrow \quad
  F_{X_n}(t)\to F_X(t)
  \ \text{at all continuity points of } F_X.
  $$

Relationship:
$$
X_n\xrightarrow{a.s.}X \;\Rightarrow\; X_n\xrightarrow{p}X
\;\Rightarrow\; X_n\xrightarrow{d}X.
$$

---

## Continuous Mapping Theorem

Let $X_n\xrightarrow{d}X$ and let $f:\mathbb R^k\to\mathbb R^m$
be continuous almost everywhere with respect to the law of $X$.

Then:
$$
f(X_n)\xrightarrow{d} f(X).
$$

If $X_n\xrightarrow{p}X$, then
$$
f(X_n)\xrightarrow{p} f(X).
$$

---

## Slutsky’s Lemma

If
$$
X_n\xrightarrow{d}X,
\qquad
Y_n\xrightarrow{p}c,
$$
where $c$ is constant, then:
- $X_n+Y_n \xrightarrow{d} X+c$,
- $X_n Y_n \xrightarrow{d} cX$,
- $X_n/Y_n \xrightarrow{d} X/c$ (if $c\neq 0$).

---

## Weak Law of Large Numbers (WLLN)

Let $\{X_i\}$ be i.i.d. with $\mathbb E[X_i]=\mu$ and
$\mathbb E[X_i^2]<\infty$. Then
$$
\frac{1}{n}\sum_{i=1}^n X_i \xrightarrow{p} \mu.
$$

---

## Central Limit Theorem (CLT)

Let $\{X_i\}$ be i.i.d. with $\mathbb E[X_i]=\mu$ and
$\mathrm{Var}(X_i)=\sigma^2<\infty$. Then
$$
\sqrt{n}\left(\frac{1}{n}\sum_{i=1}^n X_i - \mu\right)
\xrightarrow{d}
\mathcal N(0,\sigma^2).
$$

---

{: .box-note}
>- $\mathcal O_p$ and $o_p$ describe stochastic magnitude, not convergence.
>- Slutsky’s lemma and the continuous mapping theorem allow deterministic
  algebra to pass through limits.
>- These tools underpin consistency, asymptotic normality, and inference
  in econometrics and machine learning.

