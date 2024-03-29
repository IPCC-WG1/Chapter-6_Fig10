NET EFFECTIVE RADIATIVE FORCING: AEROSOLS
============

Figure number: Figure 6.10  
From the IPCC Working Group I Contribution to the Sixth Assessment Report: Chapter 6  

![Figure 6.10](/ar6_wg1_chap6_fig6_10_netERFmap_SWLW_aer.png?raw=true)

Description:
------------
Multi-model mean Effective radiative forcings (ERFs) due to aerosol changes between 1850 and recent-past (1995-2014).  
Panel (a) shows the spatial distribution of the net ERF with area-weighted global mean ERF shown at the lower right corner. Uncertainty is represented using the advanced approach: No overlay indicates regions with robust signal, where ≥66% of models show change greater than variability threshold and ≥80% of all models agree on sign of change; diagonal lines indicate regions with no change or no robust signal, where <66% of models show a change greater than the variability threshold; crossed lines indicate regions with conflicting signal, where ≥66% of models show change greater than variability threshold and <80% of all models agree on sign of change. For more information on the advanced approach, please refer to the Cross-Chapter Box Atlas.1.  Panel (b) shows the mean shortwave and longwave ERF for each of the 14 regions defined in the Atlas. Violins in panel (b) show the distribution of values over regions where ERFs are significant. ERFs are derived from the difference between top of the atmosphere (TOA) radiative fluxes for Aerosol Chemistry Model Intercomparison Project (AerChemMIP) experiments histSST and histSST-piAer (Collins et al., 2017) averaged over 1995-2014 (Box 1.4, Chapter 1).  The results come from 7 Earth System Models: MIROC6, MPI-I-ESM-1-2-HAM, MRI-ESM2-0, GFDL-ESM4, GISS-E2-1-G, NorESM2-LM, and UKESM-0-LL.   


Author list:
------------
- Kuo, C: Lawrence Berkeley National Laboratory, USA; chaincy@berkeley.edu, chaincy.ipccwg1@gmail.com (lead only); githubid: chaincy-ipcc, githubid: chaincy-cal 

ESMValTool Branch:
------------------
- ESMValTool-AR6-OriginalCode-FinalFigures: [IPCC_AR6_WG1_Ch6](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/tree/IPCC_AR6_WG1_Ch6_ESMValTool)


Recipe & diagnostics:
---------------------
Recipe used: [recipes/ar6ch6/recipe_erf_histSST-piAer_Fig6.10.yml](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/recipes/ar6ch6/recipe_ckuo_ipcc_6_10_erf_histSST-piAer.yml)   

Recipe description:  
Collect the upward shortwave and longwave fluxes at the top of the atmosphere, for AerChemMIP (Collins et al,2017,GMD,10(2),585-607, https://doi.org/10.5194/gmd-10-585-2017) experiments histSST and histSST-piAer, over the period 1995-2014.


Diagnostics used:   
[diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py)

The above diagnostic imports:  
[diag_scripts/ar6ch6/cmapipcc.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/cmapipcc.py)  
[diag_scripts/ar6ch6/ch6_fns.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ch6_fns.py)    
[diag_scripts/ar6ch6/chem_div_disc.txt](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/chem_div_disc.txt)  

Diagnostics description:  
Calculates the spatial distribution of the net ERF with area-weighted global mean ERF, calculated from the difference in upward shortwave and longwave fluxes at the top of the atmosphere, between AerChemMIP experiments histSST and histSST-piAer, averaged over 1995-2014.

Figure 6.10 is created by running the ESMValTool recipe recipes/ar6ch6/recipe_erf_histSST-piAer_Fig6.10.yml  
panel a) will be run through [recipes/ar6ch6/recipe_erf_histSST-piAer_Fig6.10.yml](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/recipes/ar6ch6/recipe_ckuo_ipcc_6_10_erf_histSST-piAer.yml) via [diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py)  
panel b) is created through [https://github.com/IPCC-WG1/Chapter-6_Fig10/tree/main/ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig10/tree/main/ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb) via netcdf output from [diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py)  

Expected image path:
--------------------
This is the path of the image relative to the automatically generated ESMValTool output location:  
- recipe_erf_histSST-piAer_Fig6.10_YYYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf/fig6_erf_piAer.png  


Recipe generations tools: 
-------------------------
N/A


Ancillary figures and datasets:
-------------------------------
Panel b) of Figure 6.10 is created by the file  
[https://github.com/IPCC-WG1/Chapter-6_Fig10/tree/main/ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig10/tree/main/ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb)  
It reads in netcdf output from [diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/blob/IPCC_AR6_WG1_Ch6_ESMValTool/esmvaltool/diag_scripts/ar6ch6/ipcc_ar6wg1_fig6.10_erf_piAer.py), which are output into the recipe path:  
- recipe_erf_histSST-piAer_Fig6.10_YYYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf/erf_hatch_LW.nc
- recipe_erf_histSST-piAer_Fig6.10_YYYYMMDD_HHMMSS/plots/diffexpts/ar6fig6_erf/erf_hatch_SW.nc


Additional datasets:
--------------------
The AR6 WG1 Atlas reference regions are used to produce Figure 6.10b.    
On the Atlas repository: 
[IPCC-WG1/Atlas/reference-regions/IPCC-WGI-reference-regions-v4_shapefile.zip](https://github.com/IPCC-WG1/Atlas/blob/main/reference-regions/IPCC-WGI-reference-regions-v4_shapefile.zip)

What are their access permissions/Licenses?  
The license details can be found at https://github.com/IPCC-WG1/Atlas/blob/main/LICENSE.md    

Software description:
---------------------
- ESMValTool environment file: [IPCC_environments/ar6wg1_chap6_figs_conda_environment.yml](https://github.com/ESMValGroup/ESMValTool-AR6-OriginalCode-FinalFigures/tree/main/IPCC_environments/ar6wg1_chap6_figs_conda_environment.yml)  
- Other software used:  
A Jupyter notebook ([ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb](https://github.com/IPCC-WG1/Chapter-6_Fig10/tree/main/ipcc_ar6wg1_Fig6.10b_FGD_submit.ipynb)) is used to create Figure 6.10 panel b. See section "Ancillary figures and datasets" and "Additional datasets", above, for information.  

Hardware description:
---------------------
Machine used: Mistral  
 
When was this machine used?  
Last used July 2021 to produce figures from ESMValTool  
