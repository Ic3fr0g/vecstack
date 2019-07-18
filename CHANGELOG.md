# Changelog

### v0.4.0 -- July 18, 2019

Since v0.4.0 vecstack provides official support for Python 3.5 and higher only,  
but still there is unofficial support for Python 2.7 and Python 3.4.  
Please see [details](https://github.com/vecxoz/vecstack/blob/master/PY2.md).

Scikit-learn API:
* Fixed #29. Out-of-memory in np.random.choice for very large ranges

Functional API:
* Feature #18. Added support for N-dimensional input. Useful for convolutional nets.
* Added aliases for `mode` parameter values which correspond to respective `variant` parameter values of `StackingTransformer`:
  * 'oof_pred_bag' == 'A'
  * 'oof_pred' == 'B'

### v0.3.0 -- April 6, 2018

Introducing Scikit-learn API: `StackingTransformer`

* Standard transformer class with `fit` and `transform` methods
* Compatible with `Pipeline` and `FeatureUnion`

### v0.2.2 -- February 23, 2018

* Fixed #5 (wrong behavior during sparse matrix processing)
* Improved input data validation
* Improved sparse matrix processing

### v0.2.1 -- January 24, 2018 -- Maintenance release

* Minor modifications

### v0.2 -- January 23, 2018

New features:

* Classification with probabilities
* Modes: compute only what you need (only OOF, only predictions, both, etc.)
* Save resulting arrays and log with model parameters

### v0.1 -- November 22, 2016 -- Initial release

Features:

* Functional stacking API
* Regression
* Classification with class labels
* Ordinary and stratified k-fold split
* User-defined metric
* User-defined transformations for target and prediction
