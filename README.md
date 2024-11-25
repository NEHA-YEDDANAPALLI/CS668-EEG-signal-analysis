# EEG SIGNAL ANALYSIS

Neha / Yeddanapalli


* *This work was realized as part of the capstone project of the MS in Data Science at Pace University*
* **Abstract:** This project focuses on classifying EEG data into seizure and non-seizure using Convolutional Neural Networks. EEG data undergoes preprocessing and converted into 2D data such that it is suitable for input of CNN. In this project, Fast Fourier Transformation is used in order to convert time to frequency domain. The CNN model is trained to identify the patterns in seizure, non seizure data and the performance is evaluated through accuracy and performance metrics. This approach promises reliable solution for real time seizure detection and clinical support in epilepsy management.
* **Dataset:** The CHB-MIT Scalp EEG Database contains scalp EEG recordings from pediatric patients with intractable seizures. This database is compiled by the Children's Hospital Boston and the Massachusetts Institute of Technology.  It includes over 900 hours of EEG data from 23 subjects, with 198 documented seizures. The data was recorded using a 256 Hz sampling rate across 22 channels. This dataset is widely used in epilepsy research to develop algorithms for automated seizure detection.
  * The dataset is available here: https://physionet.org/content/chbmit/1.0.0/
* **Methodology:** Each folder in  the dataset contains a summary text file and each file is consisting information as follows 
    * Channels used in the recording
    * Start time and end time of the file 
    * No of seizures if any 
    * Start time and end time of each seizure if any 
    * The summary text files are parsed and converted into a CSV file 
    * Each signal is then divided into seizure and non seizure portions each portion is an edf    (European data format) file 
    * Then each edf file is converted from an edf file to an npy file where the data is stored in the form of an array facilitating faster processing and compatibility with the deep learning models 

* **Results:** The proposed methodology was evaluated using a dataset consisting of seizure and non-seizure EEG signals, focusing on the model's ability to accurately classify the signals and generalize across multiple folds. The results highlight the effectiveness of the model in leveraging CNN-based architectures for feature extraction and classification.
Key observations from the evaluation include:
**Strengths of the Model:**The model successfully distinguishes between seizure and non-seizure signals with a classification accuracy of 78.94%.This model outperforms traditional machine learning models (e.g., SVM, Random Forest) by learning hierarchical features directly from raw EEG data and leveraging spatial correlations through 2D-CNNs. However, it lacks advanced mechanisms like temporal sequence modeling (RNNs/LSTMs) or attention layers found in more sophisticated EEG classification architectures.
Limitations:This model lacks the attention mechanism and also this model lacks temporal modeling.The classification accuracy could be further improved by extending training duration and utilizing a more diverse dataset.


* Poster (tbd)
