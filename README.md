# NAML-HW1
Using the UCI Abalone data set to analyze trends predicting age.

1. Regression: For this problem use the data in the UCI data set Abalone (Abalone -
UCI Machine Learning Repository) to do some linear regression analysis. The
dataset contains 4177 instances of 8 features and a target. However, let’s take 500
samples as the training set and 100 samples as the test set (pick them spread over
the data set, say every fifth entry for the training set starting at 1, and every seventh
entry for the test set starting at 3000. The goal is to find a linear regression that
predicts the age (number of rings) using a regression on features 1 – 7. For the
categorical variable (sex), choose a surrogate integer, e.g. M = 1, F = 2, I =3. Use the
training set to find the regression weights and then use the test set to determine a
RMSE (see definition in the text equation 5.24). Print out the regression coefficients
(weights) from the training set analysis and the RMSE for the test set. Note: I think
the units in the descriptive material are incorrect but this is just a matter of scaling.
For your model, y is the number of rings (target) and the features x1 through x8 are
the features. You should have 9 weights w0 through w8. I have uploaded the dataset,
Abalone, as a .csv file into Canvas but do go to the site above for a thorough
description of the dataset.

2. Perceptron: For this problem, you will need to create a separable 2D dataset (x,y).
Create the dataset as follows: on a 1x1 grid, generate 20 random data points. Then
label each point by setting the label according to f(xi)= sign(yi-(.25+.5*xi)). (This will
create a separable dataset with the target function, f, we are going to try to find
using the Perceptron Learning Algorithm). Plot the dataset using the symbols + or –
according to the label. Start the algorithm with w0 and w1 both set to .1. Run the
Perceptron Learning Algorithm until there are no errors. Then repeat the plot with
your estimated separation line, i.e. place a line using the final weights, w0 + w1*x, on
the plot. Report the number of updates that the algorithm makes before it
converges. Now generate a test set of 100 points using f as above. With the final
weights, Count the number of prediction errors made by passing through the 100
test points (No weight updates, just count the number of errors and report the
accuracy of the Perceptron determined function).

3. Support Vector Classification: For this problem, you will be looking at a classic ML
dataset from the UCI repository, Iris (Iris - UCI Machine Learning Repository). For
this exercise, use the SVC method from sklearn. If you look at the web page in the
link, you will see at about the middle of the page that there is an estimate of SVC
performance in the range of 86.8 – 100% accuracy. If you focus on just the Iris-
setosa versus the other 2, you should be able to get close to 100% accuracy. Try to
separate the other varieties that won’t separate using the soft margin SVC to
measure the performance for Iris versacolor versus the other two, and then try
separate the Iris virginica. Measure the performance of each. This will be a lead in to
the multi-class classification that we will start in Chapter 7. In the non-separable
cases, experiment with a few values of C to see how the accuracy varies with this
hyperparameter selection (try C= .1, 1, and 10 and then try an intermediate value or
two). Again, I have uploaded the dataset, Iris, as a .csv file into Canvas but do go to
the site above for a thorough description of the dataset.
