# grid-search-and-cross-validation
Train a Decision Tree for the moons dataset by below steps: make_moons function from sklearn library generates 2D binary classification datasets that are challenging to certain algorithms e.g. centroid-based clustering or linear classification, including optional Gaussian noise. Also, they are useful for visualization.

a) Use make_moons(n_samples=10000, noise=0.4) to generate a moons dataset. Plot the obtained dataset.

b) Use train_test_split() to split the dataset into a train and test sets. (test size = 0.2)

c) Explain how “grid search” works then use it with cross-validation to find good hyperparameter values for a Decision Tree classifier; Report best estimator. Also, you are allowed to use built-in functions in sklearn (Hint: try various values for max_leaf_nodes and max_depth)

d) Train it on the full training set using these hyperparameters, and measure your model’s performance on the test set. Report accuracy and confusion matrix.

e) Generate 1,000 subsets of the training set with make_moon which, each one is containing 100 instances selected randomly.

f) Train one Decision Tree on each subsets, using the best hyperparameter. Evaluate these 1,000 Decision Trees on the test set. (Hint: you can use sklearn.base.clone for this part.)
Since they were trained on smaller sets, these Decision Trees will likely perform worse than the first Decision Tree, achieving only about 80% accuracy.

g) For each test set instance, generate the predictions of the 1,000 Decision Trees, and keep only the most frequent prediction (you can use SciPy’s mode() function for this). This approach gives you majority-vote predictions over the test set. (These methods are same to ensemble approaches that will be considered in next assignment)

h) Evaluate these predictions on the test set and compare the accuracy of this model with the model in part d.
