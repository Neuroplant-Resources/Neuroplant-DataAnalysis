## Analysis code for all iterations of the pilot screens
<p>Development of an efficient chemotaxis screening pipeline has been an iterative process. These folders contain the code used to analyze images and data for each iteration of the screen. Following is a brief description of each screen, the screen's goals and a brief description of the folder contents.

### Pilot_screen
<p> This is the image and data analysis code from the first iteration of our screening platform. It includes 3 Jupyter notebooks:</p>
1.  **Neuroplant image analysis** The code reads in .tiff files and uses background subtraction to segment the image and identify the worms. To perform the background subtraction requires two images of the assay plate: before the addition of worms to the plate and after chemotaxis. The code also assumes that the worms will appear dark on a light colored background. Example images from this pilot screen can be found here: **Insert link to folder**
2. **Plot chemotaxis results** Code to generate scatter plots comparing between strains chemotaxis index results from the pilot screens. It will also generate confidence intervals of the same dataset comparing chemotaxis indices between strains
3. **Neuroplant manual analysis comparisons** This contains code to analyze the performance of the first iteration of the automated worm counting algorithm.


### Fall_screen

### 202103_screen
<p> This is the first large scale screen performed after the after the COVID 2020 shutdown. In this iteration of our screening platform we tested 96 different conditions. These conditions include compounds selected for the HEAL pain grant, compounds of interest identified by the NP team as potential chemotaxis modulators absed on literature and complex mixtures from essential oils. For this iteration of the image analysis code we discontinued the use of background selection which allowed us to discontinue capture before and after images of the assay plates, ultimately reducing the amount of data to be stored and captured. The images are also captured using Epson flatbed scanners. The images now render the worms as white on black backgrounds, and are handled accordingly in the image analysis algorithm.
	1.**2103_analysis** Contains all of the code used to analyze the data from the automated image analysis.
	2. 


