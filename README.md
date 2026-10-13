### **Project CB2330**

🪸 *Predicting Severe Coral Bleaching Events with a GLMM: replacing calendar time with climate parameters to improve model performance* 🪸

---
In the article *Spatial and temporal patterns of mass bleaching of corals in the Anthropocene* by Hughes et al. (2018) predictions about the severity of coral bleaching were made by using a generalized linear mixed model (GLMM). They observed 100 reef locations in 4 regions from 1980 to 2016 and noted if there was a severe (>30% of the area), moderate (>29% of the area), or no bleaching event. They then used this data to determine the spatial and temporal patterns of bleaching since entering the Anthropocene era (since 1980).

The authors demonstrated the long term trend that severe coral bleaching increased using Region and Time as their fixed effects, and specific reef locations as their random effect. They suggest that climate and ENSO (El Nino Southern Oscillation) data is a contributor to bleaching events, but they only imply a relation between time and temperature that results in a model that does not quite capture the upward and downward trend of their observations where severe bleaching events spike during warm phases.

The aim of this project is to use the model suggested by the authors and compare it to a new model where one of their fixed effects (Time) is replaced by climate predictors (global temperature anomaly and Nino 3.4 temperature anomaly).

Following their method of modelling in R (using the glmer() function), we retrieve the coefficients of our model and show some analysis in the notebook:
- How might a coefficient be predicted with a backwards simulation.
- How our model compares to the observed data and whether we can better predict climate phase-related spikes and drops better than the researchers' model
- How often the observations fall into the range of values our model predicts across 400 forward simulations

Although our model assumes that this phenomenon can be modelled by a linear relationship and has many limitations since factors such as reef depth or species are not considered, it was able to fit to the up-and-down trend of the observed data when compared to the researchers' model.The researchers more so use time to show us that bleaching changed while our climate variables propose an explanation for why it changed.

---
### **How to run the repository**

🪸 Go to the Github repository: 
https://github.com/qhtni/CB2330-project/blob/main/PRO1_Group8_2330.ipynb

🪸 Click the "Open in Colab" button in the top left corner to open the notebook in Google Colab. Or download the file and then open it in Google Colab.

🪸 The code is set up to collect the necessary data directly from this repository which means that an active internet connection is required in order to run the cells. 

🪸 Now the that the NoteBook is in Google Colab: Click on **Runtime** in the Colab menu and choose **Run all**

---



---


