
# Creditworthiness Prediction & Explainable AI

## Advanced Predictive Modeling, SHAP Interpretability and Data-Driven Optimization for Financial Product Decisions

An advanced Machine Learning and Explainable AI project combining predictive classification, model optimization and SHAP-based interpretability to investigate creditworthiness, identify complex relationships among financial and demographic variables, and support evidence-based financial product decisions.

## Project Overview

The project develops an integrated analytical framework for predicting customer creditworthiness and interpreting the factors influencing classification outcomes.

Rather than focusing exclusively on predictive accuracy, the methodology combines **statistical analysis, supervised Machine Learning, model optimization and advanced Explainable AI** to investigate how individual variables and their interactions contribute to financial risk assessment.

The analysis addresses three interconnected objectives:

- **Predictive optimization:** improving classification performance through model comparison, class imbalance management and decision-threshold calibration.
- **Advanced interpretability:** using SHAP to investigate feature contributions, non-linear relationships, interaction effects and critical thresholds.
- **Decision intelligence:** translating model explanations into insights for input data optimization, customer segmentation, risk assessment and potential bias identification.

The framework is applied to a banking credit product case, with particular attention to balancing credit risk management and the identification of eligible customers.

## Analytical Framework

### 1. Predictive Modeling and Classification Optimization

The project develops and evaluates supervised classification models, including Logistic Regression and Decision Trees.

The methodology integrates:

- Statistical feature analysis and multicollinearity assessment.
- Feature engineering and numerical transformations.
- Cross-validation and comparative model evaluation.
- Class imbalance management through resampling techniques.
- Hyperparameter optimization.
- Probability-threshold calibration to manage classification trade-offs.

The optimized Decision Tree achieves a reported cross-validation accuracy of **95.27%**, improving upon the Logistic Regression baseline.

The final classification framework is evaluated through confusion matrices and class-specific precision, recall and F1 scores.

Particular attention is given to the different operational consequences of false positives and false negatives, allowing classification performance to be interpreted in relation to financial risk and product offering objectives.

### 2. Advanced Explainable AI with SHAP

A central contribution of the project is the integration of **SHAP (SHapley Additive exPlanations)** to move beyond predictive performance and investigate the underlying mechanisms of model decisions.

SHAP analysis is combined with statistical correlation methods to provide complementary perspectives on feature relevance.

While Pearson correlation identifies linear statistical relationships, SHAP evaluates how explanatory variables contribute to predictions within the trained model.

The analysis includes:

- Global feature importance and ranking of predictive drivers.
- Direction and magnitude of feature contributions.
- SHAP dependence plots.
- Non-linear feature-response relationships.
- Interaction effects between financial and demographic variables.
- Identification of critical feature thresholds.

This approach provides a deeper understanding of how the model combines information and produces differentiated creditworthiness assessments.

### 3. Non-Linear Relationships and Feature Interactions

The SHAP analysis identifies **annual income, customer age and employment duration** as the principal predictive drivers.

Their influence is not exclusively linear or independent.

The project investigates two particularly relevant interactions.

**Income and Age**

SHAP dependence analysis reveals a non-linear relationship between income and creditworthiness predictions, including a transition around a log-transformed income value of approximately 12.

The contribution of income also varies according to customer age, suggesting that the model evaluates financial capacity in combination with demographic characteristics.

**Income and Employment Duration**

A second interaction analysis demonstrates how employment stability modifies the predictive contribution of income.

At comparable income levels, longer employment histories tend to contribute more favorably to creditworthiness assessments.

These findings illustrate how SHAP can identify relationships that would not be fully captured by individual-variable correlation analysis.

### 4. Model Explainability and Input Data Optimization

The integration of statistical analysis and SHAP provides a methodological foundation for evaluating the relevance and quality of input variables.

The framework supports:

- Identification of influential and potentially redundant features.
- Investigation of complex relationships among explanatory variables.
- Assessment of the informational contribution of financial and demographic characteristics.
- Identification of candidate variables for refinement or enrichment.
- Evaluation of feature thresholds relevant to customer segmentation and credit assessment.

Explainability is therefore used not only to interpret model outputs but also to inform potential improvements to the underlying predictive framework.

### 5. Risk Management, Customer Segmentation and Model Bias

The project examines how predictive outputs and SHAP explanations can support financial product decisions.

**Risk Management**

Classification thresholds and performance metrics are evaluated in relation to the consequences of incorrect creditworthiness assessments.

**Customer Segmentation**

Feature importance, non-linear effects and interactions provide analytical evidence for identifying differentiated customer profiles and potential product offering opportunities.

**Algorithmic Bias**

SHAP analysis also highlights potential systematic disadvantages affecting younger customers or individuals with less continuous employment histories.

These observations motivate further investigation into historical data representativeness, feature selection and potential indirect discrimination.

The analysis emphasizes that predictive accuracy alone is insufficient to establish the suitability of a model for financial decision-making.

## Key Findings

The project demonstrates the value of combining predictive modeling with advanced explainability.

**Predictive Performance**

Model optimization improves classification performance, while class balancing and threshold calibration provide mechanisms for managing different risk priorities.

**Multidimensional Interpretability**

SHAP reveals how financial and demographic variables interact within the predictive model, identifying effects that extend beyond simple statistical correlations.

**Non-Linear Financial Relationships**

Income, age and employment duration exhibit meaningful interaction effects and non-linear contributions to creditworthiness predictions.

**Input Data Optimization**

Model explanations provide evidence for reviewing feature relevance, identifying opportunities for data enrichment and improving the analytical framework.

**Responsible Financial AI**

The investigation of potential bias highlights the importance of transparency, interpretability and critical evaluation when applying Machine Learning to financial products.

## Technologies and Methodologies

**Programming and Data Analysis**

Python · Pandas · NumPy · SciPy

**Machine Learning**

Scikit-learn · Logistic Regression · Decision Tree Classification · Cross-Validation · Hyperparameter Optimization · Imbalanced-learn

**Explainable AI**

SHAP · Feature Importance · SHAP Dependence Plots · Feature Interaction Analysis

**Statistical and Visual Analysis**

Pearson Correlation · Chi-Square Testing · Matplotlib · Seaborn

**Development Environment**

Google Colab · Jupyter Notebook

## Project Files

- [Predictive_Model_for_Supporting_Credit_Product.ipynb](Predictive_Model_for_Supporting_Credit_Product.ipynb) — Complete analytical notebook, including statistical analysis, predictive modeling, classification optimization and advanced SHAP interpretability.

### Dataset

The project uses an externally hosted credit scoring dataset:

https://proai-datasets.s3.eu-west-3.amazonaws.com/credit_scoring.csv

The dataset is retrieved programmatically from Amazon S3, avoiding the need to include the original CSV in the GitHub repository.

## Methodology

The project follows an integrated analytical workflow:

**Financial Data → Statistical Feature Analysis → Predictive Modeling → Model Optimization → SHAP Explainability → Non-Linear and Interaction Analysis → Input Data Optimization Insights → Financial Decision Support.**

The distinctive methodological contribution is the combination of predictive classification and advanced model interpretation, transforming Machine Learning outputs into a structured understanding of financial risk drivers and their interactions.

## Project Scope

Independent Machine Learning and Explainable AI project focused on creditworthiness prediction and advanced model interpretability in a banking credit product context.

The project demonstrates how statistical analysis, predictive optimization and SHAP-based explanations can be integrated to support more transparent, analytically grounded financial decisions.

The results are experimental and do not constitute a production-ready credit approval system.
