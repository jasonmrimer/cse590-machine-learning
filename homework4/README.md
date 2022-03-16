# Objectives
1. Apply Kernel SVM and MLP classification algorithms to the fashion-MNIST dataset
2. Use k-fold cross validation to identify the best way to rescale and preprocess the data
3. Use k-fold cross validation to identify the parameters that optimize performance
(generalization) for each method
4. Compare the accuracy and identify correlation between the outputs of the two methods


# Problem
For this homework, you will apply the following classification methods to the fashion-MNIST
classification data
1. Kernel Support Vector Machines
2. Multilayer Perceptrons

- Apply 4-fold cross-validation to the provided training data subset to train your classifiers and
identify their optimal parameters. In addition to the classifier’s parameters (e.g. regularization,
kernel, Number of layers/nodes, learning rate, etc.), you should also consider the following 4 ways
to preprocess and rescale the data:
  - No preprocessing
  - StandardScaler
  - RobustScaler 
  - MinMaxScaler

- After fixing the classifiers’ parameters, apply each method to the provided testing data subset to
predict and analyze your results. Compare the accuracy obtained during training (average of the
cross-validation folds) to those of the test data and comment on the results (overfitting,
underfitting, etc.)

- Analyze the correlation between the output of the 2 classifiers by displaying the predict_proba of
SVM vs. predict_proba of MLP (using test data). Using these scatter plots (one per class), identify
(if available) the following 3 groups 
  - G-1: Samples that are easy to classify correctly by the SVM, but hard to classify by MLP 
  - G-2: Samples that are easy to classify correctly by the MLP, but hard to classify by SVM 
  - G-3: Samples that are hard to classify correctly by both methods
  
  For each group, display few samples (as images) and identify any common features among them.
