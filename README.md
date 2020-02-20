# Automated script to download charmm parameter files of ligands from swissparam

Script uses beautiful soup to scrape webpage of swissparam. Can be used to obtain charmm parameter (.par, .rtf, .str, .psf, .pdf, .mol2, .itp) files from the webserver.
Input consists - ligand mol2 file with all hydrogens.

# Usage
python swiss.py -i file.mol2


(From SwissChem - more information on correct mol2 file) :
How to obtain a correct mol2 file?
Please, note that the mol2 files submitted to SwissParam should contain all the hydrogen atoms of the molecule.

First of all, try the mol2 file you already have . Most of the mol2 files will work, whatever their origin. If one fails, you can try one of the following:
get it from the ZINC Database if the molecule is already known,

or, if the molecule comes from a PDB file (e.g. a ligand), you can use the UCSF chimera visualization software to open the PDB file, remove all molecules except the one of interest, add hydrogen atoms (using the Tools/Structure Editing/AddH menu), and save it as a mol2 file,

or use openbabel to convert a correct 3D file from another format into the mol2 format,

or draw the molecule in 2D in Chemaxon Marvin Sketch (free), add hydrogens, generate 3D coordinates and save the molecule in the "MDL molfile (mol)" format. Then convert the mol file into a mol2 file using openbabel.

This list is not exhaustive. If you have trouble getting a working mol2 file, please contact us.

