# Type Ia Supernova Calibration Example

This folder contains the mock Type Ia supernova (SN Ia) calibration analysis accompanying  
*“Analytic Marginalization over Binary Variables in Physics Data” (Högås et al., 2025).*

## Contents
- **SN_Ia_Calibration.ipynb** – main notebook generating mock data, fitting the model, and visualizing posterior distributions.  
- **data/** – input mock data and mass-distribution templates.  
- **plots/** – generated figures (mass distribution, log-mass uncertainties, marginalized posteriors, etc.).

## Method Summary
The mock dataset mimics the structure of the Pantheon+ compilation and includes:
- **Calibrator SNe:** distance moduli drawn from Cepheid-based SH0ES distances.  
- **Hubble-flow SNe:** distance moduli computed from a flat ΛCDM cosmology.  
- **Host masses:** drawn from the Pantheon+ distribution with redshift-dependent uncertainty modeled as  
  \[
  \delta_\mathrm{stat}(z) = c\,(1+z)^n,
  \]
  with a systematic floor $\delta_\mathrm{meth}$ added in quadrature.

The method compares the **Ising-marginalized** treatment of host-mass uncertainty with the standard **fixed (deterministic)** mass-step approach, showing that:
- Host-mass uncertainty affects the inferred mass-step parameters $(\gamma, M_\star)$,  
- but has negligible impact on the cosmological parameters $(H_0, \Omega_m, M_B)$.
