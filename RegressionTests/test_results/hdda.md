High Dimensional Discriminant Analysis (`hdda`)
===== 

There are regression tests to compare model results between different versions of `caret` and the individual packages. These test evaluate whether consistent results can be obtained. The code used to generate the objects that are compared can be found [here](https://github.com/topepo/caret/blob/master/RegressionTests/Code/hdda.R).
A [history of commits](https://github.com/topepo/caret/commits/master/models/files/hdda.R) for the model code is also available

Testing Information:
---------

Old:

 * x86_64-apple-darwin13.4.0 (64-bit)
 * R version 3.3.3 (2017-03-06)
 * `caret` (6.0-73), `HDclassif` (2.0.2), `MASS` (7.3-45)
 * tested on 2017-04-12 at 20:24. 
 * total test time: 13.4s


New:

 * x86_64-apple-darwin13.4.0 (64-bit)
 * R version 3.3.3 (2017-03-06)
 * `caret` (6.0-75), `HDclassif` (2.0.2), `MASS` (7.3-45)
 * tested on 2017-04-11 at 20:31. 
 * total test time: 10.6s


Results:
---------

**Test Case**: `class_cv_form`

Object class(es): `train` and `train.formula`

Model Configuration:

 * Formula method
 * Resampling: Cross-Validated (3 fold)
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 3 tuning parameter combinations were evaluated


Execution times: (old) 1s (new) 0.66s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_cv_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: Cross-Validated (3 fold)
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 3 tuning parameter combinations were evaluated


Execution times: (old) 1.76s (new) 1.09s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_loo_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: Leave-One-Out Cross-Validation
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 3 tuning parameter combinations were evaluated


Execution times: (old) 6.29s (new) 5.51s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_none_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: None
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 0 tuning parameter combinations were evaluated


Execution times: (old) 0.58s (new) 0.24s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_none_pred`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_none_prob`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `class_pred`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_pred_form`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_prob`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `class_prob_form`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `class_rand`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: Cross-Validated (3 fold)
 * Random search
 * Pre-processing: None  
 * 4 tuning parameter combinations were evaluated


Execution times: (old) 0.93s (new) 0.64s

Test Results:

 * _Equal results for Accuracy_
 * _Equal results for Kappa_

**Test Case**: `levels`

Object class(es): `character`

 * _Equal results_

