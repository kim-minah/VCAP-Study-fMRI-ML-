# VCAP Machine Learning Model Comparison & Evaluation

1. **Model Comparisons (`01_vcap_modelcomparisons.ipynb`)**
   - Loads preprocessed connectivity and behavioral/social variables.
   - Fits machine learning models (Ridge, Lasso, ElasticNet).
   - Optimizes hyperparameters via nested cross-validation.
   - Compares prediction metrics (R², MAE, RMSE, correlations) across targets.

2. **Empirical Nulls (`02_vcap_empiricalnull.ipynb`)**
   - Uses permutation testing to generate empirical null distributions.
   - Preserves optimized hyperparameters from model comparisons.
   - Produces null distributions for evaluating statistical significance of observed model performance.

3. **Evaluation (`03_evaluatemodel.ipynb`)**
   - Compares observed model performance to empirical null distributions.
   - Computes one-sided and two-sided p-values for each target.
   - Produces figures (e.g., violin plots) summarizing model vs. null comparisons.

