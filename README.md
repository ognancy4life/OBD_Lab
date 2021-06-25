# OBD_Lab

TO DO:
* Switch to Pangeo Binder and/or 2i2c binder for longer sessions and more memory (use workers)

Repository for Ocean Biogeochemical Dynamics (OBD) Graduate Lab Course at USF College of Marine Science

Click the badge below to launch a binder. Everything will be self-contained and you should not have to install python or any toolboxes on your own machine to run the code. Beware that anything you do while in the binder will not be saved. If you wish to save any output or figures, you should download them to you computer from inside the binder.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ognancy4life/OBD_Lab/HEAD)

Notebooks:

-`OBD_SOCCOM_L3.ipynb` walks through downloading a SOCCOM data snapshot and doing some basic data cleaning and plotting for one float at a time.

-`NOAA PMEL CO2 Mooring.ipynb` walks through downloading KEO mooring data from NOAA PMEL and plotting the seasonal cycle, decomposing the thermal and nonthermal drivers of pCO2. We then compare to a second mooring at a different location.

-`OBD_SOCCOM_CO2SYS.ipynb` dowloads the data for one SOCCOM float at a time and then walks through using PyCO2SYS (https://pyco2sys.readthedocs.io/en/latest/) to do carbonate system calculations. We calculate aragonite saturation state from a single SOCCOM float and compare against predicted conditions 50 years in the future.

-`OBD_SOCCOM_MixedLayerDecomposition.ipynb` dowloads the data for one SOCCOM float at a time and then walks through using PyCO2SYS (https://pyco2sys.readthedocs.io/en/latest/) to do carbonate system calculations. We then do a simple mixed layer decomposition of the drivers of carbonate chemistry.
