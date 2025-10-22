# Type Ia Supernova Calibration Example

This folder contains the mock Type Ia supernova (SN Ia) calibration analysis accompanying  
*“Analytic Marginalization over Binary Variables in Physics Data” (Högås et al., 2025).*

## Contents
- **[Mock_SNIa_Cal.ipynb](Mock_SNIa_Cal.ipynb/).ipynb** – main notebook generating mock data, fitting the model, and visualizing posterior distributions.  
- **[Pantheon+SH0ES.dat](Pantheon+SH0ES.dat/)** – input data from Pantheon+ and SH0ES.  
- **[table6.txt](table6.txt/)** – input data from SH0ES.

## Method Summary
The mock dataset mimics the structure of the Pantheon+ compilation and includes:
- **Calibrator SNe:** distance moduli drawn from Cepheid-based SH0ES distances.  
- **Hubble-flow SNe:** distance moduli computed from a flat ΛCDM cosmology.  
- **Host masses:** drawn from the Pantheon+ distribution with redshift-dependent uncertainty plus a systematic floor added in quadrature.

Before running the notebook, make sure the data files are placed in the folder data/.

## Attribution
If using the Pantheon+/SH0ES data, please cite [Scolnic et al. 2022](https://iopscience.iop.org/article/10.3847/1538-4357/ac8b7a), [Brout et al. 2022](https://iopscience.iop.org/article/10.3847/1538-4357/ac8e04), and [Riess et al. 2022](https://iopscience.iop.org/article/10.3847/2041-8213/ac5c5b)
