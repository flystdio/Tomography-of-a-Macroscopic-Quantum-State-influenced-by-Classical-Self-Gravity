# SN reconstructed determinant parameter-space data

This directory contains the numerical grid used for the SN reconstructed determinant parameter-space plot.

## Parameters

- model: `SN`
- `V_init = (0.2, 1.0, 10.0)`
- `Omega_q / 2pi`: `0.01` to `10` Hz, 320 logarithmic grid points
- `T`: `1e-5` to `1e-2` K, 800 logarithmic grid points
- noise convergence: enabled, `min_points = 8000`, `max_points = 128000`, relative tolerance `1e-3`, unconverged finest-grid values allowed
- plotted color scale: `log10[4 det(V_recon_SN) / hbar^2]` for positive determinant values

## Files

- `metadata.json`: parameters, source cache information, normalization, and summary statistics.
- `det_grid_long.csv`: full 320 x 800 determinant grid in tidy long-table form.
- `det_grid_matrix.csv`: determinant grid as a matrix, with temperature columns and measurement-strength rows.
- `positive_log10_matrix.csv`: plotted positive-log color values as a matrix; non-positive determinant entries are blank.
- `contour_crossings.csv`: log-interpolated crossings of `det_ratio = 0` and `det_ratio = 1` along temperature at each measurement-strength grid row.
- `figure.pdf`: PDF copy of the corresponding plot.
