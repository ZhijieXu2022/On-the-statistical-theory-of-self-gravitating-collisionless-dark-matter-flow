# Dark matter flow data and manuscript

Data and manuscript for **Xu, Z. (2023), *On the statistical theory of self-gravitating collisionless dark matter flow*, Physics of Fluids 35, 077105, doi:[10.1063/5.0151129](https://doi.org/10.1063/5.0151129), arXiv:[2202.00910](https://arxiv.org/abs/2202.00910)** (revised edition, v2).

The complete archive, with the same files, is on Zenodo: [doi:10.5281/zenodo.23902041](https://doi.org/10.5281/zenodo.23902041).

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.23902041.svg)](https://doi.org/10.5281/zenodo.23902041)

## Major findings

Virgo SCDM N-body simulation, redshifts z = 10 to 0:

- Exact kinematic relations link the correlation, structure, dispersion and spectrum functions of three idealized flows: incompressible, constant-divergence and irrotational. Incompressible and constant-divergence flows share the same relations for even-order correlations.
- The peculiar velocity is a constant-divergence flow on small scales, where particle pairs sit in the same halo, and an irrotational flow on large scales, with the transition near r<sub>t</sub> ≈ 1.3 Mpc/h.
- Because the flow is collisionless, the longitudinal velocities of two particles at vanishing separation are only partly correlated: the limiting correlation coefficient is ρ<sub>L</sub> = 1/2, compared with ρ<sub>L</sub> = 1 for incompressible flow.
- On large scales the transverse velocity correlation is exponential, T<sub>2</sub> ∝ e<sup>−r/r<sub>2</sub></sup>, with a time-independent comoving scale r<sub>2</sub> ≈ 23.1 Mpc/h that may be related to the horizon size at matter–radiation equality; all other velocity, density and potential statistics on these scales then follow analytically.
- On small scales the longitudinal structure function follows a one-fourth law, S<sub>2</sub><sup>l</sup> ∝ r<sup>1/4</sup>, from which the remaining small-scale statistics follow.
- Vorticity is negatively correlated for separations between 1 and 7 Mpc/h, and divergence for r ≳ 33 Mpc/h, which produces a negative density correlation on those scales.

## Contents

| Path | Content |
|---|---|
| `P20_revised.pdf` | Manuscript, revised edition (23 pages) |
| `statistics/` | 26 files: every pair statistic as a function of separation r, at redshifts z = 10 ... 0 |
| `tables/` | 11 files: the small result tables of the paper (see the index below) |
| `figures/` | 26 files: every plotted series of Figs 3-28 |
| `CITATION.cff`, `LICENSE` | citation metadata and licence |

## Format of the CSV files

Each file starts with comment lines beginning with `#`, then a header row, then data.

- `# Publisher`: author and contact.
- `# Updated`: date of the last update.
- `#Name`: what the file contains.
- `#Ref. [n]`: the equation and figure of the paper the data belong to, with the DOI.
- `#Note`: processing notes, where needed.

Statistics files use a common layout: the first column is the separation r in Mpc/h, and each further column is one redshift (`z=10`, `z=5`, ... `z=0.0`). Values of -1 mark separations where the statistic is not defined for that redshift. Velocities are in units of u0 (the rms velocity at z = 0, 354.6 km/s) unless the header says otherwise. Distances are comoving, in Mpc/h. Units are stated in the `#Name` line of each file.

## Index of the tables

| File | Content | Paper |
|---|---|---|
| `tables/01_u_rms_velocity_vs_redshift.csv` | rms peculiar velocity u(z) | Eq. (1), Fig. 21 |
| `tables/02_amplitude_a0_and_length_scales_vs_redshift.csv` | amplitude a0(a) and length scales r_t2, r_t, r_d | Eq. (110), Figs 11, 21 |
| `tables/03_table3_smooth_connection_parameters.csv` | parameters of the smooth connections, published and refitted | Table 3, Eqs (147-154), Fig. 27 |
| `tables/04_velocity_dispersion_tensor_in_spheres_z0.csv` | velocity dispersion tensor in spheres around random particles, z = 0 | Eq. (36), Figs 15, 16 |
| `tables/05_cosine_pdfs_z0.csv` | probability densities of cosines of the angles, z = 0 | Eqs (21, 22), Figs 19, 20 |
| `tables/06_angle_pdfs_z0.csv` | probability densities of the angles, z = 0 | Eqs (21, 22), Figs 19, 20 |
| `tables/07_matter_power_spectrum_nbody_z0.csv` | matter power spectrum P(k) from the N-body data, z = 0 | Eq. (133), Fig. 23 |
| `tables/08_matter_power_spectrum_theory.csv` | linear and Peacock & Dodds (1996) nonlinear P(k) | Fig. 23 |
| `tables/09_all_scale_fits_and_velocity_gradient_correlations_z0.csv` | all-scale fits R2, L2, T2 and divergence/vorticity correlations | Eqs (96, 97, 147-154), Figs 27, 28 |
| `tables/10_numbers_in_text.csv` | every number quoted in the text, compared with its recomputed value | whole paper |
| `tables/11_equation_audit.csv` | equation-by-equation audit of all 154 equations | whole paper |

The figure files (`figures/`) are named by figure number, for example `Fig22_density_correlation.csv` for Fig. 22. `Fig03_velocity_correlations.csv` is the source of `Fig04_velocity_correlations_lin.csv` and `Fig05_crossover_rt.csv`.

## Related datasets

- Dark matter flow dataset, Part II (correlation-based statistics): doi:[10.5281/zenodo.6757654](https://doi.org/10.5281/zenodo.6757654)
- Dark matter flow dataset, Part I (halo-based statistics): doi:[10.5281/zenodo.6541231](https://doi.org/10.5281/zenodo.6541231)

The simulation is the Virgo Consortium SCDM run (Jenkins et al. 1998; Frenk et al. 2000).

## Citation

Please cite the article (doi:10.1063/5.0151129) and this archive (doi:10.5281/zenodo.23902041). GitHub's "Cite this repository" button uses `CITATION.cff`.

## Licence

The text, figures and data in this repository are licensed under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/). See `LICENSE`.
