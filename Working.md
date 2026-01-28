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
<div class="wrapper">
<div class="item1">
    <b>TH Lee, E. Seregina, "Combining Forecasts under Structural Breaks Using Graphical LASSO"</b> <i>(International Journal of Forecasting, 2025)</i>
  </div>
  <div class="item2">
    <p class="dropcap">I</p>n this paper we develop a novel method of combining many forecasts based on Graphical LASSO. We represent forecast errors from different forecasters as a network of interacting entities and generalize network inference in the presence of common factor structure and structural breaks. 
First, we note that forecasters often use common information and hence make common errors, which makes the forecast errors exhibit common factor structures. We separate common forecast errors from the idiosyncratic errors and exploit sparsity of the precision matrix of the latter.
Second, since the network of experts changes over time as a response to unstable environments, we propose Regime-Dependent Factor Graphical LASSO (RD-FGL) that allows factor loadings and idiosyncratic precision matrix to be regime-dependent.
The empirical applications to forecasting macroeconomic series using the data of the European Central Bank's Survey of Professional Forecasters and Federal Reserve Economic Data monthly database demonstrate superior performance of a combined forecast using RD-FGL.
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.1016/j.ijforecast.2025.04.003" type="button" class="btn btn-new btn-sm" title="Combining Forecasts under Structural Breaks Using GLASSO"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
<div class="item1">
    <b>V. Kutateladze, E. Seregina, "Doubly Sparse Estimator for High-Dimensional Covariance Matrices"</b> <i>(Econometrics and Statistics, 2024)</i>
  </div>
  <div class="item2">
    <p class="dropcap">T</p>he classical sample covariance estimator lacks desirable properties such as consistency and suffers from eigenvalue spreading in high-dimensional settings. Improved estimators have been proposed that shrink sample eigenvalues but retain the eigenvectors of the sample covariance estimator. In high dimensions, however, sample eigenvectors are generally strongly inconsistent, rendering eigenvalue shrinkage estimators suboptimal. A Doubly Sparse Covariance Estimator (DSCE) is developed that goes beyond mere eigenvalue shrinkage: a covariance matrix is decomposed into a signal part, where sparse eigenvectors are estimated via truncation, and an idiosyncratic part, estimated via thresholding. It is shown that accurate estimation is possible if the leading eigenvectors are sufficiently sparse affecting proportionately less than $\sqrt{p}$ of the variables. DSCE fills the gap for empirical applications that fall in-between fully sparse settings and conditionally sparse settings: DSCE takes advantage of conditional sparsity implied by factor models while allowing only a subset of variables to load on factors, which relaxes pervasiveness assumption of traditional factor models. An empirical application to the constituents of the S&P 1500 illustrates that DSCE-based portfolios outperform competing methods in terms of Sharpe ratio, maximum drawdown, and cumulative return for monthly and daily data.
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.1016/j.ecosta.2024.06.001" type="button" class="btn btn-new btn-sm" title="Doubly Sparse Estimator for High-Dimensional Covariance Matrices"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
<div class="item1">
    <b>E. Seregina, "A Basket Half Full: Sparse Portfolios"</b> <i>(Quantitative Finance 2023 (12), 1833-1852)</i>
  </div>
  <div class="item2">
    <p class="dropcap">T</p>he existing approaches to sparse wealth allocations (1) are limited to low-dimensional setup when the number of assets is less than the sample size; (2) lack theoretical analysis of sparse wealth allocations and their impact on portfolio exposure; (3) are suboptimal due to the bias induced by an $\ell_1$-penalty. We address these shortcomings and develop an approach to construct sparse portfolios in high dimensions. Our contribution is twofold: from the theoretical perspective, we establish the oracle bounds of sparse weight estimators and provide guidance regarding their distribution. From the empirical perspective, we examine the merit of sparse portfolios during different market scenarios. We find that in contrast to non-sparse counterparts, our strategy is robust to recessions and can be used as a hedging vehicle during such times. 
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.1080/14697688.2023.2269997" type="button" class="btn btn-new btn-sm" title="Job Market Paper"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/JMPpres.pdf" type="button" class="btn btn-new btn-sm" title="Slides"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Optimal Portfolio Using Factor Graphical Lasso"</b> <i>(Journal of Financial Econometrics, 2023)</i>
  </div>
  <div class="item2">
    <p class="dropcap">G</p>raphical models are a powerful tool to estimate a high-dimensional inverse covariance (precision) matrix, which has been applied for a portfolio allocation problem. The assumption made by these models is a sparsity of the precision matrix. However, when stock returns are driven by common factors, such assumption does not hold. We address this limitation and develop a framework, Factor Graphical Lasso (FGL), which integrates graphical models with the factor structure in the context of portfolio allocation by decomposing a precision matrix into low-rank and sparse components. Our theoretical results and simulations show that FGL consistently estimates the portfolio weights and risk exposure and also that FGL is robust to heavy-tailed distributions which makes our method suitable for financial applications. FGL-based portfolios are shown to exhibit superior performance over several prominent competitors including equal-weighted and Index portfolios in the empirical application for the S&P500 constituents.
  </div>
  <div class="item3">
    <center> 
      <a href="https://academic.oup.com/jfec/advance-article-abstract/doi/10.1093/jjfinec/nbad011/7116303" type="button" class="btn btn-new btn-sm" title="Optimal Portfolio Using Factor Graphical Lasso"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "Graphical Models and their Interactions with Machine Learning in the Context of Economics and Finance"</b> <i>(In: Chan, F., Mátyás, L. (eds) Econometrics with Machine Learning. Advanced Studies in Theoretical and Applied Econometrics, vol 53. Springer, Cham.)</i>
  </div>
  <div class="item2">
    <p class="dropcap">M</p>any economic and financial systems, including financial markets, financial institutions, and macroeconomic policy making can be modelled as systems of interacting agents. Graphical models, which are the main focus of this chapter, are a means of estimating the relationships implied by such systems. The main goals of this chapter are (1) acquainting the readers with graphical models; (2) reviewing the existing research on graphical models for economic and finance problems; (3) reviewing the literature that merges graphical models with other machine learning methods in economics and finance.
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.1007/978-3-031-15149-1_8" type="button" class="btn btn-new btn-sm" title="Econometrics with Machine Learning"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
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
## Proceedings
<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, Y. Xu " Elicitability and Encompassing for Volatility Forecasts by Bregman Functions"</b> <i>(In JSM Proceedings 2023. Toronto, Canada)</i>
  </div>
  <div class="item2">
    <p class="dropcap">I</p>n this paper, we construct a class of strictly consistent scoring functions based on the Bregman divergence measure, which jointly elicit the mean and variance. We use the scoring functions to develop a novel out-of-sample forecast encompassing test in volatility predictive models. We show the encompassing test is asymptotically normal. Simulation results demonstrate the merits of the proposed Bregman scoring functions and the forecast encompassing test. The forecast encompassing test exhibits a proper size and good power in finite samples. In an empirical application, we investigate the predictive ability of macroeconomic and financial variables in forecasting the equity premium volatility.
  </div>
  <div class="item3">
    <center> 
      <a href="https://doi.org/10.5281/zenodo.8396034" type="button" class="btn btn-new btn-sm" title="Elicitability and Encompassing for Volatility Forecasts"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Optimal Financial Portfolio Using Graphical Lasso Under Unstable Environment"</b> <i>(In JSM Proceedings, Statistical Learning and Data Science Section. 2021. Alexandria, VA: American Statistical Association)</i>
  </div>
  <div class="item2">
    <p class="dropcap">U</p>nstable environments raise challenges for constructing a financial portfolio. In such scenarios, it is unrealistic to assume constant portfolio weights, whereas estimating weights using only post-break observations omits the information prior to the break point. This paper visualizes stock returns as a network of interacting entities and generalizes network inference in the presence of structural breaks. We estimate time-varying portfolio weights using pre- and post-break data when the stock returns are driven by common factors. Using the example of a strong structural break caused by the first wave of COVID-19 pandemic, we demonstrate that combining pre- and post-break observations for estimating portfolio weights improves portfolio return and Sharpe Ratio compared to constant weights and weights that use only post-break observations.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/LeeandSereginaJSM2021.pdf" type="button" class="btn btn-new btn-sm" title="FGL Under Unstable Environment"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>
