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
grid-column: col-start 1 / span 9;
grid-row: 1/2;
}
.item2 {
grid-column: col-start 1 / span 12 ;
grid-row: 2 / 7;
padding: 15px;
}
.item3 {
grid-column: col-start 10 / span 3;
grid-row: 1/2;
  display: flex;
  justify-content: center;
  align-items: center;
} 
</style>

## Publications
<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>V. Kutateladze, E. Seregina, "Fast and Efficient Data Science Techniques for Covid-19 Group Testing"</b> <i>(Journal of Data Science (2021), 1-19)</i>
  </div>
  <div class="item2">
    <p class="dropcap">R</p>esearchers and public officials tend to agree that until a vaccine is developed, stopping SARS-CoV-2 transmission is the name of the game. Testing is the key to preventing the spread, especially by asymptomatic individuals. With testing capacity restricted, group testing is an appealing alternative for comprehensive screening and has recently received FDA emergency authorization. This technique tests pools of individual samples, thereby often requiring fewer testing resources while potentially providing multiple folds of speedup. We approach group testing from a data science perspective and offer two contributions. First, we provide an extensive empirical comparison of modern group testing techniques based on simulated and real, laboratory data. Second, we propose a simple one-round method based on $\ell_1$-norm sparse recovery, which outperforms current state-of-the-art approaches at certain disease prevalence rates.
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.6339/21-JDS1011" type="button" class="btn btn-new btn-sm" title="Covid-19 Group Testing"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/covidslides.pdf" type="button" class="btn btn-new btn-sm" title="Covid-19 Group Testing"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/Covidposter.pdf" type="button" class="btn btn-new btn-sm" title="Covid-19 Group Testing"><i class="fas fa-file-pdf fa-lg"></i><b> Poster</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>
## Working Papers
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Optimal Portfolio Using Factor Graphical Lasso"</b> <i>(Revised & Resubmitted)</i>
  </div>
  <div class="item2">
    <p class="dropcap">G</p>raphical models are a powerful tool to estimate a high-dimensional inverse covariance (precision) matrix, which has been applied for a portfolio allocation problem. The assumption made by these models is a sparsity of the precision matrix. However, when stock returns are driven by common factors, such assumption does not hold. We address this limitation and develop a framework, Factor Graphical Lasso (FGL), which integrates graphical models with the factor structure in the context of portfolio allocation by decomposing a precision matrix into low-rank and sparse components. Our theoretical results and simulations show that FGL consistently estimates the portfolio weights and risk exposure and also that FGL is robust to heavy-tailed distributions which makes our method suitable for financial applications. FGL-based portfolios are shown to exhibit superior performance over several prominent competitors including equal-weighted and Index portfolios in the empirical application for the S&P500 constituents.
  </div>
  <div class="item3">
    <center> 
      <a href="https://arxiv.org/pdf/2011.00435.pdf" type="button" class="btn btn-new btn-sm" title="Optimal Portfolio Using Factor Graphical Lasso"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Combining Forecasts under Structural Breaks Using Graphical LASSO"</b>
  </div>
  <div class="item2">
    <p class="dropcap">I</p>n this paper we develop a novel method of combining many forecasts based on a machine learning algorithm called Graphical LASSO. We visualize forecast errors from different forecasters as a network of interacting entities and generalize network inference in the presence of common factor structure and structural breaks. 
First, we note that forecasters often use common information and hence make common mistakes, which makes the forecast errors exhibit common factor structures. We propose the Factor Graphical LASSO (Factor GLASSO), which separates common forecast errors from the idiosyncratic errors and exploits sparsity of the precision matrix of the latter.
Second, since the network of experts changes over time as a response to unstable environments such as recessions, it is unreasonable to assume constant forecast combination weights. Hence, we propose Regime-Dependent Factor Graphical LASSO (RD-Factor GLASSO) and develop its scalable implementation using the Alternating Direction Method of Multipliers (ADMM) to estimate regime-dependent forecast combination weights.
The empirical application to forecasting macroeconomic series using the data of the European Central Bank's Survey of Professional Forecasters (ECB SPF) demonstrates superior performance of a combined forecast using Factor GLASSO and RD-Factor GLASSO over forecast combinations using equal weights.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="Learning from Forecast Errors"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
      </div>
</div>

