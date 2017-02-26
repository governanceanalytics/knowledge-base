## Cross-sectional and General Issues

***Endogeneity Bias***

> Angrist, J. D. and J. S. Pischke. 2009. Mostly Harmless Econometrics: An Empiricist's Companion.  Princeton: Princeton University Press.

*Stata command: ivreg2*

***Sample Selection Bias***

> Heckman, J. J. 1976. The Common Structure of Statistical Models of Truncation, Sample Selection, and Limited Dependent Variables and a Simple Estimator for Such Model, Annuals of Economic and Social Measurement 5, 472-492.

> Rosenbaum, P. R. and D. B. Rubin. 1983. The Central Role of the Propensity Score in Observational Studies for Causal Effects. Biometrika. 70 (1): 41–55

*Stata command: heckman, psmatch2*

***Collinearity***

> Besley, D. A. 1991. Conditioning Diagnostics: Collinearity and Weak Data in Regression. New York: Wiley.

*Stata command: coldiag2*

## Panel


***Random vs Fixed Effect Models***

> Hausman, J. A. 1978. Specification Tests in Econometrics. Econometrica. 46 (6): 1251–1271

*Stata command: hausman*


***Correlation between Explanatory Variables and Individual Random Effects***

> Hausman, J. A., and W. E. Taylor. 1981. Panel data and unobservable individual effects. Econometrica 49: 1377-1398.

*Stata command: xthtaylor*

***Dynamic Panel Model***
> Arellano, M., and S. Bond. 1991. Some tests of specification for panel data: Monte Carlo evidence and an application to employment equations,  Review of Economic Studies 58: 277-297.
*Stata command: xtabond, xtabond2*

## Time-Series

***Unit-root Tests***

> Dickey, D. A. and W. A. Fuller. 1979. Distribution of the Estimators for Autoregressive Time Series with a Unit Root. Journal of the American Statistical Association. 74 (366): 427–431.

*Stata command: dfuller*

***Heteroskedasticity and Autocorrelation***

> Newey, W. K and K. D. West. 1987. A Simple, Positive Semi-definite, Heteroskedasticity and Autocorrelation Consistent Covariance Matrix. Econometrica. 55 (3): 703–708.

> Newey, W. K and K. D. West. 1994. Automatic lag selection in covariance matrix estimation. Review of Economic Studies. 61 (4): 631–654

*Stata command: newey*

***Panel Non-stationarity Tests***

> Levin, A., C.-F. Lin, and C.-S. J. Chu. 2002. Unit root tests in panel data: Asymptotic and finite-sample properties. Journal of Econometrics 108: 1–24.

*Stata command: xtunitroot*

***Panel Cointegration Tests***

> Pedroni, P. 1999. Critical Values for Cointegration Tests in Heterogeneous Panels with Multiple Regressors, Oxford Bulletin of Economics and Statistics, 61, 653-70.

> Pedroni, P. 2001. Purchasing Power Parity Tests in Cointegrated Panels, Review of Economics and Statistics, 83, 727-731

> Westerlund, J. 2007. Testing for error correction in panel data.  Oxford Bulletin of Economics and Statistics 69: 709-748.

*Stata command: xtwest, xtpedroni*

## Survival

***Parametric Survival Model***

> Kleinbaum, David G.; Klein, Mitchel. 2012, Survival analysis: A Self-learning text (Third ed.), Springer

*Stata command: streg*

***Cox Proportional Hazards Model***

> Cox, David R. 1972. Regression Models and Life-Tables. Journal of the Royal Statistical Society, Series B. 34 (2): 187–220.

*Stata Command : stcox*
