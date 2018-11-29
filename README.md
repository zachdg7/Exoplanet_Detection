# Exoplanet Detection with Artificial Neural Networks

#### Note: This project is in stage 2, the results described here and in the technical report are from stage 1. <br>
***Stage 2 Goals:*** <br>
Complete - Label stars as having exoplanets if it has a confirmed exoplanet with an orbit less than the observation period. <br>
In Progress - Turn neural network into a pipeline in order to Gridsearch over various topologies and hyperparameters. <br>
In Progress - Put pipeline on AWS server and run Gridsearch to optimize model. <br>

### Problem Statement:
The purpose of this project is to develop a neural network that can detect planets in other solar systems by analyzing changes in the brightness of stars (light curves). <br>

***Answer the Question:*** <br>
Out of the 5000 stars thought to be visible to the human eye, how many have detectable exoplanets? <br>

### Data Collection and Processing:
The light curve data used in this project was collected by the Kepler Spacecraft and retrieved from NASA's Bulk Data API. <br>
The light curves were cleaned of null values and normally scaled in order to compare stars of different brightnesses. <br>

### Neural Network Modeling:
1156 light curves from stars with confirmed planets mixed into training data when fitting the network. <br>
One-dimensional convolutional neural network engineered to detect transit patterns in lightcurves and classify star as having exoplanets or not. <br>

### Results:
85% accuracy on training dataset. <br>
Predicted 98 stars to have planets out of 5000 stars. <br>
> 12 true exoplanet stars predicted (15 times better than chance). <br>
> 40 actual exoplanet stars in set (30% in predictions). <br>

### Potential Applications
This model would be great for filtering a big data set of stars too large for humans to manually look through. This model could generate a list of stars of interest to analyze further. <br>

<br>

For a detailed description of this project, see the technical report in the links below: <br>

**Table of Contents:** <br>
    [Technical Report](/Technical_Report.ipynb) <br>
    [Data Extraction Notebook](/Data_Extraction.ipynb) <br>
    [Data Cleaning and Labeling Notebook](/Munging.ipynb) <br>
    [Neural Network Modeling Notebook](/models.ipynb) <br>
    
**Extra Technologies Used:** <br>
    Astropy library for opening .fit files <br>
    Wget scripts for downloading from NASA API <br>
    
**External links:** <br>
    Blog Post: <br>
    https://medium.com/datadriveninvestor/finding-a-new-planet-fc088e5d2b55 <br>
    Portfolio: <br>
    https://zachdg7.github.io/ <br>
    LinkedIn: <br>
    https://www.linkedin.com/in/zachary-david-green/ <br>
    
<br>



#### Inspirations and Sources: <br>
List of all confirmed Exoplanets: <br>
http://www.openexoplanetcatalogue.com/systems/?fields=radiusEarth&fields=namelink&fields=numberofstars&fields=systemname&fields=numberofplanets&fields=massEarth&fields=mass&fields=radius&fields=discoverymethod <br>
Google AI's Hunt for Exoplanets: <br>
https://ai.googleblog.com/2018/03/open-sourcing-hunt-for-exoplanets.html <br>
NASA Bulk Data: <br>
https://exoplanetarchive.ipac.caltech.edu/bulk_data_download/



<img src="assets/space_suit.jpg">