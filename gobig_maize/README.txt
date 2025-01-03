# BEGIN README.txt

gobig_maize - README.txt

./annotations
	Annotations for Zea mays (taxon ID: 4577) downloaded from the Gene Ontology 
	Annotation (GOA) database (https://www.ebi.ac.uk/QuickGO/; 
	https://doi.org/10.1093/nar/gku1113). Files are split by GO category (BP: 
	biological process; MF: molecular function; CC: cellular component). Gene-GO 
	term pairs are derived through filtering by GO terms (The GO Slim plant 
	subset terms were used as identifiers to find GO terms that map back to 
	them), and by evidence (experimental evidence codes were selected - 
	ECO:0000352, ECO:0000269, ECO:0000314, ECO:0000315, ECO:0000316, 
	ECO:0000353, ECO:0000270, ECO:0006056, ECO:0007005, ECO:0007001, 
	ECO:0007003, and ECO:0007007).

./GO_terms
	GO terms and their ancestor terms collected manually using QuickGO 
	(https://www.ebi.ac.uk/QuickGO/; 
	https://doi.org/10.1093/bioinformatics/btp536). These terms make up the 
	GO Big maize subset. Files are split by GO category (BP: biological process; 
	MF: molecular function; CC: cellular component). An example image of a 
	directed acyclic graph (DAG) is added to this directory to demonstrate how 
	a GO term and its ancestors were manually chosen and added to the files 
	based on the GO category.

./go.owl.gz
	The GO file release "2023-10-09" in the Web Ontology Language (OWL) file 
	format (downloaded from https://geneontology.org/docs/download-ontology/). 
	This file was used to tag the GO terms collected in the GO_terms directory 
	in Protégé (https://protege.stanford.edu/) to create the gobig_maize.owl 
	file.

./robot
	The directory containing input files and scripts to generate the final 
	gobig_maize files using the ROBOT tool 
	(https://github.com/ontodev/robot/tree/master; 
	https://doi.org/10.1186/s12859-019-3002-3).

./gobig_maize_files
	The directory containing the resulting gobig_maize files in OWL and OBO 
	format.

# END README.txt
