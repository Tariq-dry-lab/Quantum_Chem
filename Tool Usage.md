# Repository Structure

M.Sc_Project.zip       # Contains input data and Python scripts to analyze interaction energy and important internal coordinates
Project Description.md # Project overview and background
Tool Usage.md          # Repository structure and usage instructions

Usage
1. Clone the repository
2. Unzip the project data
  
## A) Calculating Internal Coordinates (Bond Length, Bond Angle, Dihedral Angle)

    Prepare the input file:
    Create coordinate_number.txt and list the atom IDs for the internal coordinates you want to calculate:

        Bond: two atom IDs (e.g., 1 2)

        Angle: three atom IDs (e.g., 1 2 3)

        Dihedral/Torsion: four atom IDs (e.g., 1 2 3 4)

    Input files required:

        .pdb file for each conformer in their respective folders (N1, N2, P1, P2)

        coordinate_number.txt in the project folder

    Run the script:

python3 Internal_coordinates.py N1.pdb coordinate_number.txt output.txt

    N1.pdb → PDB file of the conformer

    coordinate_number.txt → input atom numbers

    output.txt → file to save the calculated internal coordinates

## B) Analyzing Interaction Energy

    Input files required per conformer folder (N1, N2, P1, P2):

        .log file (quantum chemistry output)

        .pdb file (coordinates)

    Run the analysis script:

python Interaction_ver_2.py

This will calculate interaction energies based on the provided input files.

If you want, I can also add a mini example showing a sample coordinate_number.txt and expected output, which makes it very user-friendly for GitHub users. Do you want me to do that?
