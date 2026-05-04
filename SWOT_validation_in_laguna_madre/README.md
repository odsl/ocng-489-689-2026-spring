# OCNG 689: Satellite Oceanography Spring 2026 Final Project

## Validating Surface Water Ocean Topography (SWOT) Sea Surface Height Altimetry Data with Tide Gauge Sea Level Observations in the Laguna Madre

By: Nayana Venukanthan, under Drs. Jinbo Wang, Ping Chang, Texas A&M University (nsv9@tamu.edu)

This project compared SWOT Expert Level 2 and 3 sea surface height anomaly (SSHA) data and sea level (SL) observations from 8 tide gauges from 04/01-07/04/2023
in the Laguna Madre (Gulf of Mexico). The objective was to validate and evaluate SWOT data near the coast with tide gauge observations.

Data files in folder:
SWOT_subset_datacube.ipynb: after downloading SWOT files - SWOT_L2_LR_SSH_Expert and SWOT_L3_LR_SSH_Expert, this file can take in those files and create a datacube 
with data for the whole time period concatenated on a new time index, 

TG_ascii_to_nc.ipynb: load in Tide gauge ASCII files, process them, plot them, and output them as .nc files

SWOT_TGhrly_E2interp.ipynb: where you can load in SWOT datacube (any level or resolution, just change the 'swot_df' variable to the datacube you load in at the top), and TG .nc files and interpolate and plot comparison plots before demeaning, after demeaning, after applying quality filters, and after applying dynamic atmospheric correction (DAC) or inverted barometer correction (IBC). 
