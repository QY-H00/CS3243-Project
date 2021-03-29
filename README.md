# CS3243-Project

## Working steps:

### Initialize dataset:
1. Suppose the size of the dataset is m, the number of features is n.
2. As the dataset is the txt file where each line is a sample, it means that one txt file has m lines of (n + 1) numbers.
3. As API of sklearn accepts X (size: [n_samples, n_features]) and Y (size: [n_samples], int) as parameters.
4. So we read each dataset as following:
      ```
      import numpy as np
      from sklearn.model_selection import train_test_split
      
      set = np.loadtxt('datasets/20951.txt', delimiter=',')
      X = set[:, :-1]
      y = set[:, -1]
      X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2, random_state = 0)
      ```
### Evaluate Performance measure:
```
```
