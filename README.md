# Cantera & CoolProp Thermodynamic Comparisons

This repository mainly contains Jupyter notebook scripts comparing thermodynamic properties using Canteras and CoolProps integrated Equations of State (EOS)
It includes thermodynamic property comparisons of pure substances, mixtures, as well as my attempts at combustion simulations.

## Repository Structure

```text
.
├── LICENSE
├── README.md
├── environment_Packages.txt         # List of Conda environment packages
├── Basics.ipynb                     # Cantera vs CoolProp interface comparison
│
├── Single_Species_Thermodynamics/
│   ├── Fluid_Reference_Data/        # NIST reference data for pure substances
│   ├── Basic_Properties_with_EOS_variation.ipynb       # EOS comparison for pure substances
│   ├── Basic_Properties_with_EOS_variation_Plotting.ipynb  # Visualization of pure substance comparison results
│   ├── Graphs/                      # Generated plots
│   └── DataResults/                 # Raw data
│
└── Multi_Species_Thermodynamics/
    ├── Fluid_Reference_Data/        # Extracted literature data
    ├── Law_H2AirDensities.ipynb     # H2-Air mixture density analysis
    ├── Law_CH4N2Densities.ipynb     # CH4-N2 mixture density analysis
    ├── Law_CriticalPT.ipynb         # Critical properties of H2/CH4-air mixtures
    ├── Law_LamFlameSpeeds.ipynb     # Laminar flame speed simulations (Needs more work)
    ├── Graphs/                      # Mixture plots
    └── DataResults/                 # Mixture raw data
```

## Installing conda:
bash <conda-installer-name>-latest-Linux-x86_64.sh    (Edit the command to reflect which conda package you've downloaded)

## Installing cantera, ipython, matplotlib, jupyter
conda create --name ct-env --channel conda-forge cantera ipython matplotlib jupyter
# To use the created environment, run
conda activate ct-env

## Installing CoolProp
conda install conda-forge::coolprop

## Additional Information
[https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html] on how to install the conda Package manager (Miniconda or CondaForge is recommended)

[https://cantera.org/stable/install/conda.html#sec-install-conda] on how to install Cantera in a conda environment

[http://www.coolprop.org/coolprop/wrappers/Python/index.html#automatic-installation] on installing the CoolProp Package

## References
- [Cantera Documentation](https://cantera.org/index.html)
- [CoolProp Documentation](http://www.coolprop.org/)
- Wenkai Liang∗, Weiyu Li, Chung K. Law (2019). Lam flame Propagation in supercritical HMeAir mixtures, [https://doi.org/10.1016/j.proci.2018.06.070]
- Lentner et al. (2020). Density measurements of seven methane-rich binary mixtures -,,- , [https://doi.org/10.1016/j.jct.2019.106002]
- NIST Chemistry WebBook, its Thermochemistry data section: [https://webbook.nist.gov/chemistry/]
- & its Fluid Chemistry Section: [https://webbook.nist.gov/chemistry/fluid/]
