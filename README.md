# Exoplanet Detection with Artificial Neural Networks

### Problem Statement:
The purpose of this project is to develop a neural network that can detect planets in other solar systems by analyzing changes in the brightness of stars (light curves). <br>

#### Answer the question: <br>
Out of the 5000 stars thought to be visible to the human eye, how many have detectable exoplanets? <br>

### Data Collection and Processing:
The light curve data used in this project was collected by the Kepler Spacecraft and retrieved from NASA's Bulk Data API. <br>
The light curves were cleaned of null values and normally scaled in order to compare stars of different brightnesses. <br>

### Neural Network Modeling:
1100 light curves from stars with confirmed planets mixed into training data when fitting the network. <br>
1 dimensional convolutional neural network used to detect transit patterns in lightcurves and classify star as having exoplanets or not. <br>

### Results:
85% accuracy on training dataset. <br>
Predicted 98 stars to have planets out of 5000 stars. <br>
> 12 true exoplanet stars predicted (15 times better than chance). <br>
> 40 actual exoplanet stars in set (30% in predictions). <br>

<br>

For a detailed description of this project, see the technical report in the links below: <br>

**Table of Contents:** <br>
    [Technical Report](/Technical_Report.ipynb) <br>
    [Data Extraction Notebook](/Data_Extraction.ipynb) <br>
    [Data Munging Notebook](/Munging.ipynb) <br>
    [Modeling Notebook](/models.ipynb) <br>
    
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