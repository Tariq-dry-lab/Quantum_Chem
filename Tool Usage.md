# Repository Structure


M.sc_Project.zip   # contains input data and python script to analyse interaction energy and important internal  
Project Description.md                     # project overview and background  
Tool Usage.md                  # repository structure and usage instructions 
  

## Usage

    Clone the repository:

Unzip the data:

unzip M.Sc_Project.zip

## For  Calculating Internal Coordinates (Bond angle, Bond length and Dihedral Angle)

Prepare the input file:
In coordinate_number.txt file and list the atom IDs for the internal coordinates you want to calculate:

Bond: two atom IDs (e.g., 1 2)

Angle: three atom IDs (e.g., 1 2 3)

Dihedral/Torsion: four atom IDs (e.g., 1 2 3 4)

Run the script:
Execute the Python script to extract the internal coordinates:

    .python3 Internal_coordinates.py N1.pdb coordinate_number.txt output.txt

## Run the analysis script for Analalysing interaction energy:

    python Interaction_ver_2.py

Input files required (per conformer folder N1, N2, P1, P2):

    .log file (quantum chemistry output)

    .pdb file (coordinates)
