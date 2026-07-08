# Noise determinant versus measurement strength data

This directory contains the numerical data used by `plot_noise_components_vs_omega.py` for two tomography temperatures.

## Parameters

- `Omega_q / 2pi`: `0.01` to `10` Hz, 1280 logarithmic scan points
- tomography temperatures: `1e-4 K` and `1e-3 K`
- free evolution disabled: `t_eval = 0`, `init_T = 0`
- `V_init = (0.2, 1.0, 10.0)`
- ellipse panels at `Omega_q / 2pi = 0.05, 0.1, 1` Hz
- noise convergence: `min_points = 8000`, `max_points = 128000`, relative tolerance `1e-3`, unconverged finest-grid values allowed

## Files

- `metadata.json`: parameters, source cache information, and summary statistics.
- `noise_components_vs_omega_curves.csv`: curve data for QG/SN area changes, determinant increments, SN determinant shift, and distinguishability.
- `ellipse_covariances.csv`: covariance matrices for the ellipse panels.
- `ellipse_points.csv`: sampled one-standard-deviation ellipse coordinates for the ellipse panels.
- `figure_T0p0001.pdf`: PDF copy of the `T_tomo = 1e-4 K` plot.
- `figure_T0p001.pdf`: PDF copy of the `T_tomo = 1e-3 K` plot.
