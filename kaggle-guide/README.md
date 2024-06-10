## Use `train.csv` as your core dataset
1. Use this data for training and model evaluation
2. Run your train-test splits or cross-validation on this dataset
3. Note that the id column is mostly there for identifying a unique observation and is not necessarily relevant to your model. Note that after predicting the test cases, you'll be required to submit an end submission including the id of the observation and your predicted `y`
4. Note that your `test.csv` does not include the target variable and therefore cannot help you in modeling. Use this only for generating your final predictions for Kaggle submission.
5. For unclean data, the steps you take on the `train.csv` should be the same you take on `test.csv` before you make the prediction.