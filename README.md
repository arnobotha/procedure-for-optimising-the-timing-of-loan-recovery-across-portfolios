# Simulation-based optimisation of the timing of loan recovery across different portfolios
[![DOI](https://zenodo.org/badge/275881943.svg)](https://zenodo.org/badge/latestdoi/275881943)

A novel procedure is presented for the objective comparison and evaluation of a bank's decision rules in optimising the timing of loan recovery. This procedure is based on finding a delinquency threshold at which the financial loss of a loan portfolio (or segment therein) is minimised. As an expert system, our method incorporates the time value of money, costs, and the fundamental trade-off between accumulating arrears versus forsaking future interest revenue. Moreover, the procedure can be used with different delinquency measures (other than payments in arrears), thereby allowing an indirect comparison of these measures. We demonstrate the procedure across a range of credit risk scenarios and portfolio compositions. The computational results show that threshold optima can exist across all reasonable values of both the payment probability (default risk) and the loss rate (loan collateral). In addition, the procedure reacts intuitively to nonstandard portfolios, including systemic defaults and portfolios with a significant degree of episodic delinquency (cycles of curing and re-defaulting). In optimising a portfolio's recovery decision, our procedure can better inform the quantitative aspects of a bank's collection policy than relying on arbitrary discretion alone.

## Structure
This R-codebase can be run sequentially using the file numbering itself as a structure. Delinquency measures are algorithmically defined in **DelinqM.R** as data-driven functions, which may be valuable to the practitioner outside of the study's current scope. Note that scripts 3.2, 3.3, and 6d are interactive scripts wherein the so-called Loss-based Recovery Optimisation across Delinquency (or LROD) procedure is repeatedly run by executing the script with different settings, as set out in the comments. Each independent run produces results that are saved for graphing later on (see the graph-varients of each numbered script where relevant).

## Data
This R-codebase creates designed portfolios as constrained by the testbed described in the main text and helpful commentary. Designed data are included as .RData files as well as generic files to ease replication, though these datasets can certainly be generated from scratch using the numbered scripts with prescribed parameter settings.

## Copyright
All code and scripts are hereby released under an [MIT](https://opensource.org/licenses/MIT) license. Similarly, all graphs produced by relevant scripts as well as those published here, are hereby released under a Creative Commons Attribution ([CC-BY 4.0](https://creativecommons.org/licenses/by/4.0/)) licence.
