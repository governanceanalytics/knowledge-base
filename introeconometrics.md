# A Short Introduction of Econometrics

***What is Econometrics?***

Econometrics is a set of methods for estimating economic relationship. Recall that Economics is a discipline to explain and predict economic variables. Econometrics is thus a tool to help establish economists’ claims quantitatively. To explain and predict variables, the evidence needs to be more than correlation. Explanation implies causality. Establishing causality is however far from easy.

The fundamental difference of Economics (along with Econometrics) and Physical Sciences is that economists are unable to conduct controlled experiments (though economists are increasingly applying techniques developed by Psychology).  Economic data are nonexperimental and collected in uncontrolled environment. 

In a laboratory-controlled experiment, scientists can fix all other factors constant but adjust one of the variable and check how it affects the outcome. For example, two groups of mouse have been fed identical food, living in identical environment. One day the scientist gives an additional drug to one group (treatment group) but not the other (control group) and studies the impact for the subsequent days. By controlling all other factors, we are able to establish causality because any differences during the subsequent days are (almost) certainly due to the drug given to the treatment group. In our economy, it is by no means possible. Econometrics is thus developed along this important difference.

A lot of social scientists may have experience with multivariate regressions. If one can include all variables of the true data-generating process, we can in principle replicate the laboratory environment and establish claims of causality. However, a lot of relevant factors in Social Sciences are either unobservable, for example, preferences, or hardly be measured. Some appeal to survey data to overcome the problem but surveys are plagued with many other disadvantages. Sometimes the problem of missing some variables is due to our ignorance; we can never be sure that we have known the true model. As a result, Econometrics is developed to deal with the limitation of Statistics to study causality.

***Types of Data***

Before we start any econometric analysis, we should understand the data we have got. In general, we have three main types of variables and four main types of datasets.

**Variables**

*Numerical Variable*

This is the most common type of variables. They are usually continuous and the difference of two random values matter; the distance from 1 to 2 is different from that from 2 to 4. 

*Binary Variable*

It is either 0 or 1. I am either male or female. One either passes or fails the examination, and so on.

*Categorical Variable*

It is an integer, which refers to a defined meaning. For example, I have obtained a dataset of occupational choices of thousands of workers. The value “1” of the variable “Occupation” refers to “Accountant”, “2” “Butcher”, “3” “Clerk”, etc.

**Data**

*Cross-sectional Data*

Each observation is supposed to be independent; the value of one observation does not affect the value of another. They may be individuals, companies, cities, and countries. Oftentimes we can assume random sampling for a cross-sectional dataset.

*Time-series Data*

A time-series data measures an entity over time. For example, GDP is a time-series data since it measures the economic production at different points of the time. The main issue with time-series data is that two consecutive values are highly likely correlated. One may find an OLS estimator suffering from serial correlation.

*Panel Data*

If we have the information of many individuals over different points of time, we have obtained a panel data. The advantage of having panel data is that we could control for individual-specific and time-specific factors, allowing us to focus on other more interesting factors. One should be aware of the difference between short (N>T) and long (N<T) panel data.



