# Machine Learning Homework - Exoplanet Exploration

## Background
Create machine learning models capable of classifying candidate exoplanets from the raw dataset.

### Models

### KNN
Summary: KNN point at 9 is the closet data point where the accuracy score is highest before it stablizes.
Assumptions: This assumes the data was on the scale, but in preprocessing the X values were scaled.
Predication: The data remains stable after the max knn range.
Improvement: The hypertuning did not significantly improve since the score was 0.824 and the original model test score was 0.828. Removing some columns from the X value may change this.

### Random Forest
Summary: The original model initial has a score of 0.899 which is yields a higher score than the knn model including all the variables.
Assumptions: Subsets may not consistently match the overall data.
Predication: The model did continue to improve with each new estimator, but in minimal amount. However, this model produced the highest hypertuning score.
Improvement: Rerun with the five feature importances over 0.50 which include koi_model_snr, koi_fpflag_ss, koi_fpflag_co, and koi_fpflag_nt. This model is the easiet to run for overall score to gauge data overall and focus on a subset of the information to run to fine tune the model.

### Logistic Regression
Summary: The initial score for the train data was 0.850 and the test data was 0.842 which is comparable. However, this includes substantial false positives.
Assumptions: Use all X values scaled.
Predication:The hypertuning did improve data by a higher percentange than the other models. Unclear which of the various X values influence the logs of the y values.
Improvement: Can easily train and update X values for optimal results.




