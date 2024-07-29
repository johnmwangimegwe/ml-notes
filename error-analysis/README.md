# Error Analysis Notes
[Click here](https://docs.google.com/presentation/d/1o3o_cNCqXzmupZ3zs7-ysfbpjzkFWIaUzGXhJg6WJNo/edit?usp=sharing) to see the slides for our Error Analysis workshop on Saturday, July 27, 2024

## Bias-Variance Analysis
All problems in machine learning are as a result of only two things:
1. **High Bias (Underfitting)** - Your model has not learned enough from the features present in the data
2. **High Variance (Overfitting)** – Your model has overlearned from the training set but generalised poorly on unseen data

We usually want our model to get as close as possible to the optimal error rate (if there is any). This could be:
- The expected human error for tasks that humans are already good at e.g.  Driving Cars, Image Recognition
- The previous generation of model though in such cases there is a high possibily of improving on the optimal error

We can diagnose this by exploring the errors on both the training set and testing set as follows:
- If there is a huge gap between the errors of the training and testing set i.e training error is extremely low but the testing error is high, this is a high bias instance. You model is performing well on training data but does not generalise well on unseen data.
- If there is no huge gap between the two errors but both errors are worse (higher) than the expected optimal error. Usually if you don't know the optimal error, if there's very little difference between the training and testing error, you want to try fix high bias and see if the error reduces without creating a new gap between the errors.

We can visualise bias-variance analysis through a learning curve as follows (Blue – training error, Green – testing error):

![Learning Curve](https://zahidhasan.github.io/images/learning_curve4.png)

$$ Model Error = (E_{test} - E_{train}) + (E_{train} - E_{opt}) + E_{opt} $$

$$ where; (E_{test} - E_{train}) = avoidablevariance $$

$$ and; (E_{train} - E_{opt}) = avoidablebias $$

To fix this model, we can run the following based on where we are fixing variance bias or variance:
- Data  (The best way to fix both variance and bias but acquiring data is costly and we need to optimise our accuracy as much as we can with the data already available)
- Feature Selection (Reduce feature by focusing on the important features)
- Engineer new features (Increasing features by creating and deducing new features)
- More epochs (For Neural Nets or Gradient Descent in case the model did not converge)
- Regularisation (Every model has a hyperparameter for regularisation)
- Try different models
- Try different cost function (Almost similar to trying a different model)
