## Analysis code for all iterations of the pilot screens
<p>Development of an efficient chemotaxis screening pipeline has been an iterative process. These folders contain the code used to analyze images and data for each iteration of the screen. Following is a brief description of each screen, the screen's goals and a brief description of the folder contents.

### Pilot_screen
<p> This is the image and data analysis code from the first iteration of our screening platform. It includes 3 Jupyter notebooks:</p>
1.  **Neuroplant image analysis** The code reads in .tiff files and uses background subtraction to segment the image and identify the worms. To perform the background subtraction requires two images of the assay plate: before the addition of worms to the plate and after chemotaxis. The code also assumes that the worms will appear dark on a light colored background. Example images from this pilot screen can be found here: **Insert link to folder**
2. **Plot chemotaxis results** Code to generate scatter plots comparing between strains chemotaxis index results from the pilot screens. It will also generate confidence intervals of the same dataset comparing chemotaxis indices between strains
3. **Neuroplant manual analysis comparisons** This contains code to analyze the performance of the first iteration of the automated worm counting algorithm.


### 202011_screen
<p> This is the first screen performed after the after the COVID 2020 shutdown. In this iteration we introduced a number of improvements to the pilot screening platform. These include:
	1. Using a Multiflow liquid handler to dispense worms onto assay plates 
	2.Using flatbed scanners to capture images instead of the scanning microscope.
	3. Using Gelrite instead of agar in the chemotaxis assay plates.
	4. Increasing the number of compounds tested from 8 to 40.


Our goal for this iteration of the screen was to increase the throughput of the entire pipeline. This was achieved by implementing some of the tools mentioned above. We also discontinued the use of background selection to segment the images, which allowed us to discontinue capture before and after images of the assay plates, ultimately reducing the amount of data to be stored and captured. 

We also tested compounds that aligned with the aims of the HEAL grant, which sought to ID non-opioid compounds to assist with pain management. The compounds that were selected for this screen were selected from a compound library that was donated to the project. The library contained approximately 800 natural, plant derived compounds in DMSO. We used keywords to subset this list for compounds that may influence chemotaxis behaviors and/or manage pain (antinociceptive, antinflamatory, analgesic, etc.)

The jupyter notebooks in this folder was used to clean the data and analyze the results from the screen. </p>

### 202103_screen
<p> In this iteration of our screening platform we tested 96 different conditions. These conditions include compounds selected for the HEAL pain grant, compounds of interest identified by the NP team as potential chemotaxis modulators based on literature searches and complex mixtures from essential oils with purported theraputic properties. Improvements to the screening and analysis pipeline include:

	1. Code to crop images dynamically instead of using hard-coded boundaries.
	2. Migrating metadata capture from multiple Google Forms to a single Google sheet.
	3. Using just 1 solvent (DMSO)
	4. Using 96 well plates to blind and store diluted compounds (20 uM)
	5. Delivering compounds from 96 well alliquot plates to assay plates using multi-channel pipettes.


</p>