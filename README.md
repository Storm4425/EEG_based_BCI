# EEG-based BCI for speech decoding: a multimodal analysis

This work is realized as dissertation research project for the degree of MSc Data Science at the University of Bath. 
 <br>
  <br>
  

Abstract:
 <br>
Machine learning (ML) is a promising tool for speech decoding and the practical implementation of brain-computer interfaces (BCI). Of the many technologies available, a lot of attention has been directed towards EEG due to its being a non-invasive yet effective method to measure brain activity. In this study we develop a comprehensive experimental paradigm for the study of two of the most important areas of research in EEG-based BCI: imagined and inner speech. We assess which of these paradigms is most suitable for the realization of BCI by analysing the performance of three common ML algorithms: random forests (RF), support-vector machines (SVM) and k-nearest neighbours (KNN). Furthermore, we explore the influence of stimulus modality, word complexity and repeated imagination on speech decoding accuracy.
 <br>


 <br>
  
The data collected can be found <a href="https://drive.google.com/drive/folders/1yOWKGGSMLYj_K_Vaq0wTx6WtS_0xOEDg?usp=sharing">here</a>.

 <br>

To run the main code, please follow these steps:

- Download the data for at least on participant from the link above.
- Open BCI_pipeline.ipynb.
- In the data loading section, change the filepath to match the location of the data on your laptop. 
- If you haven't downloaded data for all participants, ensure that participant variable is set to a participant that you have downloaded.

 <br>
This repository contains the following files:

- Prompts folder <br>
Contains the images and recordings utilized in the experimental paradigm.

- BCI_pipeline.ipynb  <br>
Contains the code for EEG data preprocessing and speech decoding via machine learning.

- CyKit.ps1 <br>
Connects pc to EEG device by utilizing CyKit to initialize OpenVibe acquisition server.

- label_headers.py <br>
Labels the raw csv EEG data.

- OpenVibe_paradigm.xml <br>
Experimental paradigm realized on OpenVibe Designer.

- randomise_trials.ipynb <br>
Randomizes the list of prompts that constitute the experimental paradigm.

- run_paradigm.lua <br>
Allows to run the experimental paradigm and collect data through the OpenVibe acquisition server.
