# DMSP-Particle-Precipitate-Flux-Prediction-Mesoscale

### **🧾Description:**

We advance the modeling capability of electron particle precipitation from the magnetosphere to the ionosphere through a new database and using deep learning (DL) tools to gain utility from those data. We have compiled, curated, analyzed, and made available a new and more capable database of particle precipitation data that includes 51 satellite years of Defense Meteorological Satellite Program (DMSP) observations temporally aligned with the solar wind and geomagnetic activity data. The new total electron energy flux particle precipitation nowcast model, a neural network called PrecipNet, takes advantage of increased expressive power afforded by ML approaches to appropriately utilize diverse information from the solar wind and geomagnetic activity and, importantly, their time histories. With a more capable representation of the organizing parameters and the target electron energy flux observations, PrecipNet achieves a >50% reduction in errors from a current state‐of‐the‐art model oval variation, assessment, tracking, intensity, and online nowcasting (OVATION Prime), better captures the dynamic changes of the auroral flux, and provides evidence that it can capably reconstruct mesoscale phenomena. We create and apply a new framework for the evaluation of the space weather model that culminates previous guidance from the solar‐terrestrial research community.

Research paper manuscript: [Click Here](https://www.researchgate.net/publication/350946002_Toward_a_Next_Generation_Particle_Precipitation_Model_Mesoscale_Prediction_Through_Machine_Learning_a_Case_Study_and_Framework_for_Progress)

### **🧭 Problem Statement:** 

The target feature is `ELE_TOTAL_ENERGY_FLUX` which is a continuous variable. The task is to predict this variable based on the other 154 features step-by-step by going through each day's task. The scoring metric is `RMSE` or `R2 score.`

Repository Structure
[Model/](https://github.com/SanthoshKumarrS/DMSP-Particle-Precipitate-Flux-Prediction-Mesoscale-/tree/main/Model): Contains the curated dataset of particle precipitation, solar wind, and geomagnetic activity data.
[Notebook/](https://github.com/SanthoshKumarrS/DMSP-Particle-Precipitate-Flux-Prediction-Mesoscale-/tree/main/Notebook): Jupyter notebooks detailing data preprocessing, model development, and evaluation.

**Steps taken to solve the problem**

1. Data analysis using pandas
2. Data cleaning and preprocessing
3. Using Keras Tuner to find optimal units & lr
4. Neural Network model `R2_score - 0.93` 
5. Neural Network model `RMSE score - 0.61`

**Contributing**
We welcome contributions to enhance and expand this project. If you have suggestions, improvements, or new ideas, please open an issue or submit a pull request. Let's collaborate to advance our understanding of electron particle precipitation and its impact on space weather!

**License**
This project is licensed under the MIT License - see the LICENSE file for details.

*Disclaimer*: This project is a research endeavor and may not be suitable for all production applications. Use with care and refer to the license for more details.
