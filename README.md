# BankNote_Authentication_Using_KNN
Whenever you go to the bank to deposit some cash money, the cashier places banknotes in a machine that tells whether a banknote is real or not. This is a classification problem where we are given some input data and we have to classify the input into one of the several predefined categories. Rule-based as well as statistical techniques are commonly used for solving classification problems. Machine learning algorithms fall in the category of statistical techniques
![image](https://user-images.githubusercontent.com/85330521/210282293-3faede62-2782-4709-acb7-959aaf7f9f50.png)

# Authenticating whether a banknote is real or not is one of the most common tasks in the banking industry.
In this article, we explain the process of building a banknote authentication system using machine learning algorithms. After reading this article, you will be able to understand how classification systems are built using machine learning algorithms.

# BankNote Dataset Description
We will be working with the “Banknote” standard binary classification dataset.

The banknote dataset involves predicting whether a given banknote is authentic given a number of measures taken from a photograph.

The dataset contains 1,372 rows with 5 numeric variables. It is a classification problem with two classes (binary classification).

Below provides a list of the five variables in the dataset.

    •   variance of Wavelet Transformed image (continuous).

    •   skewness of Wavelet Transformed image (continuous).

    •   kurtosis of Wavelet Transformed image (continuous).

    •   entropy of image (continuous).

    •   class (integer).
![image](https://user-images.githubusercontent.com/85330521/210282645-cddf3277-ab69-4a74-a994-57796056ba40.png)

A histogram plot is then created for each variable.

We can see that perhaps the first two variables have a Gaussian-like distribution and the next two input variables may have a skewed Gaussian distribution or an exponential distribution.
![image](https://user-images.githubusercontent.com/85330521/210282769-95d6a733-53b0-4456-8838-78e8ecee788c.png)


# Process of building a banknote authentication system
Use the Banknote Authentication data to implement your own simple KNN
classifier using python, (Don’t use any built-in functions), divide your data into
70% for training and 30% for testing.

    1.  If there is a tie in the class predicted by the k -nearest neighbors, then among the classes that have the same number 
        of votes, the tie should be broken in favor of the class that comes first in the Train file.
        
    2.  Each feature column should be normalized separately from all other features. Specifically, for both training and test objects,
        each feature should be transformed using the function: f(v) = (v - mean) / std, using the mean and std of the values of that
        feature column on the WHOLE data.
    
    3.  Use Euclidean distance to compute distances between instances.
    
    4.  Experiment with different values of k=1,2,3....9 and output the following:
    
         a. The value of k used for the test set on the first line followed by summary info for the current k value: 
            
              1) Number of correctly classified test instances.
            
              2) The total number of instances in the test set and accuracy.
