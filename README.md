# EEG-Classification-of-Alcoholic-Schizophrenic-Depressed-and-Healthy

## Steps Involved 

### Step - 1 : Generalization of Channels 
Out of the variety of EEG channels available, we came down to 15 channels which was common is all 3 datasets. 

### Step - 2 : Principal Component Analysis 
From those 15 channels, we analysed and extracted 8 Principal Components which capture > 95% of the variance. 

### Step - 3 : Resampling of EEG Signals 
The sampling frequency of the EEG Signals of the 3 datasets was different. So we re-sampled the Signals to a common sampling frequency of 250 Hz using mne-python.

### Step - 4 : Model Creation, Training and Evaluation
We extracted exactly 250 samples from each subject file belonging to each category for the training purpose. Therefore, each input for the Neural Network was of the shape, 250 rows (samples) and 8 columns (Principal Components). After training and testing, the gave an accuracy of > 95% 

