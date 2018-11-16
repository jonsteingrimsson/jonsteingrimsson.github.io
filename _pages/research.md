---
layout: single
title: "Research"
permalink: /research/
author_profile: true
---

### Risk prediction models with time-to-event data:  

Estimating a patient’s mortality risk is important in making treatment decisions. When some observations are censored, the statistic used to make splitting decisions in the standard classification and regression tree algorithm cannot be calculated. The paper “Doubly robust survival trees” uses semi-parametric efficiency theory for missing data to appropriately account for censored observations. Regression trees can suffer from instability and the random forest procedure. The paper “Censoring unbiased regression trees and ensembles” provides extensions to the random forest algorithm and more general form of splitting statistics.  

<!--
<img align="right" src="doc/subpagelist.png">
-->

A case-cohort study is a cost efficient two-phase sampling design which collects full covariate information only on a subset of the observations. For censored linear regression previous estimator for analyzing data arising from a case-cohort study fail to fully utilize observations with missing covariate data. In “Estimation in the Semiparametric Accelerated Failure Time Model With Missing Covariates: Improving Efficiency Through Augmentation” we develop estimation procedures that more efficiently use the available data.

### Adaptive Enrichment designs:  

Adaptive enrichment designs involve a preplanned rule for modifying enrollment based on accruing data in an ongoing trial. Such designs can provide stronger conclusions compared to more traditional single stage designs when a sub-population is expected to have enhanced treatment effect. Implementation of adaptive designs relies on specification of multiple designs parameters. There is little to no guidance on how to select them. We develop a optimization approach to selecting the design parameters which searches among all possible enrichment designs for a design minimizing expected sample size over some user specified scenarios. These scenarios allow the user to tailor the adaptive enrichment design to the scientific goals and logistical constraints of the trial.

The optimization procedure is implemented using a free software with a user friendly graphical user interface available at <http://rosenblum.jhu.edu/>. The current implementation allows for binary, continuous, and time-to-event outcomes potentially measured with delay, and both superiority and non-inferiority trials. The output is a reproducible report comparing the performance of optimized adaptive enrichment designs to single stage trials.

The paper “Optimized Adaptive Enrichment Designs for Multi-Arm Trials: Learning which Subpopulations Benefit from Different Treatments” which develops a design comparing two treatments to a common control and “Comparison of Adaptive Randomized Trial Designs for Time-to-Event Outcomes that Expand Versus Restrict Enrollment Criteria, to Test Non-Inferiority” which develops an adaptive enrichment design for a non-inferiority trial with time-to-event outcomes.

### Covariate adjustments for clinical trials:  

In randomized clinical trials with baseline variables that are prognostic for the primary outcome, there is potential to improve precision and reduce sample size by appropriately adjusting for these variables. A major challenge is that there are multiple statistical methods to adjust for baseline variables, but little guidance on which is best to use in a given context.

The paper “Improving precision by adjusting for prognostic baseline variables in randomized trials with binary outcomes, without regression model assumptions” describes properties of three estimators for the primary analysis of clinical trials with binary outcomes. The paper Matching the Efficiency Gains of the Logistic Regression Estimator while Avoiding its Interpretability Problems, in Randomized Trials derives asymptotic properties of comparing the three estimators. The main results is that we provide an estimator which has the same relative efficiency as a logistic regression estimator without requiring any model assumptions.