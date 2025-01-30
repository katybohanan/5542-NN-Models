# 5542-NN-Models

1. Results of Diabetes Dataset:
   This task starts by installing the required libraries: torch, torchvision, scikit-learn, and matplotlib. After importing the necessary libraries and setting device for GPU acceleration, the Diabetes (https://www.kaggle.com/datasets/mathchi/diabetes-data-set) dataset is loaded. Next the y-value, or target, is converted to binary for the classification task. This is done by using the median as a threshold--patients are labeled 1 or 0 based on if they fall above or below the threshold. The data is split using 80% of the dataset for training and 20% for testing (standard). The data is also standardized using StandardScaler.
   The model being used for the regression and classification tasks is a Feedforward neural network. The loss function used for regression is Mean Square Error (MSE)--this tells the model to use MSE to measure how well its predictions match the actual target values during training. The loss function used for classification is Binary Cross-Entropy--this calulates the difference between the predicted probability of a sample belonging to a class and the actual class label. It penalizes the model more for confident, incorrect predictions. Both classification and regression models use the Adam optimizer and a learning rate of 0.01. The models train for 100 epochs, logging the loss every 10 epochs.
   
   The final results of the regression model:
   * MSE: 2986.7795
   * R-Squared: 0.4397
     
    The final results of the classification model:
    * Accuracy: 0.7302
    * Precision: 0.6818
    * Recall: 0.75
    * f1 Score: 0.7143

3. Results of California Housing Dataset:
   This task, similar to above, starts by installing the required libraries: torch, torchvision, scikit-learn, and matplotlib. After importing the necessary libraries and setting device for GPU acceleration, the California Housing (https://www.kaggle.com/datasets/camnugent/california-housing-prices) dataset is loaded. Next the y-value, or target, is converted to binary for the classification task. This is done by using the median as a threshold--patients are labeled 1 or 0 based on if they fall above or below the threshold. The data is split using 80% of the dataset for training and 20% for testing (standard). The data is also standardized using StandardScaler.
   The model being used for the regression and classification tasks is a Feedforward neural network. The loss function used for regression is Mean Square Error (MSE). The loss function used for classification is Binary Cross-Entropy. Both classification and regression models use the Adam optimizer and a learning rate of 0.01. The models train for 100 epochs, logging the loss every 10 epochs.

   The final results of the regression model:
   * MSE: 0.3103
   * R-Squared: 0.7632
     
    The final results of the classification model:
    * Accuracy: 0.8774
    * Precision: 0.8845
    * Recall: 0.8664
    * f1 Score: 0.8754
