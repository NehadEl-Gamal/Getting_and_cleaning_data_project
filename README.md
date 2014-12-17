---
title: "README"
author: "Nehad El-Gamal"
date: "17 ديس, 2014"
output: html_document
---

##Getting and Cleaning Data - Course Project

This repository contain the complete R code and documentation files for the Data Science's track course "Getting and Cleaning data" project.
A full description is available at the site where the data was obtained:
 http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

###Files
* CodeBook.md describes the variables, data, and any transformations or work that was performed to clean up the data.

* run_analysis.R contains all the code to perform the analysis described in the course project page.

* The output of the run_analysis.R code in text formate "averages_data.txt"

##Procedures:

* Download and unzip the data file into your work directory.
* All the similar data is merged using the rbind() function. By similar, we address those files having the same number of columns and referring to the same entities.
* Columns with the mean and standard deviation measures are subseted. then they are given the correct names, taken from features.txt.
* Activity names and IDs from activity_labels.txt and they are substituted in the dataset.
* Columns names are corrected.
* Generate a new dataset with all the average measures for each subject and activity type. The output file is called "averages_data.txt"
