In this exercise we provide in R code elements of the analysis on treatment effect of income on 
religiousness (Busser 2015). Busser (2015) use a fuzzy regression discontinuity design on a representative
dataset of 2645 households from Ecuador, to research effects of income on religion. 

In addition to the theoretical
analysis we implement in this exercise several elements reproducible research and good analysis:

1. Use of one environment for both analysis and report writing. Code and comments are written in .rnw file and 
	knitr package is employed.
2. Use of user-definied functions for the production of plots when reproducing the same plot with diffrent bin size.
3. Use of formula objects to reproduce the same analysis by adding and dropping covariates, or for different fucntional 
	forms of the score variable.
4. Use of package stargazer to produce publication quality tables. This is a recent package added to R
	packages.

In terms of analysis we show:
1. Both treatment (D) and outcome (Y) variable pass the visual inspection test of conditional mean discontinuity
	at the at the cutoff point of the score variable (S); E(Y|S), E(D|S) discontinuous at cutoff
2. Treatment effect of income on religiousness 
	(a) controling for covariates
	(b) employing different bandwidths
	(c) employing up to 3rd order polynomial of the score variable
3. Covariates pass the regression test of no-break at cutoff point