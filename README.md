# hiv-spread
Repository Structure
1. 22140-0001-Data.tsv
Raw data file obtained from the ICPSR NAHDAP HIV Transmission Network dataset (CO90).
Contains demographic attributes and contact edges (sexual and needle-sharing) for ~50,000 individuals from 1988–2001.
Used as the source dataset for all simulations.
NOTE: 22140-0002-Data.tsv was also used for initial network creation, however file was too large to upload and emailed by Nikhil instead

3. Project.ipynb
Initial development notebook.
Includes early data cleaning, demographic filtering, and preliminary attempts at SI simulations.
Replaced by Project_v2.ipynb but kept for transparency of development.

4. Project_v2.ipynb
Main analysis notebook for the final project. All relevant code for generating figures can be found starting on line [210], this code references variables established in early sections as it retains code that was not deleted upon advice from Professor Landry.
This notebook contains the full analysis route used in the report, including:
Loading and cleaning the HIV network data
Constructing demographic-specific subnetworks (age, race, sex)
Separating sexual and needle-sharing contact layers
Implementing the stochastic SI contagion model
Running 100-run simulations for each demographic subgroup
Simulating infection trajectories over time
Calculating final epidemic sizes and statistics 
Generating all figures used in the final report
