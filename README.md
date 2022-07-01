# Neuroplant-DataAnalysis -- README in production
This repository contains all of the code written to perform the data analysis for the Neuroplant methods manuscript.

**Note** Any files that start with "dep_" are depricated versions of files. I will remove these once I am fully confident they do not contain usefull chunks of code

### Pilot_screen
<p> This is the image and data analysis code from the first iteration of our screening platform. It includes 3 Jupyter notebooks:</p>
1.  **Neuroplant image analysis** The code reads in .tiff files and uses background subtraction to segment the image and identify the worms. To perform the background subtraction requires two images of the assay plate: before the addition of worms to the plate and after chemotaxis. The code also assumes that the worms will appear dark on a light colored background. Example images from this pilot screen can be found here: **Insert link to folder**
2. **Plot chemotaxis results** Code to generate scatter plots comparing between strains chemotaxis index results from the pilot screens. It will also generate confidence intervals of the same dataset comparing chemotaxis indices between strains
3. **Neuroplant manual analysis comparisons** This contains code to analyze the performance of the first iteration of the automated worm counting algorithm.

### 202103_screen
<p> This is the first large scale screen performed after the after the COVID 2020 shutdown. In this iteration of our screening platform we tested 96 different conditions. These conditions include compounds selected for the HEAL pain grant, compounds of interest identified by the NP team as potential chemotaxis modulators absed on literature and complex mixtures from essential oils. For this iteration of the image analysis code we discontinued the use of background selection which allowed us to discontinue capture before and after images of the assay plates, ultimately reducing the amount of data to be stored and captured. The images are also captured using Epson flatbed scanners. The images now render the worms as white on black backgrounds, and are handled accordingly in the image analysis algorithm.

### MS1
<p> This folder contains the code used to analyze the dataset generated from our "Mock Screen." This screen assessed the response of N2 animals against each of our reference compounds. The dataset contains 16 technical replicates for each test condition.</p>

