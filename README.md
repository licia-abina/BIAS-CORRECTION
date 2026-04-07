# BIAS-CORRECTION
This repository implements a comprehensive framework for bias correction of satellite rainfall and model-derived discharge in data-scarce regions.

The workflow integrates:

Satellite rainfall correction (CHIRPS)
Hydrological discharge correction (VegDischarge)
Multiple bias correction methods:
Random Forest (RF)
Linear Scaling (LS)
Quantile Mapping (QM)
Delta Method

The framework operates at both:

Monthly scale (primary correction)
Daily scale (refined + constrained by monthly results)
However, the monthly bias correction should preceed the daily bias correction (daily uses monthly outputs as input).

Requirements: 
numpy>=1.21
pandas>=1.3
matplotlib>=3.5
scipy>=1.7
rasterio>=1.3
scikit-learn>=1.0
geopandas>=0.12


If using this workflow, please cite:

Yeboah et al. (2026). Toward reliable water resource assessment: correcting bias in satellite-based rainfall and model-derived discharge in Kenya’s Central Highlands.
