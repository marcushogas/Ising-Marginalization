# Type Ia Supernova Calibration Example

This folder contains the mock Type Ia supernova (SN Ia) calibration analysis accompanying  
*“Analytic Marginalization over Binary Variables in Physics Data” (Högås et al., 2025).*

## Contents
- **SN_Ia_Calibration.ipynb** – main notebook generating mock data, fitting the model, and visualizing posterior distributions.  
- **Pantheon+SH0ES.dat** – input data from Pantheon+ and SH0ES.  
- **table6.txt** – input data from SH0ES.

## Method Summary
The mock dataset mimics the structure of the Pantheon+ compilation and includes:
- **Calibrator SNe:** distance moduli drawn from Cepheid-based SH0ES distances.  
- **Hubble-flow SNe:** distance moduli computed from a flat ΛCDM cosmology.  
- **Host masses:** drawn from the Pantheon+ distribution with redshift-dependent uncertainty plus a systematic floor added in quadrature.

Before running the notebook, make sure the following folders exist in the same directory:
data/, output/, and plots/.
These folders are used to store input data, generated results, and figures, respectively.
