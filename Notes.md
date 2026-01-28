---
layout: page
title: Notes
subtitle: 
---
<style>
  img:hover {
    filter: drop-shadow(0px 0px 5px var(--footertextcol));
  }

  .card-img-top {
    filter: grayscale(50%);
  }

  .roundedpic {
    border-radius: 25%;
  }

  .wrapper {
    max-width: 1024px;
    margin: 0 auto;
  }

  .wrapper>* {
    background-color: transparent;
    border-radius: 5px;
    padding: 10px;
  }

  .wrapper {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    align-content: space-between;
    justify-content: left;
    grid-template-columns: repeat(12, [col-start] 1fr);
    grid-gap: 20px;
  }

  .item1 {
    grid-column: col-start 1 / span 3;
    grid-row: 1 / 9;
  }

  .item2 {
    grid-column: col-start 4 / span 9;
    grid-row: 1 / 9;
  }

  .badge {
    padding: 3px 8px 5px;
    font-size: inherit;
    font-weight: inherit;
    background-color: var(--headbackcol);
    border-radius: 9px;
  }

  .badge:hover,
  .badge:focus {
    color: var(--headbackcol);
    background-color: var(--footertextcol);
    cursor: pointer;
  }

  .card {
    color: inherit;
    background-color: var(--headbackcol);
    border-radius: 5px;
  }

  .col-md-9 {
    max-width: 80%;
    flex-basis: 500%;
  }

  .modal-content {
    background-color: var(--headbackcol);
  }

  input,
  textarea {
    background-color: var(--footertextcol);
    width: 90%;
  }

  ::placeholder {
    color: var(--backcol);
    opacity: 1;
  }

  .row {
    flex-wrap: nowrap;
  }

  .center {
    display: flex;
    align-items: center;
  }

  .img-fluid {
    max-height: 10rem;
  }

  .htrans {
    color: inherit;
  }

  .htrans:hover {
    color: inherit;
  }

  .htrans:hover {
    color: inherit;
  }

  .htrans:focus {
    color: inherit;
  }

  @media screen and (max-width: 550px) {
    .wrapper {
      justify-content: center;
    }

    .item1 {
      max-height: 300px;
    }

    .item2 {
      text-align: center;
    }

    .card {
      margin: 0 auto;
      /* Added */
      float: none;
      /* Added */
      margin-bottom: 10px;
      /* Added */
      width: 100%;
    }

    .img-fluid {
      display: none;
    }

    .col-md-9 {
      max-width: 100%;
    }
  }
</style>


<div class="card mb-1">
  <div class="row no-gutters" style="justify-content:space-between">
    <div class="col-md-9">
      <div class="card-body">
        <h3 class="card-title"><a class="htrans" href="{{ '2026-01-01-Norms' | relative_url }}">Norms and Inequalities</a></h3>
        <p class="card-text">Measuring size, distance, and stability in vector and matrix spaces through norms and their fundamental inequalities.</p>
      </div>
    </div>
    <div class="center">
      <a href="{{ '2026-01-01-Norms' | relative_url }}" class="post-image">
        <img src="{{ 'assets/img/blog1.png' | relative_url }}" class="img-fluid rounded-start" alt="...">
      </a>
    </div>
  </div>
</div>


<div class="card mb-1">
  <div class="row no-gutters" style="justify-content:space-between">
    <div class="col-md-9">
      <div class="card-body">
        <h3 class="card-title"><a class="htrans" href="{{ '2026-01-01-Matrix-Decompositions' | relative_url }}">Matrix Decompositions</a></h3>
        <p class="card-text">Canonical matrix decompositions and variational characterizations that underpin dimensionality reduction, optimization, and spectral methods</p>
      </div>
    </div>
    <div class="center">
      <a href="{{ '2026-01-01-Matrix-Decompositions' | relative_url }}" class="post-image">
        <img src="{{ 'assets/img/blog2_upd.png' | relative_url }}" class="img-fluid rounded-start" alt="...">
      </a>
    </div>
  </div>
</div>


<div class="card mb-1">
  <div class="row no-gutters" style="justify-content:space-between">
    <div class="col-md-9">
      <div class="card-body">
        <h3 class="card-title"><a class="htrans" href="{{ '2026-01-01-Asymptotic-Notations' | relative_url }}">Asymptotic Notation and Stochastic Convergence</a></h3>
        <p class="card-text">Standard asymptotic notation and probabilistic limit tools for analyzing convergence, consistency, and stochastic approximation.</p>
      </div>
    </div>
    <div class="center">
      <a href="{{ '2026-01-01-Asymptotic-Notations' | relative_url }}" class="post-image">
        <img src="{{ 'assets/img/blog3_upd2.png' | relative_url }}" class="img-fluid rounded-start" alt="...">
      </a>
    </div>
  </div>
</div>


<div class="card mb-1">
  <div class="row no-gutters" style="justify-content:space-between">
    <div class="col-md-9">
      <div class="card-body">
        <h3 class="card-title"><a class="htrans" href="{{ '2026-01-01-Random-Projections' | relative_url }}">Random Projections</a></h3>
        <p class="card-text">Random linear embeddings and geometric principles for dimension reduction in high-dimensional spaces.</p>
      </div>
    </div>
    <div class="center">
      <a href="{{ '2026-01-01-Random-Projections' | relative_url }}" class="post-image">
        <img src="{{ 'assets/img/blog4_upd.png' | relative_url }}" class="img-fluid rounded-start" alt="...">
      </a>
    </div>
  </div>
</div>

<div class="card mb-1">
  <div class="row no-gutters" style="justify-content:space-between">
    <div class="col-md-9">
      <div class="card-body">
        <h3 class="card-title"><a class="htrans" href="{{ '2026-01-01-Matrix-Concentration-and-Perturbation-Inequalities' | relative_url }}">Matrix Concentration and Perturbation Inequalities</a></h3>
        <p class="card-text">Probabilistic inequalities and perturbation bounds governing the behavior of random matrices and their spectra.</p>
      </div>
    </div>
    <div class="center">
      <a href="{{ '2026-01-01-Matrix-Concentration-and-Perturbation-Inequalities' | relative_url }}" class="post-image">
        <img src="{{ 'assets/img/blog5_upd2.png' | relative_url }}" class="img-fluid rounded-start" alt="...">
      </a>
    </div>
  </div>
</div>