## Working Papers
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>A. Brini, E. Seregina "A Nonlinear Target-Factor Model with Attention Mechanism for Mixed-Frequency Data"</b>
  </div>
  <div class="item2">
    <p class="dropcap">W</p>e propose Mixed-Panels-Transformer Encoder (MPTE), a novel framework for estimating factor models in panel datasets with mixed frequencies and nonlinear signals. Traditional factor models rely on linear signal extraction and require homogeneous sampling frequencies, limiting their applicability to modern high-dimensional datasets where variables are observed at different temporal resolutions. Our approach leverages Transformer-style attention mechanisms to enable context-aware signal construction through flexible, data-dependent weighting schemes that replace fixed linear combinations with adaptive reweighting based on similarity and relevance. We extend classical principal component analysis (PCA) to accommodate general temporal and cross-sectional attention matrices, allowing the model to learn how to aggregate information across frequencies without manual alignment or pre-specified weights. For linear activation functions, we establish consistency and asymptotic normality of factor and loading estimators, showing that our framework nests Target PCA as a special case while providing efficiency gains through transfer learning across auxiliary datasets. The nonlinear extension uses a Transformer architecture to capture complex hierarchical interactions while preserving the theoretical foundations. In simulations, MPTE demonstrates superior performance in nonlinear environments, and in an empirical application to 13 macroeconomic forecasting targets using a selected set of 48 monthly and quarterly series from the FRED-MD and FRED-QD databases, our method achieves competitive performance against established benchmarks. We further analyze attention patterns and systematically ablate model components to assess variable importance and temporal dependence. The resulting patterns highlight which indicators and horizons are most influential for forecasting.
  </div>
  <div class="item3">
    <center> 
      <a href="https://arxiv.org/pdf/2601.16274" type="button" class="btn btn-new btn-sm" title="Factor Model with Attention"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, Y. Xu "Higher Order Elicitability and Forecast Encompassing for Volatility Forecasts by Bregman Functions"</b>
  </div>
  <div class="item2">
    <p class="dropcap">M</p>ost papers in the literature on volatility forecast comparison use a scoring (loss) function that assumes that the conditional mean is zero and uses the realized variance as a proxy for true volatility. However, the rankings of volatility forecast models can be affected by the zero mean assumption and the finite sample quality of the proxy. In this paper, we construct a class of strictly consistent scoring functions based on the Bregman divergence measure, which can jointly elicit the mean and variance without the zero mean assumption and without using a proxy. We use the proposed Bregman scoring function to develop a forecast encompassing test for comparing the predictive ability of a large set of potential predictors in volatility forecast models. We also relate the Bregman score with the log score of the predictive Gaussian likelihood and compare them in terms of the finite sample properties (in size and power) of the forecast encompassing test. The simulation and empirical application demonstrate the merits of the proposed score functions and the encompassing test based on the Bregman score function and the log score.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="High-Dimensional Covariance Estimation"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
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