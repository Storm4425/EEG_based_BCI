# Using AI to read the mind: EEG-based brain-computer interface for multi-modal speech decoding

This work is realized as dissertation research project for the degree of MSc Data Science at the University of Bath. 
 <br>
  <br>
  

Abstract:
 <br>
Machine learning (ML) is a promising tool for speech decoding and the practical implementation of brain-computer interfaces (BCI). Of the many technologies available, a lot of attention has been directed towards EEG due to its being a non-invasive yet effective method to measure brain activity. In this study we develop a comprehensive experimental paradigm and gather experimental data from 9 participants. We study two of the most important areas of research in EEG-based BCI: imagined and inner speech, with a focus on practical implementation within the healthcare domain. We assess which of these paradigms is most suitable for the realization of BCI by analysing the performance of three common ML algorithms: random forests (RF), support-vector machines (SVM) and k-nearest neighbours (KNN). Furthermore, we explore the influence of stimulus modality, word complexity and repeated imagination on speech decoding accuracy. We obtain statistically significant results well above chance-level, notably for RF and audio-elicited prompts.
 <br>


 <br>
  
The dissertation paper can be found at https://laidlawscholars.network/manage/documents/192939 and the data collected can be found at https://drive.google.com/drive/folders/1yOWKGGSMLYj_K_Vaq0wTx6WtS_0xOEDg?usp=sharing (data available until 09/09/27).

 <br>


To run the main code, please follow these steps:

- 1. Download the data for at least on participant from the link above.
- 2. Open the Jupiter notebook BCI_pipeline.ipynb. This contains the main code along with instructions and comments.
- 3. In the data loading section, change the filepath to match the location of the data on your laptop.
- 4. If you haven't downloaded data for all participants, ensure that the participant variable is set to the participant data that you have downloaded.

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

 <br>
 Reproducibility:
 
- The EPOC+ Emotiv headset device can be found at https://www.emotiv.com/epoc/.
- OpenViBE designer and acquisition server, and CyKit were downloaded from https://github.com/scottwellington/FEIS/tree/v1.1 packages.
- Emotiv applications downloaded from https://www.emotiv.com/emotiv-launcher/.
