# FAQs of Econometrics from a Practitioner's Point of View

***Important! Please refer to textbooks for more details! For example, Kennedy, Peter. 2008. A Guide to Econometrics, Sixth Edition.  Blackwell Publishing.***

## General and Cross-sectional Data
**1. The regression passes through Stata (or whatever statistical softwares) and produces significant results. It must be correct and I display the results in my paper.**

Answer:

It is a common mistake in academia. Softwares may help you detect some basic problems, for example, perfect collinearity, but it simply follows the orders given by humans. Human errors on specification of the model will certainly pass onto the regression results. Moreover, it is a very bad practice to believe that the result must be good because of its significance. A significant result may be a wrong result, and sometimes very likely. It is not uncommon to hear inexperienced practitioners defending their results by the "stars" attached to the estimates. 

**2. Given a linear regression model, is it true that OLS must work when I have obtained a big dataset?**

*Answer:*

No. Sometimes the data may be truncated at some value. For count variables, sometimes negative binomial regression is more suitable. In general OLS performs well (generates consistent estimates) since the chance of having a normally distributed error term is getting bigger as the size of the sample increases. 

**3. Is it true that I can always establish causality when I have obtained a big dataset?**

*Answer:*

No. Endogeneity bias comes from the fact that a relevant variable is missing, or that measurement error exists. One can only claim for causality from OLS if the estimation keeps all other factors constant. A big data may help because one can now include more control variables into the model. However, it does not solve the problem that some variables are in principle unobservable. For example, one may be able to collect all physical characteristics of patients in order to establish causality between characteristics and incidence of illnesses. It is still not sufficient because habits and preferences are still unaccounted for. Darker skins may be correlated with skin cancer but it could be due to the habit of sun bathing of some patients. It is not correct to say that darker skin leads to a higher probability of having skin cancer.

**4.	How can I establish causality between two variables?**

*Answer:*

First, statistics is built upon the principle to reject a hypothesis, but not to confirm it. We can never be sure a causality is confirmed and proved. We are waiting for new data or new estimation techniques to reject existing hypotheses. In Econometrics, we have some techniques for us to better understand potential causality. Two-stage least squared (2SLS) or Instrumental variable estimation is one of those. The first step is to explain the endogenous explanatory variable by at least one exogenous variable, which theoretically does not explain the dependent variable of interest. The second step is to include the predicted values of the first step to replace the endogenous variable in the model to explain the dependent variable of interest. The idea of the first step is that it keeps only the part of the variation of the endogenous variable which are explained by the exogenous variable to be included in the model so that the error terms are randomly distributed.

**5.	I suspect that the sample is not randomly selected. What can I do?**

*Answer:*

A lot of sample is obviously not randomly selected. For example, we can only observe the wage of those who participate in the labour force. Simply using the information on wage of those who participate may produce biased estimates of the parameters. If the selection is exogenously determined, i.e. the selection is due to a factor that does not explain wage, OLS is still consistent. With a stronger assumption OLS is even unbiased. 

However, if the selection is believed to be endogenous, the Heckman 2-step estimation may correct the bias. First step: using all available instruments (Z) to explain the endogenous binary choice: To work as a computer scientist or not by a Probit Model (Propensity score) Second step: The predicted values of the first-step are then used to compute the inverse Mills ratio, which is then put into the second step as an additional explanatory variable to explain the dependent variable (income or promotion) along with a subset of the instruments (X is a subset of Z). (Stata command: rheckman) Two important notes: To do the Heckman 2-step estimation, we need at least one additional variable, which is not included in the second step. The additional variable should be correctly excluded in the second step, i.e. it is not (theoretically) an explanatory variable in the true data-generating process

## Time-series Data

**1.Why does non-stationarity matter?**

*Answer*

Non-stationarity will violate the assumption that the error terms are normally distributed. A usual step is to include lags and/or leads into the model to capture serial correlation.

**2.	What can be done to improve out-of-sample prediction?**

*Answer*

One may conduct a in-sample prediction to check if the model produces satisfactory results. First you apply your model and estimate the coefficients with a subset of your sample, for example the first 90% of the periods available. Then you do an out-of-sample prediction for the next 10% of the periods to see if the prediction is close enough to the actual data. By doing this, you may identify missing elements of your model and improve the predictive power of your model.

## Panel Data

**1.	Random-effect vs Fixed-effect model: which one should I choose?**

*Answer:*

One may do a Hausman test to see if one or the other should be chosen. However, it may not be sufficient. One may display both models side by side for comparison. Only God knows the truth! In general, if the number of groups is not very large compared with the number of total observations, a fixed-effect model is more convincing since we do not expect the error terms to be randomly distributed in that case. Keep in mind that the Hausman test is only valid if strict-exogeneity assumption holds. 

**2.	Is it true that techniques developed for short-panel (the number of groups is larger than the number of periods) can also be used for long-panel study?**

*Answer:*

No. One should check technique by technique. Most of them are based on the assumption that N>T. Recently a lot more tools have been developed for the long forgotten long-panel dataset. One major difference is that for long-panal data one may have to deal with issues of non-stationarity of variables.
