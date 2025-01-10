# BEGIN README.txt

GO_terms - README.txt

./1_Get_GO_List.ipynb
	A Python notebook file that extracts the GO terms by category (BP: 
	biological process; MF: molecular function; CC: cellular component) from 
	their respective annotation files under ../annotations. The three resulting 
	files are combined into one file containing all extracted GO terms.
	
./BP_GObig_plant.csv
	Output file of 1_Get_GO_List.ipynb that contains all biological process GO 
	terms extracted from the respective annotation file.

./MF_GObig_plant.csv
	Output file of 1_Get_GO_List.ipynb that contains all molecular function GO 
	terms extracted from the respective annotation file.

./CC_GObig_plant.csv
	Output file of 1_Get_GO_List.ipynb that contains all cellular component GO 
	terms extracted from the respective annotation file.

./all_GObig_plant.csv
	Output file of 1_Get_GO_List.ipynb that contains all GO terms extracted from
	the annotation files. This file is an input for 2_Get_GOBig_Ancestors.ipynb.

./2_Get_GOBig_Ancestors.ipynb
	A Python notebook file for automatic generation of the list of ancestors 
	for the extracted GO terms. The go.obo file used and relationships 
	considered can be modified. This file creates an output that includes all 
	extracted GO terms and their ancestor terms. Each term appears once.
	
./go_2024-04-24.obo.gz
	The GO file release "2024-04-24" in the OBO file format (downloaded from 
	https://geneontology.org/docs/download-ontology/). This file was used in 
	both 2_Get_GOBig_Ancestors.ipynb and 
	3_Additional_Terms_From_Taxon_Constraints.ipynb Python notebooks to load the
	GO and relationships between terms. This file can be substituted with a 
	another release.
	
./Gobig_plant_with_ancestors.csv
	Output file of 2_Get_GOBig_Ancestors.ipynb that contains the list of all 
	extracted GO terms from the annotation files along with their ancestor GO 
	terms. This file is an input for 
	3_Additional_Terms_From_Taxon_Constraints.ipynb.

./go_taxon_constraints.owl.gz
	The GO taxon constraints file in the Web Ontology Language (OWL) file 
	format that was used to find any GO term labelled with “only in taxon” for 
	the class Viridiplantae that was not already included in the 
	Gobig_plant_with_ancestors.csv file (due to the absence of their assignment 
	as a function with an experimental evidence code to a plant gene). For more 
	information about GO taxon constraints: 
	https://geneontology.org/docs/taxon-constraints/.

./Plant_taxon_constraints.csv
	File containing a list of GO terms labelled with “only in taxon” for the 
	class Viridiplantae that were not already included in the 
	Gobig_plant_with_ancestors.csv file. This file is an input for 
	3_Additional_Terms_From_Taxon_Constraints.ipynb to capture more plant 
	functions to be represented in the final subset of GO terms.

./3_Additional_Terms_From_Taxon_Constraints.ipynb
	A Python notebook file similar to 2_Get_GOBig_Ancestors.ipynb for automatic 
	generation of the list of ancestor terms for the GO terms derived from the 
	Plant_taxon_constraints.csv file. The go.obo file used and relationships 
	considered can be modified. This file creates an output that adds the GO 
	terms derived from the Plant_taxon_constraints.csv file and their ancestor 
	terms to the ones in the Gobig_plant_with_ancestors.csv file. Each term 
	appears once.

./GObig_plant_final.csv
	Output file for 3_Additional_Terms_From_Taxon_Constraints.ipynb that 
	contains the list of all GO terms of interest including the additional terms 
	derived from Plant_taxon_constraints.csv and their ancestor GO terms. These 
	terms make up the GO Big plant subset.

# END README.txt
