# Titanic Survival Prediction
 Titanic Survival Prediction Task
 
 Dataset: https://www.kaggle.com/c/titanic/overview
 
## Preprocessing
Field
* Name: 

依據名字的title如```['Mr.', 'Mrs.', 'Miss.', 'Master', 'Other']```分成5類

* Age:

處理missing value，以名字title分群，並以每個title group的年齡中位數值填補

* Cabin

與艙等位置有關，

* Embarked

missing value用```S```填補(```S```出現次數最多)

* Fare

missing value由全部fare的平均填補

## Modeling
Environment: Google Colab

Random Forest Classifier + GridSearchCV

best estimator:
```
RandomForestClassifier(bootstrap=True, ccp_alpha=0.0, class_weight=None,
                       criterion='gini', max_depth=4, max_features='auto',
                       max_leaf_nodes=None, max_samples=None,
                       min_impurity_decrease=0.0, min_impurity_split=None,
                       min_samples_leaf=3, min_samples_split=4,
                       min_weight_fraction_leaf=0.0, n_estimators=40,
                       n_jobs=None, oob_score=True, random_state=None,
                       verbose=0, warm_start=False)

```

## Result
Public leaderboard: 0.78947 (~10%)
