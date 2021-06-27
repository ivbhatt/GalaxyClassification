# ALDA-G11-GalaxyClassification
Repository to store code written by Group 11 (CSC 522: ALDA), Spring 21 offered by Dr. Thomas Price  

This repository contains a bunch of jupyter-notebooks each does a specific task in the pipeline. Those are described below.
These notebooks were written on GoogleColab and we used GoogleDrive as the persistent storage.
These notebooks are not intended to be run outside of the GoogleColab-GoogleDrive environment. 
In order to run them outside, the paths set in the beginning of each notebook will have to be edited. 
Please ensure the proper file structure is present to run web scraping and image augmentation code.

## Description
SDSS telescopes have captured over 40 TB worth of galaxy images and classification of these images is the first step towards obtaining a deeper understanding of physical processes within them, star formation, and the nature of the universe. Since we could not find an easily accessible dataset for galaxy classification, we compiled a dataset for Galaxy classification and provided benchmarks with some of the common learning algorithms that would help in automating the galaxy classification which until recently had to be performed by hand by expert astronomers. We classify the images of galaxies into four classes: spiral, elliptical, irregular, and invalid.

## Files

* sdss_image_capture -> uses the API provided by the Sloan Sky Observatory to get images of elliptical and spiral galaxies
* webscrape_image_capture -> uses the proxycrawl python package to scrape images of irregular images from Google, also invalid images are scraped using this code (but different search strings)
* Augmenting_Iregularimages.ipynb -> performs data-augmentation on the images of irregular galaxies
* Combining_Dataset -> Combines the dataset (until this point images of different classes are stored in different formats in different places), resizes the images, standardizes everything.
* PCA -> Performs PCA (and PCA related experiments on the combined dataset)
* SVM_and_RF-> trains Support Vector Machine models and Random Forest models
* MLP -> trains the MLP model
* CNN -> trains the CNN model
* Demonstrate_NB -> used to fetch all trained models and generate predictions on same data :)
<br>
Collaborators: Ishan Bhatt (ivbhatt), Pragna Bollam (pbollab), Meghana Kota (mkota), Shilpa Kancharla (skancha).

