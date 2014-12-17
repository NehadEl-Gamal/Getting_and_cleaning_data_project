---
title: "README"
author: "Nehad El-Gamal"
date: "17 ديس, 2014"
output: html_document
---

##Getting and Cleaning Data - Course Project

This repository hosts the R code and documentation files for the Data Science's track course "Getting and Cleaning data" project.
A full description is available at the site where the data was obtained:
 http://archive.ics.uci.edu/ml/datasets/Human+Activity+Recognition+Using+Smartphones

###Files
* CodeBook.md describes the variables, the data, and any transformations or work that was performed to clean up the data.

* run_analysis.R contains all the code to perform the analyses described in the course project page.

* The output of the run_analysis.R code in text formate "averages_data.txt"

##Procedures:
The script run_analysis.Rperforms the 5 steps described in the course project's definition.

* Download and unzip the data file into your work directory.
* First, all the similar data is merged using the rbind() function. By similar, we address those files having the same number of columns and referring to the same entities.
* Then, only those columns with the mean and standard deviation measures are taken from the whole dataset. After extracting these columns, they are given the correct names, taken from features.txt.
* As activity data is addressed with values 1:6, we take the activity names and IDs from activity_labels.txt and they are substituted in the dataset.
* On the whole dataset, those columns with vague column names are corrected.
* Finally, we generate a new dataset with all the average measures for each subject and activity type (30 subjects * 6 activities = 180 rows). The output file is called averages_data.txt, and uploaded to this repository.
