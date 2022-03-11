This folder contains the codes to reproduce the analysis and figures from Olinger et al 2022.

The entire project is contained within the notebook "riftquake_analysis.ipynb."

Seismic data is downloaded from IRIS as part of the workflow. Seismic data files will be placed in data/MSEED/raw and data/XML. Approppiate directories for each station and component will be made in data/MSEED/no_IR when the instrument response is removed from the raw data. Processed GPS data, imagery, and shapefiles are included in the data directory. 

Individual code files are located in the folder that corresponds to the code type. For instance, the files to prepare templates and run template matching are in detection/template_match.py.

Outputs for each step are dumped into the respective folder within the directory outputs. For instance, figures will be placed in outputs/figures.

The only exception to this is the folder "greens_functions," which contains the Green's functions used for deconvolution and the MATLAB model that produced them. The model is not called in "riftquake_analysis.ipynb," but it is included should someone want to apply it. 

Many of the functions produce large files that are then necessary inputs for other functions. To reproduce the entire project, you must run the workflow from start to finish! If you would like to reproduce a particular step without running the workflow up that point, feel free to contact me at setholinger@fas.harvard.edu and I will transfer any files required to run that particular step.

-S
