# EEG-based BCI for speech decoding

This work is realized as dissertation research project for the degree of MSc Data Science at the University of Bath. 
 <br>
  <br>
  

Abstract:
 <br>
Many studies have shown that machine earning is a promising tool for speech decoding and
the practical implementation of brain-computer interfaces (BCIs). Of the many technologies
available, a lot of attention has been directed towards EEG due to its being a non-invasive yet
effective method to collect brain signals. In this study we focus on two of the main paradigms
for EEG-based BCIs: inner and imagined speech. We investigate the performance of three
common machine learning algorithms: random forests, support-vector machines and k-nearest
neighbours. In particular, we research which method achieve best performance depending on
the sensory modality of the stimulus which triggers the speaking brain activity. Furthermore,
the impact of word complexity and word repetition on decoding accuracy is analysed for the
paradigms above.
 <br>
  <br>
  
This project has been conducted with the help of two other University of Bath master's students: Ruthwik Hosur Paramashivaiah (<a href="https://github.com/https://github.com/Mithrandir98">Github profile</a>) and Will Adkins (<a href="https://github.com/WillSAdkins">GitHub profile</a>). In particular, the data collection, experimental paradigm and main framework of investigation have been developed collaboratively.

 <br>
  
The dissertation paper can be found here (add link).
  
The data collected can be found <a href="https://drive.google.com/drive/folders/1yOWKGGSMLYj_K_Vaq0wTx6WtS_0xOEDg?usp=sharing">here</a>.

 <br>
This repository contains the following files:

- Prompts <br>
Contains the images and recordings utilized in the experimental paradigm.

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
