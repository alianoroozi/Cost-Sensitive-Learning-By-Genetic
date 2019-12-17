# Genetic algorithm based approach for cost sensitive learning

In this notebook, I implement a **genetic algorithm based approach for cost sensitive learning**, in which the misclassification cost is considered together with the cost of feature extraction. 

The decision tree classifier of Sklearn is chosen as the classification algorithm. You can choose any algorithm that you want.

A bit string representation is used to indicate what features are selected. For example, the bit string 101001 indicates that the 1st, 3rd, and 6th features are selected and the remaining ones are not.

The fitness function considers both the misclassification cost and the cost of extracting the selected features.

The [Thyroid Disease Data Set](https://archive.ics.uci.edu/ml/datasets/Thyroid+Disease) is used for the experiments: 
* ann-train.data contains train data,
* ann-test.data contains test data,
* ann-thyroid.cost contains the costs of using each feature. It does not include the cost of the 21st feature, because it is a combination of the other features.

