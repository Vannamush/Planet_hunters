I used data from NASA's Kepler space telescope to train AI models for detecting exoplanets. 
I explored the method of transit photometry, learning how astronomers detect planets orbiting stars. 
The project involves visualizing light curves and identifying exoplanets. 
The aim is to showcase how AI can efficiently classify exoplanet stars and contribute to space exploration.

I was able to identify an exoplanet - NIC 7003

PLANET HUNTERS: Searching for Exoplanets

Project Overview

Planet Hunters is a group project focused on detecting exoplanets using light-curve data from NASA’s Kepler Space Telescope. The project explores how machine-learning models can identify patterns in a star’s brightness that may indicate a planet passing in front of it.

The team experimented with multiple models, including K-Nearest Neighbors (KNN), a neural network, and a Convolutional Neural Network (CNN). The project also examined how data augmentation and preprocessing can help address class imbalance and improve model performance.

Project Goals

Understand how exoplanets can be detected through transit photometry.
Explore Kepler stellar-brightness measurements, also called flux data.
Compare machine-learning models trained with raw and augmented data.
Investigate how data preprocessing and balancing affect model performance.
Explain the models’ results and their ability to identify potential exoplanets.

Data and Methods

The project used existing Kepler light-curve data containing stellar-brightness measurements recorded over time. A transit may cause a small dip in a star’s measured brightness.

The presentation describes these data-processing methods:

SMOTE: Generates synthetic examples to help balance the classes.
Savitzky–Golay filtering: Smooths light curves while preserving their overall trends.
Fourier transformation: Examines frequency patterns in the light curves.
Normalization: Scales values to a range between 0 and 1.
Robust scaling: Scales data using the median and interquartile range (IQR).
The presentation reports that SMOTE produced a balanced dataset with 5,050 samples per class.
Machine-Learning Models

K-Nearest Neighbors (KNN) with Raw Data

The first model used raw Kepler data without the additional augmentation described later in the project.
The presentation identifies a major limitation: the dataset was highly imbalanced, with many more non-exoplanet examples than confirmed exoplanet examples. This caused the model to favor predicting that a star had no exoplanet.

KNN with Augmented Data

The second KNN model used the augmented dataset to address class imbalance.
Reported results:
Training accuracy: 95.4%
Testing accuracy: 90%
Real exoplanets correctly identified in the test: 4 out of 5
These are the results reported in the group presentation and have not been independently recalculated.

Neural Network with Augmented Data

The third model used a neural network trained with augmented data. The presentation describes the model as learning patterns in stellar-brightness measurements that may indicate a transit.
According to the presentation, the model identified 3 out of 5 real planet-hosting stars in the test results.

Convolutional Neural Network (CNN) with Augmented Data

The final model used a CNN to recognize patterns in light curves. The presentation includes convolutional layers, max-pooling layers, a flattening layer, and a sigmoid output for classification.
The presentation reports accuracy of around 99% and shows the model’s classifications in a confusion matrix. These figures describe the results presented by the group; they do not, by themselves, establish how well the model generalizes to new data.

My Contribution

My main role in the Planet Hunters project was research. I also contributed to the presentation, did some coding, and worked with the project’s existing data.

My contributions included the following areas:

Research: Contributed to the research aspect of the project.
Presentation: Contributed to the project presentation.
Coding: Did some coding as part of the project. The specific code or components I wrote were not identified in the information provided.
Data: Worked with existing data rather than collecting new telescope observations myself.
Results: Explained the results reported by the team’s machine-learning models.

I have kept this section limited to the responsibilities I identified as part of the team.

Results and Lessons Learned

The project demonstrated how data imbalance can affect a classifier and how augmentation can change its performance. The presentation reports improved KNN results after using augmented data, along with results from a neural network and a CNN.

The main lessons were:

Raw data may contain substantial class imbalance.
Data balancing and preprocessing can affect model performance.
Different machine-learning architectures may produce different detection results.
Accuracy alone is not enough to establish whether a model reliably detects exoplanets; test-set composition and performance on independent data also matter.

Acknowledgments and Resources

The project used existing Kepler light-curve data and the group’s presentation and script as its project references.
Instructor contributions: The provided materials do not identify specific contributions from instructors, so I have not attributed particular work or resources to them.

Conclusion

Planet Hunters explored the use of machine learning to identify potential exoplanets from Kepler stellar-brightness measurements. By comparing KNN models with raw and augmented data, a neural network, and a CNN, the group investigated the importance of data preparation and model selection.
My role focused primarily on research, with additional contributions to the presentation, some coding, working with existing data, and explaining the team’s reported results.

