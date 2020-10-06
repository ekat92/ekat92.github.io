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


<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "Sparse Portfolio"</b> <i>(submitted to The Review of Financial Studies)</i>
  </div>
  <div class="item2">
    <p class="dropcap">T</p>he classical approach to portfolio optimization is notorious for producing undesirable extreme long and short positions due to inaccurate estimation of asset weights that fluctuate substantially over time. Besides, its asset allocations are associated with non-negligible transaction costs, high turnover and large monitoring costs. To overcome these shortcomings, we develop a novel optimization approach which produces sparse wealth allocations by setting some weights to zero using a penalty function. The proposed statistical method proceeds in two steps: first, it uses an $\ell_1$-penalty on the weight vector to select stocks, second, we apply de-biasing and post-lasso to obtain the optimal asset allocation weights. The main contribution is twofold: from the theoretical perspective, this paper establishes unbiasedness and consistency of the optimal sparse allocations in a high-dimensional setting, when the number of assets exceeds the sample size. We demonstrate the importance of the de-biasing step that has been overlooked in previous studies. From the empirical perspective, the application to the constituents of the S&P500 reveals that compared to the common strategy of holding all assets, our sparse portfolio strategy leads to lower risk, lower turnover, and higher out-of-sample Sharpe ratio. We illustrate that during several economic downturns including the dot-com bubble of 2000 and the financial crisis of 2007-09, our sparse de-biased estimator was the only model that produced positive cumulative excess return (CER) and did not exceed the target level of risk. In contrast, all non-sparse models produced negative CER and violated the risk constraint. This finding suggests that our de-biased sparse estimator exhibits desirable minimax properties: it minimizes the maximum risk level of a portfolio.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/JMP.pdf" type="button" class="btn btn-new btn-sm" title="Job Market Paper"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Optimal Portfolio Using Factor Graphical Lasso"</b> <i>(submitted to the Journal of Business & Economic Statistics)</i>
  </div>
  <div class="item2">
    <p class="dropcap">G</p>raphical models are a powerful tool to estimate a high-dimensional inverse covariance (<i>precision</i>) matrix, which has been applied for portfolio allocation problem. The assumption made by these models is a sparsity of the precision matrix. However, when the stock returns are driven by the common factors, this assumption does not hold.
		Our paper develops a framework for estimating a high-dimensional precision matrix which combines the benefits of exploring the factor structure of the stock returns and the sparsity of the precision matrix of the factor-adjusted returns. The proposed algorithm is called <i>Factor Graphical Lasso</i> (FGL). We study a high-dimensional portfolio allocation problem when the asset returns admit the approximate factor model. In high dimensions, when the number of assets is large relative to the sample size, the sample covariance matrix of the excess returns is subject to the large estimation uncertainty, which leads to unstable solutions for portfolio weights. To resolve this issue, we consider the decomposition of low-rank and sparse components. This strategy allows us to consistently estimate the optimal portfolio in high dimensions, even when the covariance matrix is ill-behaved. We establish consistency of the portfolio weights in a high-dimensional setting <i>without assuming sparsity on the covariance or precision matrix of stock returns</i>. Our theoretical results and simulations demonstrate that FGL is robust to heavy-tailed distributions, which makes our method suitable for financial applications. The empirical application uses daily and monthly data for the constituents of the S&P500 to demonstrate superior performance of FGL compared to the equal-weighted portfolio, index and some prominent precision and covariance-based estimators. 
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/FGLabstract.pdf" type="button" class="btn btn-new btn-sm" title="Optimal Portfolio Using Factor Graphical Lasso"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>

<span style="display:block; height: 0px;"></span>