<span style="display:block; height: 0px;"></span>
<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "A Basket Half Full: Sparse Portfolios"</b> 
  </div>
  <div class="item2">
    <p class="dropcap">T</p>he existing approaches to sparse wealth allocations (1) are limited to low-dimensional setup when the number of assets is less than the sample size; (2) lack theoretical analysis of sparse wealth allocations and their impact on portfolio exposure; (3) are suboptimal due to the bias induced by an $\ell_1$-penalty. We address these shortcomings and develop an approach to construct sparse portfolios in high dimensions. Our contribution is twofold: from the theoretical perspective, we establish the oracle bounds of sparse weight estimators and provide guidance regarding their distribution. From the empirical perspective, we examine the merit of sparse portfolios during different market scenarios. We find that in contrast to non-sparse counterparts, our strategy is robust to recessions and can be used as a hedging vehicle during such times. 
  </div>
  <div class="item3">
    <center> 
      <a href="https://arxiv.org/pdf/2011.04278.pdf" type="button" class="btn btn-new btn-sm" title="Job Market Paper"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/JMPpres.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Learning from Forecast Errors: A New Approach to Forecast Combination"</b>
  </div>
  <div class="item2">
    <p class="dropcap">F</p>orecasters often use common information and hence make common mistakes. We propose a new approach, Factor Graphical Model (FGM), to forecast combinations that separates idiosyncratic forecast errors from the common errors. FGM exploits the factor structure of forecast errors and the sparsity of the precision matrix of the idiosyncratic errors. We prove the consistency of forecast combination weights and mean squared forecast error estimated using FGM, supporting the results with extensive simulations. Empirical applications to forecasting macroeconomic series shows that forecast combination using FGM outperforms combined forecasts using equal weights and graphical models without incorporating factor structure of forecast errors.
  </div>
  <div class="item3">
    <center> 
      <a href="https://arxiv.org/pdf/2011.02077.pdf" type="button" class="btn btn-new btn-sm" title="Learning from Forecast Errors"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/LearningfromForecastErrorsSlides.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
      </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Time-Varying Factor Graphical Models"</b>
  </div>
  <div class="item2">
    <p class="dropcap">B</p>uilding a financial portfolio at the times of structural breaks, such as the one caused by COVID-19 outbreak, is challenging due to a bias-variance trade-off.  In such scenarios, using only post-break observations leads to unstable and volatile portfolio allocations, whereas using full sample but ignoring the break point leads to a large bias in portfolio weights estimates. One efficient way to overcome this difficulty is to account for the structural change and use both pre- and post-break observations. This paper proposes to estimate time-varying precision matrix for portfolio optimization problem using pre- and post-break data when the stock returns are driven by common factors. We allow portfolio weights to change over time which makes the model more flexible. We call the proposed
algorithm ``Time-Varying Factor Graphical Model". Our model is solved using the alternating directions method of multipliers (ADMM), we derive closed-form solutions for the 
ADMM subproblems to further speed up the runtime. 
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="Time-Varying Factor Graphical Models"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/shortpres.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>V. Kutateladze, E. Seregina, "High-Dimensional Covariance Estimation"</b>
  </div>
  <div class="item2">
    <p class="dropcap">C</p>ovariance matrix estimates are required in a wide range of applied problems in multivariate data analysis, including portfolio and risk management in finance, factor models and testing in economics, and graphical models and classification in machine learning. In modern applications, where often the model dimensionality is comparable or even larger than the sample size, the classical sample covariance estimator lacks desirable properties, such as consistency, and suffers from eigenvalue spreading. In recent years, improved estimators have been proposed based on the idea of regularization. Specifically, such estimators, known as rotation-equivariant estimators, shrink the sample eigenvalues, while keeping the eigenvectors of the sample covariance estimator. In high dimensions, however, the sample eigenvectors will generally be strongly inconsistent, rendering eigenvalue shrinkage estimators suboptimal. We consider an estimator that goes beyond mere eigenvalue shrinkage and aims at precise estimation of eigenvectors in sparse settings, without requiring eigenvalues to diverge. The rate of convergence is provided in terms of spectral norm and it achieves the optimal rate under reasonable assumptions. We also provide a numerical simulation demonstrating the superior performance of the proposed estimator as compared to the competition.	
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/Covariance.pdf" type="button" class="btn btn-new btn-sm" title="High-Dimensional Covariance Estimation"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "Projected Factor Graphical Models"</b>
  </div>
  <div class="item2">
    <p class="dropcap">F</p>undamental analysis and the mean-variance portfolio optimization are traditionally viewed as two alternative approaches to portfolio allocation. In this paper we develop a novel precision matrix estimator that integrates these approaches. The proposed algorithm is called "Projected Factor Graphical Models". Our method allows to incorporate the information on the companies’ fundamentals, such as current earnings, growth in net operating assets and growth in financing, when deciding which stocks to include in the portfolio and how much to invest in these stocks. Using the fact that, at some point, the stock’s market value will converge to its intrinsic value, we use the partial equilibrium returns model that governs the behavior of stock returns as a linear function of firm’s characteristics. The latter is used to construct a precision matrix estimator for portfolio weights.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="Projected Factor Graphical Models"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>