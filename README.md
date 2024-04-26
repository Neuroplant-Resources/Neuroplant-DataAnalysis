# Neuroplant-DataAnalysis
This repository contains all of the code written to analyze the data and generate the figures for the Neuroplant (NP) methods manuscript. The code is broken up into two categories:
1. Data cleaning and intermediate analysis
2. Rendering figures

#### Mock screen 1 (MS1)
<p> This folder contains the code used to analyze the dataset generated from our "Mock Screen." This screen assessed the response of N2 animals against each of our reference compounds in 16 technical replicates. All worm location data were generated using the Neuroplant image analysis software - Our Worm Locator (OWL).</p>

1. Mock_assay_compound_randomization.ipynb: Creates a randomized blind key for all of the compounds.
2. MS_analysis: Cleans the data and aggregates worm locations for plotting

#### Manuscript plots
<p> Contains the code used to generate all of analysis plots for the NP screening manuscript </p>

#### OWL performance analysis
<p>The contents include 2 performance analyses of the OWL performed in Spring 2021 and Spring 2022.</p>

#### S1
<p> Contains all of the code used to analyze the data from Screen 1 testing the N2 behavioral response to 96 conditions. It also contains the analysis for follow up screens using the CX10, PR678 and GN1077 mutant lines.</p>

The NP screening pipeline has undergone many iterations and so the data analysis has gone through similar iterations. We have retained a few scriptsf that are no longer in use, but have labeled these as deprecated (dep).

#### Screen development
<p> This contains code used to analyze the data from all previous iterations of the screening pipeline. There is more detail about the contents of this folder in the README found inside. </p>

#### DivergentStrains
<p> One of the offshoot projects includes screening a set of C. elegans wild isolates known as the divergent strains. This folder contains the initial code used to clean up and analyze this dataset.</p>

