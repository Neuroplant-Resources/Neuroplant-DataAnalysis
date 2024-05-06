# Neuroplant-DataAnalysis
[![DOI](https://zenodo.org/badge/508834618.svg)](https://zenodo.org/doi/10.5281/zenodo.11122496)
This repository contains all of the code written to analyze the data and generate the figures for the Neuroplant (NP) methods manuscript. The code is broken up into two categories:
1. Data cleaning and intermediate analysis
2. Plotting data for figures

A .yml file has been provided to create a virtual environment so that the code runs smoothly. We recommend using MiniForge, MambaForge, or Miniconda to create your virtual environment. Anaconda works too, but is slow and takes up a lot of disk space.

All worm location data used in these plots were generated using the Neuroplant image analysis software - Our Worm Locator (OWL). The OWL can be cloned from: https://github.com/Neuroplant-Resources/Neuroplant-OWL

#### Mock screen 1 (MS1)
<p> This folder contains the code used to analyze the dataset generated from our "Mock Screen." This screen assessed the response of N2 animals against each of our reference compounds in 16 technical replicates. </p>

1. Mock_assay_compound_randomization.ipynb: Creates a randomized blind key for all of the compounds.
2. MS_analysis: Cleans the data and aggregates worm locations for plotting

#### Manuscript plots
<p> Contains the code used to generate all of the figure plots for the NP screening manuscript.</p>

#### OWL performance analysis
<p>To assess the accuracy of our automated worm locator we compared images processed by the algorithm against the same set of images processed by humans. The metrics that we compared include:</p>
1. The total number of worms identified in each well
2. The position of all worms identified in each well.

Each image was analyzed by the algorithm once and analyzed by 2 separate people. This allowed us to assess the agreement between the algorithm and a human, in addition to the agreement between two humans. 

#### S1
Contains all of the code used to create a randomized compound blinding key, as well as scripts to clean and analyze the data from Screen 1 testing the N2 behavioral response to 96 conditions. It also contains the clean-up and analysis for follow-up screens using the CX10, PR678 (S1F1), and GN1077 (S1F2) mutant lines.

The NP screening pipeline has undergone many iterations, so the data analysis pipeline has gone through similar iterations. We have retained a script that is no longer in use, but was used to create an intermediate dataset for a figure; it has been labeled as deprecated (dep).


