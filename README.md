# ALDA-G11-GalaxyClassificatoin
Repository to store code written by Group 11 (CSC 522: ALDA), Spring 21 offered by Dr. Thomas Price  

This repository contains a bunch of jupyter-notebooks each does a specific task in the pipeline. Those are described below.
These notebooks were written on GoogleColab and we used GoogleDrive as the persistent storage.
These notebooks are not intended to be run outside of the GoogleColab-GoogleDrive environment. 
In order to run them outside, the paths set in the beginning of each notebook will have to be edited.

## Files

* sdss_image_capture.ipynb -> uses the API provided by the Sloan Sky Observatory to get images of elliptical and spiral galaxies
* webscrape_image_capture -> uses the proxycrawl python package to scrape images of irregular images from Google, also invalid images are scraped using this code (but different search strings)
* Augmenting_Iregularimages.ipynb -> performs data-augmentation on the images of irregular galaxies
* Combining_Dataset -> Combines the dataset (until this point images of different classes are stored in different formats in different places), resizes the images, standardizes everything.
* PCA.ipynb -> Performs PCA (and PCA related experiments on the combined dataset)
* svm + RF -> trains Support Vector Machine models and Random Forest models

Collaborators: Ishan Bhatt (ivbhatt), Pragna Bollam (pbollab), Meghana Kota (mkota), Shilpa Kancharla (skancha)

