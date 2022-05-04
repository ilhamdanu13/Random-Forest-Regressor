# Random Forest Regressor
This algorithm is a combination of each tree from the decision tree which is then combined into a single model.

Random Forest is an algorithm for classification. Then, how does it work? Random Forest works by building several decision trees and combining them to get more stable and accurate predictions. The 'forest' built by Random Forest is a collection of decision trees which are usually trained by the bagging method. The general idea of ​​the bagging method is a combination of learning models to improve overall results

The Random Forest algorithm increases the randomness of the model while growing the tree. Instead of looking for the most important feature when splitting a node, Random Forest looks for the best feature among a random subset of features. As a result, this method produces a wide variety and generally results in better models.

![Logo](https://cdn.analyticsvidhya.com/wp-content/uploads/2020/02/rfc_vs_dt1.png)





# Import Package
import common package:

import **numpy as np**

import **pandas as pd**


from **sklearn.model_selection** import **train_test_split**

from **sklearn.pipeline** import **Pipeline**

from **sklearn.compose** import **ColumnTransformer**


from **jcopml.utils** import **save_model, load_model**

from **jcopml.pipeline** import **num_pipe, cat_pipe**

from **jcopml.plot** import **plot_missing_value**

from **jcopml.feature_importance** import **mean_score_decrease**

import Algorithm's Package:

from **sklearn.ensemble** import **RandomForestRegressor**

from **sklearn.model_selection** import **GridSearchCV**

from **jcopml.tuning** import **grid_search_params as gsp**