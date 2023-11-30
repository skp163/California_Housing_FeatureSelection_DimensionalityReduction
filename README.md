# California_Housing_FeatureSelection_DimensionalityReduction

<img src="https://github.com/skp163/California_Housing_FeatureSelection_DimensionalityReduction/blob/main/Assets/Feature%20Selection%20%26%20Dimensionality%20Reduction%20(1).gif" width="800" height="300" />

## Overview
I am using different methods of feature selection and dimensionality reduction on California housing dataset to achive most optimized result. 

### Data Set: <br/>
[sklearn.datasets.fetch_california_housing](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.fetch_california_housing.html)

***Number of Features : 8*** <br/>
***Sample size: 20640***

### Methods Used:
1. Filterbased Method
    - Using all Features Method
    - Correlation Method
    - Wrapper Based Methods
2. Mutual Information Method
3. PCA


### 1. Filterbased Method

<img src="https://github.com/skp163/California_Housing_FeatureSelection_DimensionalityReduction/blob/main/Assets/Filter_1.png" width="600" height="70" />

        - Using all Features Method:
            Used linear regression for predicting price of the houses in California. In this method< I have considered all the available features in the model.
            Result:

            |R2_Error |  MSE   |
            |---------|--------|
            | 0.62909 | 0.49887|

        - Correlation Method:
            Used 
