# BEGIN README.txt

gobig_plant - README.txt

./annotations
	Annotations for Viridiplantae (taxon ID: 33090) downloaded from the Gene 
	Ontology Annotation (GOA) database (https://www.ebi.ac.uk/QuickGO/; 
	https://doi.org/10.1093/nar/gku1113). Files are split by GO category (BP: 
	biological process; MF: molecular function; CC: cellular component). Gene-GO 
	term pairs are derived through filtering by evidence (experimental evidence
	codes were selected - ECO:0000352, ECO:0000269, ECO:0000314, ECO:0000315, 
	ECO:0000316, ECO:0000353, ECO:0000270, ECO:0006056, ECO:0007005, 
	ECO:0007001, ECO:0007003, and ECO:0007007).

./GO_terms
	The collected GO terms and their ancestor terms using Python scripts. These 
	terms make up the GO Big plant subset. The Python notebook files and other 
	resource files for the automated collection of these terms are included in 
	this directory. They can be used to generate the GO terms for other GO Big 
	subsets of interest.

./go.owl.gz
	The GO file release "2024-04-24" in the Web Ontology Language (OWL) file 
	format (downloaded from https://geneontology.org/docs/download-ontology/). 
	This file was used to tag the GO terms collected in the GO_terms directory 
	in Protégé (https://protege.stanford.edu/) to create the gobig_plant.owl 
	file.

./robot
	The directory containing input files and scripts to generate the final 
	gobig_plant files using the ROBOT tool 
	(https://github.com/ontodev/robot/tree/master; 
	https://doi.org/10.1186/s12859-019-3002-3).

./gobig_plant_files
	The directory containing the resulting gobig_plant files in OWL and OBO 
	format.

# END README.txt
