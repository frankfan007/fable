# fable (development version)

## Breaking changes

* The sample path means are now used instead of analytical means when forecasts 
  are produced from sample paths.

# fable 0.2.0

## Improvements

* Added autoregressive modelling with `AR()`.
* Better handling of rank deficiency in `ARIMA()`.
* Added `generate.ARIMA()` method.
* Added bootstrap forecast paths for `ARIMA()` models.
* `ARIMA()` specials now allow specifying fixed coefficients via the `fixed` argument.
* Documentation improvements.

# fable 0.1.2

## Improvements

* Added `CROSTON()` for Croston's method of intermittent demand forecasting.
* Documentation improvements

## Bug fixes

* Fixed NNETAR & VAR handling of missing values (#215).
* Fix ETS forecasting with forecast horizons less than the seasonal period (#219).
* Fixed season() special for non-seasonally based time indices (#220)
* Fix issue with simulation forecasting from damped ETS models.

# fable 0.1.1

## Improvements

* Added interpolation method for `MEAN()` model (#203).
* Added rolling mean option for `MEAN()` model (#204).

## Bug fixes

* Corrected forecast standard error for drift models.

# fable 0.1.0

* First release.

## New features

* Support for 9 models and relevant methods: `ARIMA`, `ETS`, `TSLM`, `MEAN`, `RW`, `NAIVE`, `SNAIVE`, `NNETAR`, `VAR`.
