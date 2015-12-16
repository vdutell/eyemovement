# eyemovement
## A project studying fixational eye movement  

Vasha DuTell  
vasha@berkeley.edu  
vashadutell@gmail.com  


# Files:

## EyeMovementFilerGenerate.ipynb
EyeMovementFilterGenerate is the cleanest version of the code, functionalized and commented for calling from an outside pipeline. 
This file contains the most important parts of the code, including the defintion of the Eyetrace datatype, the preprocessing of the eyetrace data,  as well as the Brownain Motion and Velocity models implemented as a Kalman Filter and as an eyetrace generator. The parameters for running these filters and generators are used here, but the documentation for chosing the parameters (the justification for their fit) are not validated here.

## EyeMovementAnalysis.ipynb
EyeMovementAnalysis is an in depth analysis of the statistics of the eyetraces, as well as justification for the fitting of the parameters used by the Kalmann Filter and the trace generations for the Brownian Motion and Velocity models. It also contains code analyzing the error from both the AOSLO and the covariance from the Velocity Model Kalman filter, and how that error propogates through higer derivatives of position (velocity, acceleration, etc).
This file has some comments, but is NOT functionalized for use by calling from another external pipeline.

## EyeMovementResearchNotes.ipynb
EyeMovementResearchNotes links to and summarizes the reavlent pervious work on the topic of fixational drift and eye movement in general. It contains both the relavent papers to the characteristsics of microsaccades and drift, as well as more general information from Wikipedia.

## /oldcode/Eye Movement Single Readin.ipynb
This is the first version of the code developed to read in just 4 eyemovement traces, taken under the same stimulus condition, but at a higher frame rate. Most of its contents is included and improved in EyeMovementAnalysis, but is retained for completeness.
