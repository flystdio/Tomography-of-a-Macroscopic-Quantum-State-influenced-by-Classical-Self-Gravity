# SN ellipse two-angle-set supplementary data

This directory contains the numerical data used for the `SN_ellipse_two_angle_sets` plot at the current parameters.

## Parameters

- `T_tomo = 0.0003 K`
- `Omega_q / 2pi = 0.1 Hz`
- free evolution disabled, `t_eval = 0 s`
- `V_init = (0.2, 1, 10)`
- angle set A: `0, \pi/4, \pi/2`
- angle set B: `\pi/3, 2\pi/3, \pi`

## Files

- `metadata.json`: parameters, derived scales, and summary distances.
- `covariances.csv`: initial and reconstructed covariance matrices in both original `omega_q` normalization and plotted `Omega_q` normalization.
- `ellipse_points.csv`: sampled one-standard-deviation ellipse coordinates used for plotting, in `x / delta x_q` and `p / delta p_q`.
- `noise_components.csv`: per-angle noise components used before covariance reconstruction.
- `covariance_components.csv`: reconstructed covariance increments by noise component.
