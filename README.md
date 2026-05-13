# STAT3In: Computer-Aided Prediction of Inhibitors Against STAT3 for Managing COVID-19 Associated Cytokine Storm

STAT3In is a computational web server developed for the prediction and design of STAT3 inhibitors.

STAT3 is an important transcription factor involved in inflammation, cancer progression, angiogenesis, and cytokine storm. Since IL6-mediated STAT3 activation is associated with COVID-19-related cytokine storm, STAT3In was developed to identify small chemical molecules that may inhibit the STAT3 signaling pathway.

Web Server: https://webs.iiitd.edu.in/raghava/stat3in/



## Citation

Dhall, A., Patiyal, S., Sharma, N., Devi, N. L., and Raghava, G. P. S. Computer-aided prediction of inhibitors against STAT3 for managing COVID-19 associated cytokine storm. Computers in Biology and Medicine, 137, 104780, 2021.

https://doi.org/10.1016/j.compbiomed.2021.104780

This tool and dataset is also available on Zenodo at 



## About the Research

Proinflammatory cytokines are strongly associated with disease severity in COVID-19 patients. IL6-mediated activation of STAT3 can promote inflammatory signaling and contribute to cytokine storm.

STAT3 is a cytoplasmic transcription factor involved in several biological processes such as cell proliferation, differentiation, angiogenesis, inflammation, and apoptosis. However, abnormal activation of STAT3 is associated with cancer, pulmonary fibrosis, acute lung injury, and COVID-19-related cytokine storm.

STAT3In was developed to predict small chemical molecules that may act as STAT3 inhibitors and help in identifying potential candidates for managing IL6/STAT3-mediated inflammatory responses.

Data Compilation: STAT3 inhibitors and non-inhibitors were collected from PubChem BioAssay AID 862. The final dataset contained 1565 STAT3 inhibitors and 1671 non-inhibitors.

Methodology: STAT3In uses machine learning models trained on chemical descriptors and molecular fingerprints. The descriptors were calculated using PaDEL software, and models were developed using classifiers such as Random Forest, Decision Tree, Logistic Regression, Support Vector Classifier, Gaussian Naive Bayes, K-Nearest Neighbour, and eXtreme Gradient Boosting.



## Key Features

### 1. STAT3 Inhibitor Prediction

Predictive Modeling: Allows users to submit chemical compounds and predict whether they are likely to be STAT3 inhibitors or non-inhibitors.

Chemical Input Formats: The server accepts chemical compounds in SDF, SMILES, and MOL formats.

Performance: The fingerprint-based model achieved 0.86 AUC with 78.70% accuracy on the validation dataset.

Hybrid Model: The best hybrid descriptor-based Random Forest model achieved 0.87 AUC with 78.55% accuracy on the validation dataset.



### 2. Descriptor-Based Machine Learning

2-D Descriptors: Models developed using 2-D chemical descriptors achieved maximum AUC of 0.84.

3-D Descriptors: Models developed using 3-D chemical descriptors achieved maximum AUC of 0.73.

Fingerprints: Fingerprint-based models performed better than individual 2-D and 3-D descriptor-based models.

Hybrid Descriptors: A combined feature set using 2-D descriptors, 3-D descriptors, and fingerprints improved the overall prediction performance.

Feature Selection: The study used variance threshold, correlation-based filtering, SVC-L1 feature selection, and feature ranking to identify important descriptors.



### 3. Integrated Web-Bench

Predict Module: Allows users to classify submitted chemical compounds as STAT3 inhibitors or non-inhibitors.

Draw Module: Allows users to draw or modify chemical structures using the Ketcher chemical editor and directly submit them for prediction.

Analog Design Module: Generates chemical analogs using submitted scaffolds, building blocks, and linkers, followed by prediction of their STAT3 inhibition potential.

Batch Prediction: Users can submit single or multiple chemical molecules for prediction.

Downloadable Results: Prediction results are provided in tabular format and can be downloaded as CSV files.



## Applications

COVID-19 Cytokine Storm Research: STAT3In can help identify molecules that may inhibit IL6/STAT3-mediated inflammatory responses associated with cytokine storm.

Cancer Therapy Research: Since STAT3 is involved in tumor progression, angiogenesis, and apoptosis, the tool can support discovery of STAT3-targeting anticancer molecules.

Drug Repurposing: STAT3In was used to screen FDA-approved drugs and identify potential STAT3 inhibitors such as warfarin, dexpanthenol, perindopril, tamoxifen, pentagastrin, duloxetine, ledipasvir, and olopatadine.

Small Molecule Screening: The tool can support virtual screening of chemical libraries for STAT3 inhibition potential.

Molecular Design: The analog design module can help generate and evaluate new chemical analogs as possible STAT3 inhibitors.



## Contact and Authors

Prof. Gajendra P. S. Raghava  
Corresponding Author  

Email: raghava@iiitd.ac.in  

Department of Computational Biology  
Indraprastha Institute of Information Technology Delhi  
Okhla Phase III, New Delhi, India  



## Support

The authors acknowledge the Department of Computational Biology, IIIT Delhi, New Delhi, for infrastructure and facilities.

The authors also acknowledge fellowship support from the Department of Science and Technology INSPIRE program and the Department of Biotechnology, Government of India.
