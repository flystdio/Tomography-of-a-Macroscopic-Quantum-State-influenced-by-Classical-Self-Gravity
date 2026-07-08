# Matched-temperature manual-time tomography data

This directory contains the numerical data for the matched-temperature manual-time tomography contour plot generated at `t_eval = 0`.

## Parameters

- `t_eval = 0 s`
- `V_init = (0.2, 1.0, 10.0)`
- `Omega_q / 2pi`: `0.01` to `10` Hz, 320 logarithmic grid points
- shared temperature `T_init = T_tomo`: `1e-5` to `1e-2` K, 800 logarithmic grid points
- noise convergence: `min_points = 8000`, `max_points = 128000`, relative tolerance `1e-3`, unconverged finest-grid values allowed
- plotted quantity: `D_geo = 1 - B_cl(V_SN^recon, V_QG^recon)`

## Files

- `metadata.json`: parameters, source cache information, noise settings, and summary statistics.
- `manual_time_grid_long.csv`: full 320 x 800 grid in tidy long-table form.
- `D_geo_matrix.csv`: plotted distinguishability grid as a matrix.
- `B_cl_overlap_matrix.csv`: classical overlap grid as a matrix.
- `sn_det_grid_matrix.csv`: `det(V_SN^recon)` grid as a matrix.
- `free_state_grid.csv`: SN/QG initial covariances at each temperature and the selected free-evolution time.
- `sn_det_zero_boundary.csv`: refined `det(V_SN^recon)=0` boundary points.
- `figure.pdf`: PDF copy of the corresponding contour plot.
