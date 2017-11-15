# Creating a synthetic population for a whole country
- Author: William Sexton
- Daniel Lin
- Last Modified: 10/02/2017 by Daniel

The programs for this project are ran under the following directory structure:

###Project
- docs
- inputs
  - housing_data
  - person_data
- outputs
  - housing_rep
  - person_recode
  - person_rep
- programs
- tests
- README.md


This directory contains the most recent version of the code used to create SynPopulation. We modified the bootstrap process to account for flaws in the previous versions. This code maintains the runtime improves of [ACS_multiprocessing](/labordynamicsinstitute/SynUSpopulation/tree/ACS_multiprocess).

## Inputs
Assumes you have folders containing the raw ACS person and raw ACS housing data within the directory containing python code.

## Outputs

Also you must create the follow empty folder: housing_rep, person_rep, person_recode.

## To run
`python gen_counts.py [folder for raw ACS person data] [folder for raw ACS housing data]`

`python rep_syn_housing.py [folder for raw ACS housing data]`

`python rep_syn_person.py [folder for raw ACS person data]`

`python recode.py [folder containing output from rep_syn_person]`
