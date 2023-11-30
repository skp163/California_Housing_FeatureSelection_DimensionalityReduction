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
            Used linear regression for predicting price of the houses in California. In this method
            I have considered all the available features in the model.
            Result:

            |R2_Error |  MSE   |
            |---------|--------|
            | 0.62909 | 0.49887|

        - Correlation Method:
        
            ![Features Correlation](https://github.com/skp163/California_Housing_FeatureSelection_DimensionalityReduction/blob/main/Assets/Correlation_Matrix1.png)
        
            Used Pearson’s Correlation to check how independent varibles are correlated with each other.
            If 2 or more independent features are highly correlated then they can be considered
            as duplicate features and can be dropped. Hence in this case I find 'AveBedrms' and 'AveRooms'
            is highly correlated from the Correlation Matrix. We need to drop one of the. Hence I am
            dropping 'AveRooms'. And I observed little improvement in my r2_error score.

            Our new reslut is:
            |R2_Error |  MSE   |
            |---------|--------|
            | 0.58185 | 0.55992|
