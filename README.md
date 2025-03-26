# **Speaker Ethnicity Recognition Using Speech Processing**  

## **1. Project Overview**  
This project focuses on the classification of British speakers in Birmingham based on ethnicity using machine learning techniques. The goal is to distinguish between two ethnic groups—*Asian* and *White*—using extracted audio features from spoken speech samples.  

## **2. Dataset Description**  
The dataset consists of WAV audio files stored in a structured directory format on Google Drive:  
- *`dataset/train/'* – Training data, further divided into:  
  - `Asian/`  
    - `male/` (Speeches from Asian male speakers)  
    - `female/` (Speeches from Asian female speakers)  
  - `White/`  
    - `male/` (Speeches from White male speakers)  
    - `female/` (Speeches from White female speakers)
      
- *`dataset/test/`* – Testing data, structured as:  
  - `Asian/` (Speeches from Asian speakers)  
  - `White/` (Speeches from White speakers)  

(Gender information is present in the dataset but is not considered relevant for classification—only ethnicity is used for the task)

** --> To see dataset, follow the Link:** https://drive.google.com/drive/folders/1qjyiC9Em7cWzliiozLODm01NDsOAj0WK?usp=drive_link
  
## **3. Feature Extraction**  
Each audio file undergoes feature extraction using the `Librosa` library. Extracted features include:  
- **Energy** (overall loudness of speech)  
- **Zero-Crossing Rate** (rate of sign changes in the waveform)  
- **Pitch** (fundamental frequency of speech)  
- **MFCCs (Mel-frequency Cepstral Coefficients)**  
  - 12 MFCCs  
  - Delta-MFCCs (first-order derivative)  
  - Delta-Delta MFCCs (second-order derivative)  

These extracted features are stored in a CSV file for training and testing machine learning models.

## **4. Machine Learning Models**  
At least two machine learning models must be implemented. Potential choices include:  
- **K-Nearest Neighbors (KNN)** – A non-parametric classifier that measures similarity between feature vectors.  
- **Gaussian Mixture Model (GMM)** – A probabilistic model that represents feature distributions as a mixture of Gaussian distributions.  
- **Support Vector Machine (SVM)** – A robust classifier that finds an optimal hyperplane for separating classes.  

## **5. Evaluation Metrics**  
Performance will be evaluated using:  
- **Accuracy** – Percentage of correctly classified samples.  
- **Precision, Recall, F1-score** – Metrics to assess classification balance.  
- **Confusion Matrix** – Visual representation of misclassification rates.  

##  Contributing
We welcome contributions! If you find an issue or want to enhance the project, feel free to Submit a pull request

##  Contact
For any inquiries, feel free to reach out:
- **Email:**(mailto:dana.gassad03@gmail.com)
