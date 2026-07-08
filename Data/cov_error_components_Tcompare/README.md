# Covariance error component comparison data

This directory contains the numerical data used for the covariance error component comparison plot.

## Parameters

- `Omega_q / 2pi`: `0.01` to `10` Hz, 512 logarithmic scan points
- tomography temperatures: `1e-4 K` and `1e-3 K`
- free evolution disabled: `t_eval = 0`, `init_T = 0`
- `V_init = (0.2, 1.0, 10.0)`
- noise convergence: `min_points = 8000`, `max_points = 128000`, relative tolerance `1e-3`, unconverged finest-grid values allowed

## Files

- `metadata.json`: parameters, source cache information, and summary statistics.
- `cov_error_components_long.csv`: tidy long table containing QG, SN, and SN-QG covariance error components for both temperatures.
- `cov_error_components_matrix_T0p0001.csv`: wide table for `T_tomo = 1e-4 K`.
- `cov_error_components_matrix_T0p001.csv`: wide table for `T_tomo = 1e-3 K`.
- `figure.pdf`: PDF copy of the corresponding comparison plot.
