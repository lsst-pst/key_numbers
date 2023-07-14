##################################################
Rubin Observatory System & LSST Survey Key Numbers
##################################################

This repository contains files of Rubin Observatory LSST System Parameters and Key Numbers. 
The System Parameters have been extracted from the Rubin Observatory System Model and the Key Numbers are imported initially from the confluence page <https://confluence.lsstcorp.org/display/LKB/LSST+Key+Numbers>

This repository should become the single source for metrics, quantities or notes or science estimates that are frequently looked up for talks.

The System paramter files are in xml format and have been extracted from the Rubin Observatory system model. 
These xml files serve as the source of truth for the calculation of System key numbers. 
The format will prbably be changed

Files in this repository:

 - xml/LPM-17_LSE-29_30_59_60_61_62_89_Requirement_Parameters.xml extract of all model parameters in specicication documents LPM-17, LSE-29, LSE-30, LSE-59, LSE-60, LDM-61, LXX-62, LXX-89
 - doc/LKB-LSSTKeyNumbers-140723-1454-13798.pdf : which captures a discuss on key numbers from confluence

 This repository contains code to compute key numbers derived from the LSST SRD System Parameters. 

######
Inputs
######

To date there have been several reference documents quoting the baseline configuration and key numbers. All should be reviewed, the relevant information migrated to this repository and then deprecated. 

* `LSST Key Numbers confluence <https://confluence.lsstcorp.org/display/LKB/LSST+Key+Numbers>`_ LSST Key System Parameters Summary
* `Document-16 <https://docushare.lsst.org/docushare/dsweb/Get/Document-16>`_ excel spreadsheet contains the LSST baseline configuration from 2009-04. 
* `Document-4169 <https://docushare.lsst.org/docushare/dsweb/Get/Document-4169>`_ excel spreadsheet contains the LSST baseline configuration from 2009-04. 
* `Document-16168 <https://docushare.lsst.org/docushare/dsweb/Services/Document-16168>`_
* `Collection-886 <https://www.lsstcorp.org/docushare/dsweb/View/Collection-886>`_

LSST throughput curves are described in https://github.com/lsst/throughputs/tree/master/baseline

#######
Outputs
#######

A pdf document of the numbers in this repository can be generated for versioning and citation,  and uploaded to Docushare, if desired. 

####
TODO
####

* The information from Document-16 needs to be reviewed. Information that is stil lrelevant should be migrated to this repository and the Document-16 deprecated. 
* The original confluence page is very DM and data-volume centric. Should add basic metrics on collecting area, image quality, etc., to make it a more community-useful data sheet as well as a better resource for preparing and fact-checking talks.
* Add nominal camera numbers, e.g number/pixel count of CCDs, oixel scale, readnoise, dark current, non-linearity, full well depth,  cross-talk, QE(lambda), lens reflectivities, expected gain. (Steve R added some already to the confluence page)

######
Design
######
* Look at the astropy a model: https://docs.astropy.org/en/stable/cosmology/
* astropy.units for aasec, etc: astropy.units.core.PrefixUnit


###########
Maintainers
###########
The contents of this repository are maintained by the Rubin Subsystem Scientists. 


#########
Resources
#########
https://towardsdatascience.com/replacing-excel-with-python-30aa060d35e

How to enable a password for a

https://jupyter-notebook.readthedocs.io/en/stable/public_server.html

