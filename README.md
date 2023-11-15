# EEG Signal Classification

### Overview
This project focuses on classifying mental states (concentrated, relaxed, and neutral) using EEG recordings. The dataset comprises recordings from four participants, featuring five electrodes across 24 EEG sessions. The goal is to leverage machine learning techniques to interpret EEG data, advancing our understanding of neurological patterns associated with different mental states.

### Dataset Overview
Participants: 4
Electrodes: 5
EEG Sessions: 24
Data Preprocessing
To extract meaningful insights from the EEG recordings, the dataset was processed as follows:

- Segmentation: Each EEG recording was split into 100 segments, allowing for a granular analysis of mental states.
- Feature Extraction: Features such as minimum, maximum, mean, and standard deviation were extracted from each segment. Frequency information was also obtained using a Fast Fourier Transform (FFT).

### Models

##### K-NN Model
The initial model employed a K-Nearest Neighbors (K-NN) classification, achieving an accuracy of 43%. Further refinement and exploration were conducted based on the insights gained from this model.

##### Principal Component Analysis (PCA)
Principal Component Analysis revealed that the first two components are the most relevant in capturing variance within the dataset. This insight influenced subsequent model development.

##### XGBoost Model
The final model utilized XGBoost, incorporating the dimensionality reduction from PCA. This model yielded an accuracy of 70%, showcasing improvements over the initial K-NN model.

### Business Recommendations
The developed model has practical applications in the following areas:

- Mental State Classification: The model can effectively classify mental states, providing valuable insights into distinct brain activity patterns associated with concentration, relaxation, and neutrality.

- Neuromotor Interfaces: As a prototype, this model can pave the way for the development of neuromotor interfaces. These interfaces can interpret brain imaging data, facilitating advancements in brain-computer interfaces and neuroprosthetics.

### Future Improvements
Signal Strength Enhancement:

Investigate signal amplification techniques to address challenges related to weak EEG signals.
Expanded Electrode Coverage:

Collect data from a more extensive array of electrodes to capture a broader spectrum of brain activity, potentially improving model sensitivity.

## Conclusion
This project lays the foundation for leveraging EEG data to classify mental states. By addressing current limitations and exploring future improvements, there is substantial potential for enhancing the accuracy and applicability of the model.
