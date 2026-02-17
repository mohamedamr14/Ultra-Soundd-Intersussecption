Bayesian Meta-Analysis of Ultrasound Accuracy in Pediatric Intussusception
Overview

This repository contains the analytical work supporting our systematic review and Bayesian meta-analysis evaluating the diagnostic accuracy of ultrasound for pediatric intussusception in emergency settings.

This project synthesizes evidence from 44 studies (n = 4,142 patients) and applies hierarchical Bayesian modelling to estimate pooled sensitivity, specificity, predictive values, and sources of heterogeneity.

My Contribution (Co-Author)

As a co-author, I was primarily responsible for:

Conducting Bayesian bivariate meta-analysis of diagnostic accuracy

Implementing hierarchical summary ROC (HSROC) modelling

Performing robustness analyses using alternative prior specifications (H-Cauchy and Penalized Complexity priors)

Estimating pooled prevalence using random-effects GLMM

Deriving predictive values across varying prevalence bands

Conducting subgroup analyses (symptoms, demographics, operator specialty)

Assessing heterogeneity and between-study variance

Evaluating publication bias and contributing to GRADE certainty assessment

Drafting and interpreting all statistical results sections

Methods Summary
Diagnostic Accuracy Modelling

Bayesian bivariate models implemented using meta4diag

Weakly informative H-Cauchy priors

Penalized Complexity (PC) priors for sensitivity analysis

Estimation of pooled sensitivity, specificity, correlation structure

HSROC curve construction

Prevalence Estimation

Random-effects Generalized Linear Mixed Model (GLMM)

Logit transformation with back-transformation to probability scale

Heterogeneity quantified using τ² and I²

Prediction intervals calculated

Predictive Values

Positive Predictive Value (PPV) and Negative Predictive Value (NPV)

Derived across observed prevalence bands

Fagan nomogram generated for clinical interpretation

Subgroup Analyses

Bayesian bivariate models with covariates

Assessment of symptom-level and demographic effects

Operator specialty comparison

Evaluation of variance components and sensitivity-specificity correlation

Key Findings

Pooled Sensitivity: ~96%

Pooled Specificity: ~96%

AUC: ~0.81–0.82 (good diagnostic performance)

Predictive values strongly dependent on baseline prevalence

High reproducibility of sensitivity across studies

No conclusive evidence of performance differences by symptoms, age, sex, or operator background

High certainty of evidence for pooled diagnostic accuracy

Software & Tools

R

meta4diag

GLMM (random-effects modelling)

Bayesian hierarchical modelling framework

Reproducibility

All models were implemented using reproducible R scripts with clearly documented prior specifications and analytical steps. Sensitivity analyses were conducted to confirm robustness of pooled estimates under alternative prior assumptions.

Clinical Relevance

This analysis demonstrates that ultrasound is a highly accurate, rapid, and non-invasive diagnostic tool for pediatric intussusception, with performance remaining stable across most clinical and demographic contexts. Predictive values vary by baseline prevalence, reinforcing the importance of contextual interpretation in emergency settings.
