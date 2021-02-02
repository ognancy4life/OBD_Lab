This .zip archive contains Quality Controlled float data for biogeochemical profiling floats deployed by the Southern Ocean Carbon and Climate Observation and Modeling (SOCCOM) program.  Additional University of Washington/MBARI floats deployed outside of the SOCCOM array have also been included in the archive.  Data for all floats were processed by the SOCCOM data management team at the Monterey Bay Aquarium Research Institute (MBARI).

FORMAT:
The ascii files contained herein were formatted to be compatible with Ocean Data View (ODV). Character encoding is UTF-8. ODV is freely available at https://odv.awi.de/.  In addition, a Matlab function has been provided in each .zip archive for parsing the .txt files into data structures within Matlab (see get_FloatViz_data.m).  Please note that the data files within this .zip archive represent a snapshot of all SOCCOM float data processed at MBARI as of the date listed in the file name.  Therefore, be aware that processing updates (** AND THUS CHANGES TO THE DATA **) may have occurred since the time the snapshot was created.  For the most up-to-date files (processed every 4 hours), visit ftp://ftp.mbari.org/pub/SOCCOM/FloatVizData/ or http://www.mbari.org/science/upper-ocean-systems/chemical-sensor-group/floatviz/

ALTERNATE FORMATS: NetCDF and Matlab
Matlab and NetCDF formatted files are provided for each ODV text file.  The Matlab format is loaded as structure, FloatViz, with the ODV parameter names as the structure's fieldnames.  The NetCDF format is similar to ARGO Float NetCDF format in its structure.  The parameter names, however, match the ODV text parameter names.  In addition to the quality control flag strings that ARGO profiles use, an array of quality control flags is provided in the NetCDF files for programming convenience.

QUALITY CONTROL DOCUMENTATION:
Quality control (QC) of SOCCOM float data is performed routinely by SOCCOM data managers at MBARI.  QC notification emails are currently being sent out periodically to inform users of key updates to processing, QC and/or sensor calibrations for specific floats.  Comments on recent processing updates are also included.  All QC emails as of the date of this snapshot are included in each downloadable zip file.

PARAMETERS:
For information pertaining to float identification, sensor arrays, data parameters, and quality control please refer to descriptions within the file headers.  Snapshots created after Jan 01, 2017 include estimated total alkalinity and derived carbon parameters for DIC and pCO2 using one of three algorithms (LIAR, MLR, or CANYON).  Floats without a pH sensor will not have these additional parameters within their respective data files.  See file headers for details.  Additionally, files located at the urls listed above will include carbon parameters derived using observed pH and total alkalinity estimated by the LIAR method.

RESOLUTION:
This archive contains either low resolution or high resolution data.  The format is defined by the folder name: SOCCOM_LoResQC_METHOD_ddmmmyyy or SOCCOM_HiResQC_METHOD_ddmmmyyyy (where METHOD = LIAR, MLR, or CANYON).  Note that for APEX floats, the low resolution files only report data at depths where biogeochemical sensors sample, while the high resolution files merge this low resolution data with higher resolution pressure, temperature and salinity data (sampled every two meters in the upper 1000 meters).  Be aware that, due to the merging of the two separate sampling schemes by interleaving the LowRes samples into the HiRes sample structure, HiRes files could potentially contain separate sets of samples with duplicate pressure values. For Navis floats all biogeochemical sensors except nitrate are sampled every 2 meters in the upper 1000 m.  Starting with the Dec2020 snapshot archive, all Navis float data is contained in both the LoRes and HiRes archive.

DISCLAIMER:
These data are provided as-is.  We do our best to provide high-quality, complete data but make no guarantees as to the presence of errors within the data themselves or the algorithms used in the generation of derived parameters.  It is the user's responsibility to ensure that the data meets the user's needs.  However, please report any observed discrepancies in the data to the contact listed below and we will do our best to fix them.  

ACKNOWLEDGEMENTS: 
Authors using SOCCOM float data should acknowledge that "Data were collected and made freely available by the Southern Ocean Carbon and Climate Observations and Modeling (SOCCOM) Project funded by the National Science Foundation, Division of Polar Programs (NSF PLR-1425989, with extension NSF OPP-1936222), supplemented by NASA, and by the International Argo Program and the NOAA programs that contribute to it. The Argo Program is part of the Global Ocean Observing System (https://doi.org/10.17882/42182, https://www.ocean-ops.org/board?t=argo)". In addition, users should reference the appropriate SOCCOM DOI, as listed on each page under Cite This Work.

CONTACT:
Please report any discrepancies, problems or concerns to the following and include "FLOATVIZ SNAPSHOT PROCESSING" in the subject line of the email.
Tanya Maurer tmaurer@mbari.org
Josh Plant jplant@mbari.org
SOCCOM Data Management
MBARI
7700 Sandholdt Road
Moss Landing, CA 95039
