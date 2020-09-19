---
layout: page
title: Research
subtitle:
---

<style>
.socialcolor{
  color: var(--footertextcol);
}
.btn-new{
  background-color:var(--footertextcol);color: var(--backcol);
}
.btn-new:hover{
  background-color:var(--posthovercol);color: white;
}
.wrapper {
max-width: 1024px;
margin: 0 auto;
}
.wrapper > * {
background-color: var(--headbackcol);
border-radius: 5px;
padding: 12px;
}
.wrapper {
display: grid;
grid-template-columns: repeat(12, [col-start] 1fr);
grid-gap: 5px;
}
.item1 {
grid-column: col-start 1 / span 12;
}
.item2 {
grid-column: col-start 1 / span 11 ;
grid-row: 2 / 7;
padding: 15px;
}
.item3 {
grid-column: col-start 12 / span 1;
grid-row: 2/7;
} 
</style>


<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "Sparse Portfolio"</b> 
  </div>
  <div class="item2">
    <p class="dropcap">T</p>he classical approach to portfolio optimization is notorious for producing undesirable extreme long and short positions due to inaccurate estimation of asset weights that fluctuate substantially over time. Besides, its asset allocations are associated with non-negligible transaction costs, high turnover and large monitoring costs. To overcome these shortcomings, we develop a novel optimization approach which produces sparse wealth allocations by setting some weights to zero using a penalty function. The proposed statistical method proceeds in two steps: first, it uses an $\ell_1$-penalty on the weight vector to select stocks, second, we apply de-biasing and post-lasso to obtain the optimal asset allocation weights. The main contribution is twofold: from the theoretical perspective, this paper establishes unbiasedness and consistency of the optimal sparse allocations in a high-dimensional setting, when the number of assets exceeds the sample size. We demonstrate the importance of the de-biasing step that has been overlooked in previous studies. From the empirical perspective, the application to the constituents of the S&P500 reveals that compared to the common strategy of holding all assets, our sparse portfolio strategy leads to lower risk, lower turnover, and higher out-of-sample Sharpe ratio. We illustrate that during several economic downturns including the dot-com bubble of 2000 and the financial crisis of 2007-09, our sparse de-biased estimator was the only model that produced positive cumulative excess return (CER) and did not exceed the target level of risk. In contrast, all non-sparse models produced negative CER and violated the risk constraint. This finding suggests that our de-biased sparse estimator exhibits desirable minimax properties: it minimizes the maximum risk level of a portfolio.

  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/JMP.pdf" type="button" class="btn btn-new btn-sm" title="Job Market Paper"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="1-page CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>Author, "Paper Title "</b><i>(submitted to Journal)</i>
  </div>
  <div class="item2">
    <p class="dropcap">A</p>bstract goes here Sample abstract goes here Sample abstract goes here Sample abstract goes here 
    Sample abstract goes here Sample abstract goes here Sample abstract goes here Sample abstract goes here 
    Sample abstract goes here Sample abstract goes here Sample abstract goes here Sample abstract goes here 
    Sample abstract goes here Sample abstract goes here Sample abstract goes here Sample abstract goes here 
  </div>
  <div class="item3">
    <center> 
      <span style="display:block; height: 15px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="1-page CV"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="1-page CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>


