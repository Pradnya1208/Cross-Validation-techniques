<div align="center">
  
[1]: https://github.com/Pradnya1208
[2]: https://www.linkedin.com/in/pradnya-patil-b049161ba/
[3]: https://public.tableau.com/app/profile/pradnya.patil3254#!/
[4]: https://twitter.com/Pradnya1208


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]
[![tableau](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/e257c5d6cf02f13072429935b0828525c601414f/icons/icons8-tableau-software%20(1).svg)][3]
[![twitter](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c9f9c5dc4e24eff0143b3056708d24650cbccdde/icons/iconmonstr-twitter-5.svg)][4]

</div>

# <div align="center">Cross validation Techniques</div>
<div align="center"><img src="https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/output/intro.gif?raw=true"></div>


## Overview:
One of the commonly encountered problems in software engineering is that our data sets are usually of limited size, i.e., a few hundred observations when we are lucky. Dividing the available data into a modeling set and a test set is usually difficult as it implies that either the test set is going to be too small to obtain representative and reliable results or the modeling set is going to be too small to build a refined predictive model. One reasonable compromise is to use a cross-validation procedure. To get an impression of how well the model performs when applied to different data sets, i.e., its prediction accuracy, a cross-validation should be carried out.

Depending on the availability and size of the data set, various cross-validation techniques can be used:
- K-fold Cross-Validation
- Stratified K-fold Cross-Validation
- Holdout method
- Leave-p-out Cross-Validation
- Leave-one-out Cross-Validation
- Monte carlo Cross-Validation## K-fold Cross-Validation:
Cross-validation is a resampling procedure used to evaluate machine learning models on a limited data sample.

The procedure has a single parameter called k that refers to the number of groups that a given data sample is to be split into. As such, the procedure is often called k-fold cross-validation. When a specific value for k is chosen, it may be used in place of k in the reference to the model, such as k=10 becoming 10-fold cross-validation.
<br>

<img src="https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/output/kfold.PNG?raw=true" width="80%">
<br>

Checkout the [K-fold](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/K-Fold%20Cross%20validation.ipynb) implementation.

## Stratified K-fold Cross-Validation:
Stratification seeks to ensure that each fold is representative of all strata of the data. Generally this is done in a supervised way for classification and aims to ensure each class is (approximately) equally represented across each test fold (which are of course combined in a complementary way to form training folds).
<br>

<img src="https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/output/stratified.png?raw=true" width="80%">
<br>

Checkout the [Notebook](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/%20Stratified%20K-Fold%20Cross-Validation.ipynb) for more details.

## Holdout Method:
The holdout method is the simplest kind of cross validation. The data set is separated into two sets, called the training set and the testing set. The function approximator fits a function using the training set only. Then the function approximator is asked to predict the output values for the data in the testing set (it has never seen these output values before). The errors it makes are accumulated as before to give the mean absolute test set error, which is used to evaluate the model. The advantage of this method is that it is usually preferable to the residual method and takes no longer to compute. However, its evaluation can have a high variance. The evaluation may depend heavily on which data points end up in the training set and which end up in the test set, and thus the evaluation may be significantly different depending on how the division is made.
<br>

<img src="https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/output/holdout.PNG?raw=true" width="60%">
<br>

Check the implementation [here](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/Hold%20Out%20Cross%20Validation.ipynb)

## Leave-p-out Cross-Validation:

Another type of cross-validation is the Leave-p-out cross-validation method. Herein, the data sample comprises data points (n). The total number of data points (n) is used to separate a set of data points that is used for testing. 
These data points are referred to as (p). The training data set is obtained by calculating (n-p) and the model is trained accordingly. Once the training is done, p data points are used for cross-validation. 

Check the code [here](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/Leave%20P%20Out%20cross-validation.ipynb)

## Leave-one-out Cross-Validation:
The Leave-One-Out Cross-Validation, or LOOCV, procedure is used to estimate the performance of machine learning algorithms when they are used to make predictions on data not used to train the model.

It is a computationally expensive procedure to perform, although it results in a reliable and unbiased estimate of model performance. Although simple to use and no configuration to specify, there are times when the procedure should not be used, such as when you have a very large dataset or a computationally expensive model to evaluate.
<br>

<img src="https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/output/loocv.gif?raw=true" width="60%">
<br>

checkout the implementation [here](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/Leave%20One%20Out%20cross-validation.ipynb)

## Monte carlo Cross-Validation:
Monte Carlo cross-validation,creates multiple random splits of the dataset into training and validation data. For each such split, the model is fit to the training data, and predictive accuracy is assessed using the validation data. The results are then averaged over the splits. The advantage of this method (over k-fold cross validation) is that the proportion of the training/validation split is not dependent on the number of iterations (i.e., the number of partitions). The disadvantage of this method is that some observations may never be selected in the validation subsample, whereas others may be selected more than once. In other words, validation subsets may overlap. This method also exhibits Monte Carlo variation, meaning that the results will vary if the analysis is repeated with different random splits.

<br>

Checkout the implementation [here](https://github.com/Pradnya1208/Cross-Validation-techniques/blob/main/Monte%20Carlo%20Cross-Validation(Shuffle%20Split).ipynb).



## Implementation:

**Libraries:**  `NumPy`  `pandas` `sklearn`  `Matplotlib`


### Learnings:
`Cross validation Techniques`






## References:
[Cross validation techniques](https://www.sciencedirect.com/topics/engineering/cross-validation-technique)
<br>
[Cross Validation](https://www.wikiwand.com/en/Cross-validation_(statistics))

### Feedback

If you have any feedback, please reach out at pradnyapatil671@gmail.com


### 🚀 About Me
#### Hi, I'm Pradnya! 👋
I am an AI Enthusiast and  Data science & ML practitioner




[1]: https://github.com/Pradnya1208
[2]: https://www.linkedin.com/in/pradnya-patil-b049161ba/
[3]: https://public.tableau.com/app/profile/pradnya.patil3254#!/
[4]: https://twitter.com/Pradnya1208


[![github](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c292abd3f9cc647a7edc0061193f1523e9c05e1f/icons/git.svg)][1]
[![linkedin](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/9f5c4a255972275ced549ea6e34ef35019166944/icons/iconmonstr-linkedin-5.svg)][2]
[![tableau](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/e257c5d6cf02f13072429935b0828525c601414f/icons/icons8-tableau-software%20(1).svg)][3]
[![twitter](https://raw.githubusercontent.com/Pradnya1208/Telecom-Customer-Churn-prediction/c9f9c5dc4e24eff0143b3056708d24650cbccdde/icons/iconmonstr-twitter-5.svg)][4]



