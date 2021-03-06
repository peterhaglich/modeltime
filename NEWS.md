
# modeltime 0.0.2.9000 (Development Version)

### Fixes

- `modeltime_forecast()`: More descriptive errors when external regressors are required. 
- `prophet_reg()` & `prophet_boost()`: More descriptive error message when less than 100 observations are trained on. Prophet requires >= 100 observations per [facebook/prophet#1554](https://github.com/facebook/prophet/issues/1554)

# modeltime 0.0.2

### Confidence Interval Estimation

- `modeltime_forecast()`: Now estimates confidence intervals using centered standard deviation. The mean is assumed to be zero and residuals deviate from mean = 0. 

### Fixes

- Updates to work with `parsnip` 0.1.2.
- `prophet_boost()`: Set `nthreads = 1` (default) to ensure parallelization is thread safe. 

# modeltime 0.0.1

* Initial Release