<div class="wrapper">
  <div class="item1">
    <b>TH Lee, E. Seregina, "Learning from Forecast Errors: A New Approach to Forecast Combination"</b> <i>(submitted to the International Journal of Forecasting)</i>
  </div>
  <div class="item2">
    <p class="dropcap">T</p>his paper studies forecast combination (as an expert system) using the precision matrix estimation of forecast errors when the latter admit the approximate factor model. This approach incorporates the facts that experts often use common sets of information and hence they tend to make common mistakes. This premise is evidenced in many empirical results. For example, the European Central Bank's Survey of Professional Forecasters on Euro-area real GDP growth demonstrates that the professional forecasters tend to <i>jointly</i> understate or overstate GDP growth. Motivated by this stylized fact, we develop a novel framework which exploits the factor structure of forecast errors and the sparsity in the precision matrix of the idiosyncratic components of the forecast errors. The proposed algorithm is called <i>Factor Graphical Model</i> (FGM). Our approach overcomes the challenge of obtaining the forecasts that contain unique information, which was shown to be necessary to achieve a "winning" forecast combination. In simulation, we demonstrate the merits of the FGM in comparison with the equal-weighted forecasts and the standard graphical methods in the literature. An empirical application to forecasting macroeconomic time series in big data environment highlights the advantage of the FGM approach in comparison with the existing methods of forecast combination. 
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/Forecastingabstract.pdf" type="button" class="btn btn-new btn-sm" title="Learning from Forecast Errors"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
      </div>
</div>

<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>V. Kutateladze, E. Seregina, "Fast and Efficient Data Science Techniques for Covid-19 Group Testing"</b> <i>(2020 NABE Tech Economics Conference: Virtual Poster Session: Finalist)</i>
  </div>
  <div class="item2">
    <p class="dropcap">R</p>esearchers and public officials tend to agree that until a vaccine is developed, stopping SARS-CoV-2 transmission is the name of the game. Testing is the key to preventing the spread, especially by asymptomatic individuals. With testing capacity restricted, group testing is an appealing alternative for comprehensive screening and has recently received FDA emergency authorization. This technique tests pools of individual samples, thereby often requiring fewer testing resources while potentially providing multiple folds of speedup. We approach group testing from a data science perspective and offer two contributions. First, we provide an extensive empirical comparison of modern group testing techniques based on simulated and real, laboratory data. Second, we propose a simple one-round method based on $\ell_1$-norm sparse recovery, which outperforms current state-of-the-art approaches at certain disease prevalence rates.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="Covid-19 Group Testing"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
      <span style="display:block; height: 7px;"></span>
      <a href="/pdfs/covidslides.pdf" type="button" class="btn btn-new btn-sm" title="CV"><i class="fas fa-file-pdf fa-lg"></i><b> Slides</b></a>
    </center>
  </div>
</div>
<span style="display:block; height: 0px;"></span>


<div class="wrapper">
  <div class="item1">
    <b>E. Seregina, "Time-Varying Factor Graphical Models"</b>
  </div>
  <div class="item2">
    <p class="dropcap">A</p>t the beginning of COVID-19 outbreak, stock market was volatile, exhibiting sudden trend switches. As a result, using a long history of the past performance leads to large estimation errors. One efficient way to overcome this difficulty is to use the information extracted from higher frequency returns, e.g. daily data, to make longer term predictions of lower frequency returns, e.g. monthly data. Such strategy naturally augments the information set for the monthly data leading to decreased estimation errors and improved performance. This paper proposes to estimate the lower frequency precision matrix using higher frequency returns. In addition, we allow the dependence structure between stocks to change over time, which makes the proposed model more flexible. We call the proposed algoritm "Time-Varying Factor Graphical Model". Our model is solved using the alternating directions method of multipliers (ADMM), we derive closed-form solutions for the ADMM subproblems to further speed up the runtime.
  </div>
  <div class="item3">
    <center> 
      <a href="/pdfs/CV.pdf" type="button" class="btn btn-new btn-sm" title="Time-Varying Factor Graphical Models"><i class="fas fa-file-pdf fa-lg"></i><b> Paper</b></a> 
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